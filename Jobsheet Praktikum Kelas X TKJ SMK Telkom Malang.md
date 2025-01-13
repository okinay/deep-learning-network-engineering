### Jobsheet Praktikum Kelas X TKJ SMK

#### **Tujuan Pembelajaran**

Siswa diharapkan mampu:

1. Memahami konsep dasar virtualisasi dan CentOS secara mendalam.
2. Menggunakan VirtualBox untuk membuat, mengelola, dan memodifikasi virtual machine dengan konfigurasi lanjutan.
3. Menginstal, mengonfigurasi, dan mengelola CentOS beserta layanan seperti DNS dan Web Server dengan pendekatan yang terstruktur.
4. Mengembangkan keterampilan troubleshooting serta kemampuan implementasi proyek nyata yang relevan dengan kebutuhan industri.
5. Mampu mendokumentasikan seluruh proses secara profesional untuk mendukung pemahaman teknis yang berkelanjutan.

---

#### **Petunjuk Praktikum**

1. Awali praktikum dengan doa untuk memohon kelancaran.
2. Pelajari dan pahami teori yang relevan sebelum memulai aktivitas praktikum.
3. Ikuti setiap langkah yang tertulis pada jobsheet dengan teliti dan seksama.
4. Jika menghadapi kendala atau ketidakjelasan, segera tanyakan kepada instruktur untuk mendapatkan penjelasan yang lebih rinci.
5. Laksanakan semua tugas dengan sikap jujur, bertanggung jawab, dan disiplin tinggi.
6. Dokumentasikan seluruh aktivitas praktikum untuk keperluan evaluasi dan pembelajaran lanjutan.

---

#### **Alat dan Bahan**

- **Perangkat Keras**:
  - Komputer/Laptop dengan spesifikasi minimal RAM 8GB dan penyimpanan 100GB.
  - Koneksi internet stabil untuk mengunduh perangkat lunak dan pembaruan.
- **Perangkat Lunak**:
  - VirtualBox versi terbaru (minimal 7.x).
  - File ISO CentOS 7 atau 8 (versi terbaru direkomendasikan).
  - Editor teks seperti Nano, Vim, atau Visual Studio Code.

---

#### **Dasar Teori**

1. **Virtualisasi**: Teknologi yang memungkinkan eksekusi sistem operasi dalam lingkungan virtual pada perangkat keras yang sama.
2. **CentOS**: Sistem operasi berbasis Linux yang dikenal stabil, aman, dan digunakan secara luas pada server di lingkungan produksi.
3. **DNS Server**: Layanan penting dalam jaringan yang menerjemahkan nama domain menjadi alamat IP sehingga memudahkan akses ke layanan tertentu.
4. **Web Server**: Perangkat lunak yang digunakan untuk menyajikan halaman web dan mendukung pengembangan layanan berbasis internet.
5. **Troubleshooting**: Proses sistematis untuk menganalisis, mengidentifikasi, dan memperbaiki permasalahan teknis pada sistem atau jaringan.

---

#### **Latihan Praktikum**

##### **Pekan 1: Pengenalan Virtualisasi dan Instalasi CentOS**

1. **Langkah 1: Instalasi VirtualBox**

   - Unduh VirtualBox dari situs resminya.
   - Instal perangkat lunak sesuai dengan sistem operasi yang digunakan.

2. **Langkah 2: Unduh ISO CentOS**

   - Kunjungi situs resmi CentOS dan unduh file ISO versi terbaru.

3. **Langkah 3: Membuat Virtual Machine**

   - Buka VirtualBox dan buat mesin virtual baru dengan pengaturan berikut:
     - Nama: CentOS-VM
     - Jenis OS: Linux
     - Versi: Red Hat (64-bit)
     - Alokasi RAM: 2GB atau lebih.

4. **Langkah 4: Menghubungkan ISO CentOS**

   - Masukkan ISO CentOS sebagai disk boot pada pengaturan storage VirtualBox.

5. **Tugas Praktikum**:

   - Dokumentasikan proses pembuatan Virtual Machine dan lampirkan tangkapan layar setiap langkah.

---

##### **Pekan 2: Konfigurasi Virtual Machine dan Instalasi CentOS**

1. **Langkah 1: Pengaturan Virtual Machine**

   - Konfigurasi jaringan VM ke mode "Bridged Adapter" untuk koneksi internet.
   - Alokasikan penyimpanan minimal 20GB untuk sistem operasi CentOS.

