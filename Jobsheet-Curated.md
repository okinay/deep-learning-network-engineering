# 📘 Jobsheet Praktikum: Deep Learning Network Engineering
## Kelas X TKJ - SMK Telkom Malang (Curated Edition)

![CentOS](https://wiki.centos.org/attachments/ArtWork(2f)Brand(2f)Logo/centos-logo-light-vertical.svg)

---

### 📌 Ringkasan Program
Jobsheet ini adalah panduan komprehensif bagi siswa untuk menguasai teknologi jaringan dan server menggunakan CentOS. Kurikulum ini dirancang untuk membawa siswa dari tingkat pemula (dasar virtualisasi) hingga mampu mengelola infrastruktur server yang kompleks (DNS & Web Server).

> [!NOTE]
> **Tujuan Utama**: Membekali siswa dengan keterampilan teknis (hard skills) dan dokumentasi profesional (soft skills) yang relevan dengan standar industri IT masa kini.

---

### 🛠️ Persiapan Awal
Sebelum memulai, pastikan perangkat Anda memenuhi spesifikasi berikut:

- **Perangkat Keras**: Laptop/PC dengan RAM Minimal 8GB, Penyimpanan Bebas 100GB.
- **Koneksi**: Internet stabil untuk unduhan ISO dan update paket.
- **Perangkat Lunak**:
  - [VirtualBox 7.x+](https://www.virtualbox.org/)
  - [ISO CentOS 9 Stream / 10](https://www.centos.org/download/)
  - Editor Teks: Nano, Vim, atau VS Code.

---

## 📦 Modul 1: Fondasi Virtualisasi & Instalasi OS
*(Estimasi: Pekan 1 - 2)*

### 🟦 Pekan 1: Pengenalan Lingkungan Virtual
Fokus pada instalasi tool utama dan pembuatan lingkungan virtual yang stabil.

1. **Instalasi VirtualBox**: Pastikan instalasi berhasil tanpa error driver.
2. **Setup Virtual Machine (VM)**:
   - Nama: `CentOS-VM`
   - Tipe: `Linux`, Versi: `Red Hat (64-bit)`
   - RAM: Minimal `2048MB` (2GB).
3. **Mounting ISO**: Menghubungkan file ISO CentOS ke storage VM.

> [!TIP]
> Gunakan alokasi RAM yang cukup (misal 4GB jika laptop Anda memiliki 16GB) agar proses instalasi berjalan lebih cepat.

#### 📝 Tugas Pekan 1:
Buat laporan (PDF) yang berisi screenshot tahapan pembuatan VM dan penjelasan singkat mengenai konfigurasi hardware yang Anda pilih.

---

### 🟦 Pekan 2: Instalasi & Konfigurasi OS
Fokus pada proses instalasi CentOS yang optimal untuk server.

1. **Konfigurasi Jaringan VM**: Gunakan mode **"Bridged Adapter"** agar VM bisa mendapatkan akses internet langsung saat instalasi.
2. **Parameter Instalasi**:
   - **Language**: English (Standard industri).
   - **Software Selection**: **Minimal Install** (Untuk performa maksimal).
   - **Partitioning**: Automatic.
   - **Hostname**: `centos.local`.
3. **Login Pertama**: Verifikasi user `root` dan pastikan sistem dapat booting dengan sempurna.

---

## 💻 Modul 2: Eksplorasi Linux & Manajemen Jaringan
*(Estimasi: Pekan 3 - 4)*

### 🟦 Pekan 3: Penguasaan Terminal & Hirarki Sistem
Sangat krusial untuk memahami struktur folder Linux sebelum mengelola layanan.

#### 📂 Hirarki Direktori Utama:
- `/etc`: Pusat konfigurasi sistem (Jantung server).
- `/var`: Data dinamis (log, database, web files).
- `/root` & `/home`: Area kerja user.
- `/bin` & `/sbin`: Command executable.

#### ⌨️ Skill Wajib (Basic Commands):
| Perintah | Fungsi | Contoh |
| :--- | :--- | :--- |
| `ls -l` | List file detail | `ls -l /etc` |
| `cd` | Pindah direktori | `cd /var/www` |
| `mkdir` | Membuat folder | `mkdir project1` |
| `chmod` | Izin akses | `chmod 755 script.sh` |
| `yum update` | Update sistem | `sudo yum update -y` |

---

### 🟦 Pekan 4: Konfigurasi Jaringan Lanjut
Mengatur konektivitas antar mesin (Host-to-Guest).

1. **Dual Network Interface**:
   - **Adapter 1**: NAT (Untuk akses internet).
   - **Adapter 2**: Host-Only (Untuk komunikasi antara laptop Anda dan VM).
2. **Setup IP Statis**:
   Menggunakan NMCLI untuk interface Host-Only:
   ```bash
   # Contoh interface enp0s8
   nmcli connection modify enp0s8 ipv4.addresses 192.168.100.1/24 ipv4.method manual
   nmcli connection up enp0s8
   ```
3. **Uji Koneksi**: Pastikan laptop Anda bisa melakukan `ping 192.168.100.1`.

---

## 🌐 Modul 3: Layanan Inti Jaringan (DNS & Web Server)
*(Estimasi: Pekan 5 - 6)*

### 🟦 Pekan 5: DNS Server (BIND)
Memahami sistem penerjemahan nama domain ke IP.

1. **Instalasi BIND**:
   ```bash
   sudo yum install bind bind-utils -y
   ```
2. **Konfigurasi `named.conf`**: Fokus pada IP Listen dan Allow-Query.
3. **Zona DNS**: Menambahkan domain `moklet-tkj.com`.
4. **File Zona**: Mengisi A-Record dan NS-Record.

> [!IMPORTANT]
> Jangan lupa mengatur izin file (Permissions) ke `root:named` pada direktori `/var/named/` agar service BIND dapat membaca konfigurasi zona.

#### 🔭 Uji DNS:
Verifikasi dengan `dig` atau `nslookup`:
```bash
dig @192.168.1.1 www.moklet-tkj.com
```

---

### 🟦 Pekan 6: Web Server (Apache)
Implementasi Virtual Host untuk menghosting banyak situs.

1. **Instalasi Apache**: `sudo yum install httpd -y`.
2. **Virtual Host**: Setup domain `moklet-tkj.com` di `/etc/httpd/conf.d/`.
3. **Integrasi**: Pastikan DNS mengarah ke IP Server dan Web Server menyajikan file `index.html` yang benar.

---

## 🔍 Modul 4: Diagnosa & Troubleshooting
*(Estimasi: Pekan 7)*

Fokus pada penyelesaian masalah (Troubleshooting) yang sering muncul.

1. **Analisis Log**:
   - `/var/log/messages`: Error sistem/DNS.
   - `/var/log/httpd/error_log`: Error Apache.
2. **Uji Konektivitas**: Gunakan `ping`, `dig`, and `curl`.
3. **Common Issues**: Firewall blocking port 80/53, Syntax error in config files.

> [!CAUTION]
> Selalu reboot service (`systemctl restart service`) setelah melakukan perubahan pada file konfigurasi mana pun.

---

## 🚀 Praktikum Lanjut: Studi Kasus & Proyek Akhir
*(Estimasi: Pekan 8 - 13)*

Program ini diakhiri dengan serangkaian tantangan dunia nyata untuk menguji kemandirian siswa.

### 💼 Pekan 8 - 12: Seri Tantangan Korporat
- **Pekan 8**: Domain Lokal Bisnis (`moklet.local`).
- **Pekan 9**: Hosting Landing Page Tim Dev.
- **Pekan 10**: Hardening Server (Firewall Configuration).
- **Pekan 11**: Integrasi Subdomain (`admin.moklet.local`).
- **Pekan 12**: Disaster Recovery (Simulasi kerusakan server).

### 🏆 Pekan 13: Proyek Akhir Terintegrasi
Membangun infrastruktur full-stack untuk `moklet-project.local` dengan dua subdomain (`www` & `api`) serta pengamanan firewall yang ketat.

---

## 🛠️ Command Toolbox (Cheat Sheet)

### 🐧 Sistem & File
- `hostnamectl set-hostname <nama>` : Mengubah nama server.
- `top` : Monitoring penggunaan RAM & CPU.
- `ls -la` : Melihat semua file termasuk hidden files.
- `nano /path/ke/file` : Mengedit file teks dengan cepat.

### 🌐 Jaringan & Service
- `ip a` : Cek IP Address yang aktif.
- `nmcli connection show` : Melihat list koneksi jaringan.
- `systemctl start <service>` : Menjalankan layanan (httpd, named).
- `systemctl enable <service>` : Membuat layanan otomatis jalan saat boot.

### 🛡️ Firewall (Kritis)
- `firewall-cmd --add-port=80/tcp --permanent` : Membuka port Web.
- `firewall-cmd --reload` : Menerapkan perubahan firewall.

---

## 📊 Matriks Capaian & Checklist
Gunakan tabel ini untuk melacak kemajuan belajar Anda:

| Modul | Pekan | Deskripsi | Status | Deliverable |
| :--- | :--- | :--- | :---: | :--- |
| **Foundations** | 1 | VirtualBox & VM Setup | [ ] | Laporan PDF VM |
| | 2 | CentOS Installation | [ ] | Screenshot Login root |
| **Linux Essentials**| 3 | Perintah Dasar Linux | [ ] | Quiz Basic Commands |
| | 4 | IP Statis & NMCLI | [ ] | Uji Ping Success |
| **Infrastructure** | 5 | DNS BIND Setup | [ ] | Output Dig/Nslookup |
| | 6 | Apache Virtual Host | [ ] | Tampilan Index Web |
| **Maintenance** | 7 | Troubleshooting Log | [ ] | Log Analysis Report |
| **Portfolio** | 13 | Proyek Akhir | [ ] | Demo & Dokumentasi |

---
*Curated with ❤️ for SMK Telkom Malang Students.*
