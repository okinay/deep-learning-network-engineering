# 📘 Jobsheet Praktikum: Deep Learning Network Engineering
## Kelas X TKJ - SMK Telkom Malang (Detailed Edition)

![CentOS](https://wiki.centos.org/attachments/ArtWork(2f)Brand(2f)Logo/centos-logo-light-vertical.svg)

---

### 📌 Ringkasan Program
Jobsheet ini adalah panduan komprehensif bagi siswa untuk menguasai teknologi jaringan dan server menggunakan CentOS. Kurikulum ini dirancang untuk membawa siswa dari tingkat pemula (dasar virtualisasi) hingga mampu mengelola infrastruktur server yang kompleks.

> [!NOTE]
> **Tujuan Utama**: Membekali siswa dengan keterampilan teknis (*hard skills*) dan dokumentasi profesional (*soft skills*) yang relevan dengan standar industri IT masa kini.

---

## 📦 Modul 1: Fondasi Virtualisasi & Instalasi OS
*(Estimasi: Pekan 1 - 2)*

### 🟦 Pekan 1: Pengenalan Lingkungan Virtual
Siswa belajar mengelola *Virtual Machine* (VM) sebagai simulasi server nyata.

1. **Instalasi VirtualBox**: Pastikan mengunduh versi 7.x atau terbaru.
2. **Setup VM**:
   - Nama: `CentOS-VM`
   - RAM: `2048MB` (Min) - `4096MB` (Recom).
   - Storage: `20GB` Dynamic Allocated.
3. **Mounting ISO**: Masukkan file ISO CentOS ke tab **Storage > Controller IDE**.

---

### 🟦 Pekan 2: Instalasi CentOS dengan Pendekatan Server
Instalasi dilakukan dengan mode **Minimal Install** untuk meminimalkan beban sistem.

1. **Network Configuration**: Interface pertama diatur ke **Bridged Adapter** untuk akses internet.
2. **Software Selection**: Pilih **"Minimal Install"**.
3. **Partitioning**: Pilih **"Automatic"** (LVM secara default).
4. **Post-Installation**: Setelah reboot, login menggunakan user `root`.

---

## 💻 Modul 2: Eksplorasi Linux & Remote Management
*(Estimasi: Pekan 3 - 4)*

### 🟦 Pekan 3: Penguasaan Terminal (Deep Dive)
Terminal adalah alat utama administrator server. Berikut adalah detail perintah yang wajib dikuasai:

#### 1. Navigasi & File System
- `pwd` (Print Working Directory): Mengetahui posisi folder saat ini.
- `ls -lah`: Menampilkan list file beserta file tersembunyi (`a`), format detail (`l`), dan ukuran yang mudah dibaca/human-readable (`h`).
- `cd /var/log`: Pindah ke direktori log sistem.
- `touch file.txt`: Membuat file kosong baru.
- `mkdir -p folder/subfolder`: Membuat folder beserta parent-nya sekaligus.

#### 2. Manajemen Izin (Permissions)
- `chmod 755`: Owner bisa segalanya (Read/Write/Execute), Group & Others hanya Read/Execute.
- `chown root:named /var/named/zonefile`: Mengubah pemilik file menjadi user `root` dan group `named`.

#### 3. Update & Package Manager (YUM/DNF)
- `sudo yum update -y`: Memperbarui semua repository dan paket ke versi terbaru.
- `sudo yum install <nama_paket>`: Mencari dan mengunduh paket dari internet.

---

### 🟦 Pekan 4: Manajemen Jaringan & Remote Server
Administrator jarang masuk langsung ke server fisik; mereka mengonfigurasi IP statis agar server selalu dapat dihubungi melalui kabel jaringan.

#### 1. Konfigurasi IP Statis (NMCLI)
CentOS secara default menggunakan **NetworkManager** untuk mengelola koneksi.
- **Cek Interface**: `nmcli connection show`
  *(Perhatikan nama koneksi, misalnya `enp0s8` untuk adapter Host-Only).*
- **Set IP Statis**: `192.168.100.1` dengan subnet `/24`.
  ```bash
  nmcli connection modify enp0s8 ipv4.addresses 192.168.100.1/24 ipv4.method manual
  ```
  *(Flags: `modify` mengubah profil, `addresses` menentukan IP, `method manual` mengaktifkan mode statis).*
- **Aktifkan Perubahan**:
  ```bash
  nmcli connection up enp0s8
  ```
- **Verifikasi Akhir**: `ip a` (Pastikan IP baru sudah muncul pada interface yang benar).

#### 2. Remote Server (SSH & SCP)
Setelah IP server statis, Anda dapat mengaksesnya dari laptop tanpa harus membuka layar VirtualBox.

#### 2.1. Setup SSH (Secure Shell)
Secara default CentOS sudah mengaktifkan SSH di port 22.
- **Cek Status Service**: `systemctl status sshd`
- **Remote dari Host/Laptop**:
  Buka Windows Terminal atau PowerShell (Pastikan IP VM bisa diping):
  ```bash
  ssh root@192.168.100.1
  ```
  *(Masukkan password root saat diminta).*

#### 2.2. Pengiriman File Aman (SCP)
Mengirim file dari Laptop (Host) ke Server (Guest) atau sebaliknya:
- **Kirim dari Host ke Server**:
  ```bash
  scp tugas_praktikum.pdf root@192.168.100.1:/home/root/
  ```
- **Ambil log dari Server ke Host**:
  ```bash
  scp root@192.168.100.1:/var/log/messages ./log_copy.txt
  ```

> [!TIP]
> Gunakan aplikasi **WinSCP** (Windows) atau **FileZilla** untuk manajemen file server dengan antarmuka grafis (GUI) melalui protokol SFTP/SSH.

---

## 🌐 Modul 3: Layanan Inti Jaringan (Detailed Config)
*(Estimasi: Pekan 5 - 6)*

### 🟦 Pekan 5: DNS Server (BIND)
Langkah detail konfigurasi BIND untuk domain `moklet-tkj.com`.

1. **Instalasi**: `sudo yum install bind bind-utils -y`.
2. **Edit `/etc/named.conf`**:
   ```bash
   listen-on port 53 { 127.0.0.1; any; }; # Izinkan listen di semua IP
   allow-query { any; };                  # Izinkan query dari mana saja
   ```
3. **Membuat Zone File (`/var/named/moklet-tkj.com.zone`)**:
   ```bash
   $TTL 86400
   @ IN SOA ns1.moklet-tkj.com. admin.moklet-tkj.com. ( 2025010101 3600 1800 604800 86400 )
   @   IN NS  ns1.moklet-tkj.com.
   ns1 IN A   192.168.100.1
   www IN A   192.168.100.1
   ```
4. **Verifikasi**: `named-checkconf /etc/named.conf` dan `named-checkzone moklet-tkj.com /var/named/moklet-tkj.com.zone`.

---

### 🟦 Pekan 6: Web Server (Apache)
Administrator web harus memahami cara menginstal paket dasar hingga mengelola banyak situs dalam satu server.

#### 6.1. Instalasi & Pengujian Dasar
Tahap awal adalah memastikan layanan Apache dapat berjalan dan melayani konten statis.
- **Instalasi**:
  ```bash
  sudo yum install httpd -y
  ```
- **Aktivasi Service**:
  ```bash
  systemctl start httpd
  systemctl enable httpd
  ```
- **Mengganti Tampilan Default**:
  Secara default Apache menampilkan halaman tes. Untuk menggantinya dengan buatan sendiri:
  ```bash
  # Pindah ke direktori utama web
  cd /var/www/html/
  
  # Buat file index.html baru
  nano index.html
  ```
  Isi `index.html` dengan kode sederhana:
  ```html
  <html>
  <body>
      <h1>Selamat Datang di Server Saya!</h1>
      <p>Halaman ini dibuat sebagai hasil praktikum TKJ Pekan 6.</p>
  </body>
  </html>
  ```
- **Pengujian Awal**:
  Gunakan browser di laptop Anda dan akses IP server (`http://192.168.100.1`). Anda seharusnya melihat tampilan HTML yang baru saja dibuat, bukan lagi halaman tes default.

> [!IMPORTANT]
> Pastikan port 80 (HTTP) sudah dibuka di firewall agar halaman tes dapat diakses dari luar VM.

#### 6.2. Konfigurasi Virtual Host
Digunakan agar satu server dapat menghosting domain unik seperti `moklet-tkj.com`.
- **Persiapan Folder**:
  ```bash
  mkdir -p /var/www/html/moklet
  echo "<h1>Web Lab TKJ Sudah Aktif!</h1>" > /var/www/html/moklet/index.html
  ```
- **Buat File Konfigurasi (`/etc/httpd/conf.d/moklet.conf`)**:
  ```apache
  <VirtualHost *:80>
      ServerName moklet-tkj.com
      ServerAlias www.moklet-tkj.com
      DocumentRoot /var/www/html/moklet
      
      <Directory /var/www/html/moklet>
          Options Indexes FollowSymLinks
          AllowOverride All
          Require all granted
      </Directory>
  </VirtualHost>
  ```
- **Restart & Verifikasi**:
  Selalu restart setelah mengubah file `.conf`:
  ```bash
  systemctl restart httpd
  ```
  Akses domain `http://moklet-tkj.com` di browser. Jika DNS BIND sudah benar, pesan "Web Lab TKJ Sudah Aktif!" akan muncul.

---

## 🔍 Modul 4: Security & Troubleshooting
*(Estimasi: Pekan 7)*

### 🛡️ Firewall Management (Firewalld)
Server tidak akan bisa diakses jika port tidak dibuka di firewall.
- `firewall-cmd --permanent --add-service=dns`
- `firewall-cmd --permanent --add-service=http`
- `firewall-cmd --reload`

### 🔧 Troubleshooting Loop
Jika service gagal jalan (`Failed`), gunakan:
1. `journalctl -xe`: Melihat error log terbaru.
2. `systemctl status <service>`: Cek baris error spesifik.
3. `ping` & `dig`: Cek koneksi fisik dan resolusi nama.

---

## 🚀 Praktikum Lanjut: Studi Kasus & Proyek
*(Pekan 8 - 13)*

Fokus pada kemandirian siswa dalam menghadapi skenario industri:
- **Pekan 8-11**: Implementasi Subdomain dan Hardening (Keamanan).
- **Pekan 12**: Simulasi Disaster Recovery (Perbaikan konfigurasi yang rusak).
- **Pekan 13**: **Proyek Akhir Terintegrasi** (Full setup DNS + Web + Remote + Firewall).

---

## 🛠️ Command Toolbox (Quick Reference)

| Kategori | Perintah | Deskripsi |
| :--- | :--- | :--- |
| **System** | `systemctl restart <name>` | Me-restart layanan |
| | `hostnamectl` | Cek identitas server |
| **Network** | `nmcli con mod <itf> ipv4.method manual` | Set IP Statis |
| | `ip addr show` | Melihat detail IP interface |
| **Remote** | `ssh user@ip` | Akses remote server |
| | `scp local_file user@ip:/path` | Copy file ke remote |
| **Security** | `firewall-cmd --list-all` | Cek aturan firewall aktif |

---

## 📊 Matriks Capaian & Checklist
| Modul | Deliverable | Deadline | Status |
| :--- | :--- | :---: | :---: |
| **Modul 1** | Laporan Setup VM & Install OS | Pekan 2 | [ ] |
| **Modul 2** | Akses Remote SSH Success | Pekan 4 | [ ] |
| **Modul 3** | Domain & Web Lab Aktif | Pekan 6 | [ ] |
| **Modul 4** | Laporan Troubleshooting | Pekan 7 | [ ] |
| **Portfolio**| Proyek Akhir (Final Report) | Pekan 13 | [ ] |

---
*Curated with ❤️ for SMK Telkom Malang Students.*