2. **Langkah 2: Instalasi CentOS**

   - Boot Virtual Machine menggunakan ISO CentOS.
   - Ikuti wizard instalasi dengan langkah berikut:
     - Pilih bahasa: English.
     - Pilih software: Minimal Install.
     - Konfigurasi partisi: Automatic.
     - Atur hostname: centos.local.

3. **Langkah 3: Verifikasi Instalasi**

   - Setelah instalasi selesai, reboot sistem dan login sebagai root.

4. **Tugas Praktikum**:

   - Buat laporan proses instalasi dengan catatan konfigurasi yang digunakan.

---

##### **Pekan 3: Konfigurasi Dasar CentOS**

1. **Langkah 1: Update Sistem**

   - Jalankan perintah berikut untuk memperbarui sistem:
     ```bash
     sudo yum update -y
     ```

2. **Langkah 2: Konfigurasi Jaringan**

   - Edit file konfigurasi jaringan di `/etc/sysconfig/network-scripts/ifcfg-<interface>`.
   - Set IP statis, subnet mask, dan gateway.

3. **Langkah 3: Mengatur Hostname**

   - Ubah hostname menggunakan perintah:
     ```bash
     sudo hostnamectl set-hostname centos.moklet-tkj.com
     ```

4. **Tugas Praktikum**:

   - Dokumentasikan konfigurasi jaringan dan hostname.

---

##### **Pekan 4: Instalasi dan Konfigurasi BIND (DNS Server)**

1. **Langkah 1: Instalasi BIND**

   - Instal layanan DNS Server menggunakan perintah berikut:
     ```bash
     sudo yum install bind bind-utils -y
     ```

2. **Langkah 2: Konfigurasi named.conf**

   - Edit file `/etc/named.conf` dan sesuaikan pengaturan zona.

3. **Langkah 3: Membuat Zona DNS**

   - Tambahkan file zona untuk domain "moklet-tkj.com" di direktori `/var/named`.

4. **Langkah 4: Pengujian DNS**

   - Gunakan perintah `dig` dan `nslookup` untuk memastikan DNS berfungsi.

5. **Tugas Praktikum**:

   - Laporkan hasil konfigurasi dan pengujian DNS Server.

---

##### **Pekan 5: Integrasi DNS dan Web Server**

1. **Langkah 1: Instalasi Web Server**

   - Instal Apache menggunakan perintah berikut:
     ```bash
     sudo yum install httpd -y
     ```

2. **Langkah 2: Konfigurasi Virtual Host**

   - Tambahkan virtual host untuk domain "moklet-tkj.com" di `/etc/httpd/conf.d/moklet-tkj.com.conf`.

3. **Langkah 3: Pengujian Integrasi**

   - Restart layanan Apache dan DNS menggunakan perintah berikut:
     ```bash
     sudo systemctl restart httpd
     sudo systemctl restart named
     ```
   - Gunakan browser untuk mengakses "moklet-tkj.com".

4. **Tugas Praktikum**:

   - Dokumentasikan langkah integrasi dan hasil pengujian.

---

##### **Pekan 6: Troubleshooting DNS dan Web Server**

1. **Langkah 1: Analisis Log**

   - Periksa log error DNS di `/var/log/messages` dan log Apache di `/var/log/httpd/error_log`.

2. **Langkah 2: Uji Konektivitas**

   - Gunakan perintah `ping`, `dig`, dan `curl` untuk memeriksa koneksi dan respons server.

3. **Langkah 3: Perbaikan Masalah Umum**

   - Perbaiki kesalahan konfigurasi berdasarkan log dan hasil pengujian.

4. **Tugas Praktikum**:

   - Buat laporan troubleshooting dengan solusi yang diterapkan.

---

##### **Pekan 7-12: Proyek Akhir**

1. **Langkah 1: Perencanaan**

   - Identifikasi kebutuhan proyek, seperti implementasi layanan DNS dan Web Server untuk aplikasi tertentu.

2. **Langkah 2: Implementasi**

   - Konfigurasi lengkap DNS dan Web Server sesuai dengan skenario proyek.

3. **Langkah 3: Pengujian dan Dokumentasi**

   - Uji layanan yang dikembangkan dan buat dokumentasi proyek secara menyeluruh.

4. **Tugas Praktikum**:

   - Presentasikan hasil proyek kepada instruktur dan teman sejawat.

---

