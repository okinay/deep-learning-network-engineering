# Jobsheet Praktikum Kelas X TKJ SMK

![Logo CentOS](https://wiki.centos.org/attachments/ArtWork(2f)Brand(2f)Logo/centos-logo-light-vertical.svg)  

## **Ringkasan Tujuan Jobsheet**
Jobsheet ini dirancang untuk memberikan panduan langkah demi langkah kepada siswa dalam memahami dan mengimplementasikan teknologi jaringan dan server, mulai dari dasar hingga tingkat lanjut. Siswa diharapkan mampu:

1. Memahami konsep virtualisasi dan mengelola virtual machine menggunakan VirtualBox.
2. Menginstal dan mengonfigurasi sistem operasi CentOS beserta layanan seperti DNS dan Web Server.
3. Melakukan troubleshooting pada layanan jaringan.
4. Menyelesaikan proyek akhir yang mencakup integrasi berbagai layanan untuk skenario dunia nyata.
5. Mempresentasikan hasil proyek dengan dokumentasi teknis yang baik.

---

## **Tujuan Pembelajaran**

Siswa diharapkan mampu:

1. Memahami konsep dasar virtualisasi dan CentOS secara mendalam, termasuk bagaimana teknologi virtualisasi dapat mempermudah pengelolaan server dan infrastruktur jaringan dalam skala besar. Pemahaman ini bertujuan untuk membantu siswa mengembangkan keterampilan dasar yang esensial dalam dunia kerja berbasis teknologi.
2. Menggunakan VirtualBox untuk membuat, mengelola, dan memodifikasi virtual machine dengan konfigurasi lanjutan.
3. Menginstal, mengonfigurasi, dan mengelola CentOS beserta layanan seperti DNS dan Web Server dengan pendekatan yang terstruktur.
4. Mengembangkan keterampilan troubleshooting serta kemampuan implementasi proyek nyata yang relevan dengan kebutuhan industri.
5. Mampu mendokumentasikan seluruh proses secara profesional untuk mendukung pemahaman teknis yang berkelanjutan.

---

## **Petunjuk Praktikum**

1. Awali praktikum dengan doa untuk memohon kelancaran.
2. Pelajari dan pahami teori yang relevan sebelum memulai aktivitas praktikum.
3. Ikuti setiap langkah yang tertulis pada jobsheet dengan teliti dan seksama.
4. Jika menghadapi kendala atau ketidakjelasan, segera tanyakan kepada instruktur untuk mendapatkan penjelasan yang lebih rinci.
5. Laksanakan semua tugas dengan sikap jujur, bertanggung jawab, dan disiplin tinggi.
6. Dokumentasikan seluruh aktivitas praktikum untuk keperluan evaluasi dan pembelajaran lanjutan.

---

## **Alat dan Bahan**

- **Perangkat Keras**:
  - Komputer/Laptop dengan spesifikasi minimal RAM 8GB dan penyimpanan 100GB.
  - Koneksi internet stabil untuk mengunduh perangkat lunak dan pembaruan.
- **Perangkat Lunak**:
  - VirtualBox versi terbaru (minimal 7.x).
  - File ISO CentOS 9 dan 10 (versi terbaru direkomendasikan). File ISO bisa diunduh di [centos.org](https://www.centos.org/download/).
  - Editor teks seperti Nano, Vim, atau Visual Studio Code.

---

## **Dasar Teori**

1. **Virtualisasi**: Teknologi yang memungkinkan eksekusi sistem operasi dalam lingkungan virtual pada perangkat keras yang sama.
2. **CentOS**: Sistem operasi berbasis Linux yang dikenal stabil, aman, dan digunakan secara luas pada server di lingkungan produksi.
3. **DNS Server**: Layanan penting dalam jaringan yang menerjemahkan nama domain menjadi alamat IP sehingga memudahkan akses ke layanan tertentu.
4. **Web Server**: Perangkat lunak yang digunakan untuk menyajikan halaman web dan mendukung pengembangan layanan berbasis internet.
5. **Troubleshooting**: Proses sistematis untuk menganalisis, mengidentifikasi, dan memperbaiki permasalahan teknis pada sistem atau jaringan.

---

## **Latihan Praktikum**

### **Pekan 1: Pengenalan Virtualisasi dan Instalasi CentOS**

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

   - Dokumentasikan proses pembuatan Virtual Machine dengan menyusun laporan yang mencakup langkah-langkah berikut:

1. **Persiapan Awal**:
   - Unduh perangkat lunak VirtualBox dan file ISO CentOS.
   - Cantumkan spesifikasi minimum yang digunakan.

2. **Langkah-Langkah Pembuatan**:
   - Buat mesin virtual baru dan atur pengaturan seperti nama, jenis OS, alokasi RAM, dan pengaturan penyimpanan.
   - Tambahkan file ISO sebagai media instalasi.

3. **Tangkapan Layar**:
   - Lampirkan tangkapan layar setiap langkah utama, termasuk:
     - Tampilan pengaturan nama dan jenis OS.
     - Pengaturan alokasi RAM dan penyimpanan.
     - Penambahan ISO sebagai media instalasi.

4. **Catatan Tambahan**:
   - Jelaskan alasan memilih konfigurasi tertentu.
   - Sertakan kendala yang mungkin dihadapi selama proses ini dan cara penyelesaiannya.

Gunakan format dokumen PDF untuk laporan dan pastikan setiap tangkapan layar diberi keterangan yang jelas.

---

### **Pekan 2: Konfigurasi Virtual Machine dan Instalasi CentOS**

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
   - Sertakan tangkapan layar dari setiap langkah instalasi, termasuk:
     - Pemilihan bahasa dan software.
     - Konfigurasi partisi dan hostname.
     - Tampilan login setelah instalasi selesai.
---

### **Pekan 3: Konfigurasi Dasar CentOS dan Perintah Dasar Linux**

Sebelum melanjutkan ke instalasi layanan jaringan, siswa perlu memahami konfigurasi dasar CentOS dan perintah dasar Linux. Pada praktikum ini, siswa akan mempelajari langkah-langkah dasar untuk mengelola sistem operasi dan memahami perintah dasar yang digunakan dalam lingkungan Linux. 

Dan siswa perlu tahu terkait dengan hirarki direktori pada linux, berikut adalah penjelasannya: 
Gambar Hirarki Direktori Linux
![Hirarki Direktori Linux](https://blogger.googleusercontent.com/img/b/R29vZ2xl/AVvXsEgOQ7VdeB3zTl7w6VhCQdw9tAJKcXcj1UO7FbJJ_GRQfjj4cnus_zIIzkMgunmi94zMpBF40O1qpUuoiz3C3OEPSeZjNP4kvWSrQDmSOyKODggY3M5otnxkzwfMx8gwkB2wZIg3F-e0pnY/s1600/linux-filesystem.png)

- `/` : direktori root, merupakan direktori utama pada sistem operasi Linux.
- `/bin` : berisi file biner (eksekutabel) yang digunakan oleh pengguna dan sistem.
- `/boot` : berisi file yang diperlukan untuk proses booting sistem.
- `/dev` : berisi file yang terkait dengan perangkat keras.
- `/etc` : berisi file konfigurasi sistem.
- `/home` : berisi direktori pengguna.
- `/lib` : berisi library yang digunakan oleh program.
- `/media` : berisi direktori untuk media penyimpanan sementara.
- `/mnt` : berisi direktori untuk media penyimpanan sementara.
- `/opt` : berisi direktori untuk paket aplikasi tambahan.
- `/proc` : berisi informasi proses sistem.
- `/root` : direktori home untuk pengguna root.
- `/run` : berisi file yang dibuat oleh sistem saat boot.
- `/sbin` : berisi file biner (eksekutabel) yang digunakan oleh sistem.
- `/srv` : berisi data yang disediakan oleh server.
- `/sys` : berisi informasi tentang perangkat keras.
- `/tmp` : berisi file sementara.
- `/usr` : berisi file yang tidak berubah selama sistem berjalan.
- `/var` : berisi file yang sering berubah saat sistem berjalan.

Untuk memahami konfigurasi dasar CentOS dan perintah dasar Linux, siswa akan mempelajari langkah-langkah berikut:

1. **Langkah 1: Perintah Dasar Linux**

   1. **Navigasi File System** 
   Di Linux, direktori dan file diatur dalam struktur hirarkis. Perintah dasar untuk navigasi file system adalah: 
      - **Format Perintah**:  
         - Melihat isi direktori:  
            ```bash
            ls [opsi] [direktori]
            ```  
         - Berpindah direktori:  
            ```bash
            cd [direktori]
            ```  
      - **Contoh Perintah**:  
         - Menampilkan isi direktori saat ini dalam format terperinci:  
            ```bash
            ls -l
            ```  
         - Berpindah ke direktori `/etc`:  
            ```bash
            cd /etc
            ```  

   2. **Manajemen File dan Direktori**  
   Perintah dasar untuk manajemen file dan direktori adalah: 
      - **Format Perintah**:  
         - Membuat file kosong:  
            ```bash
            touch [nama_file]
            ```  
         - Membuat direktori:  
            ```bash
            mkdir [nama_direktori]
            ```  
         - Menghapus file atau direktori:  
            ```bash
            rm [opsi] [nama_file/direktori]
            ```  
         - Memindahkan atau mengganti nama file:  
            ```bash
            mv [nama_file] [lokasi_tujuan]
            ```  
      - **Contoh Perintah**:  
         - Membuat file bernama `contoh.txt`:  
            ```bash
            touch contoh.txt
            ```  
         - Membuat direktori bernama `folder_baru`:  
            ```bash
            mkdir folder_baru
            ```  
         - Menghapus file `contoh.txt`:  
            ```bash
            rm contoh.txt
            ```  
         - Memindahkan file `contoh.txt` ke `/tmp`:  
            ```bash
            mv contoh.txt /tmp
            ```  

   3. **Manajemen Perizinan File** 
   Perintah dasar untuk manajemen perizinan file adalah:
      - **Format Perintah**:  
         - Mengubah izin file:  
            ```bash
            chmod [mode] [nama_file]
            ```  
         - Mengubah kepemilikan file:  
            ```bash
            chown [user]:[grup] [nama_file]
            ```  
      - **Contoh Perintah**:  
         - Memberikan izin `read`, `write`, dan `execute` kepada pemilik file:  
            ```bash
            chmod 755 contoh.txt
            ```  
         - Mengubah pemilik file `contoh.txt` menjadi user `root`:  
            ```bash
            chown root:root contoh.txt
            ```  

   4. **Pemantauan Sistem**  
   Perintah dasar untuk pemantauan sistem adalah:
      - **Format Perintah**:  
         - Melihat proses yang berjalan:  
            ```bash
            ps [opsi]
            ```  
         - Melihat penggunaan CPU dan memori secara real-time:  
            ```bash
            top
            ```  
      - **Contoh Perintah**:  
         - Menampilkan semua proses yang berjalan dalam format lengkap:  
            ```bash
            ps aux
            ```  
         - Menjalankan **top** untuk melihat statistik penggunaan sistem:  
            ```bash
            top
            ```  

   5. **Pengelolaan Jaringan**  
   Perintah dasar untuk pengelolaan jaringan adalah:
      - **Format Perintah**:  
         - Menampilkan informasi jaringan:  
            ```bash
            ip [opsi]
            ```  
         - Menguji konektivitas jaringan:  
            ```bash
            ping [opsi] [alamat_ip/nama_domain]
            ```  
      - **Contoh Perintah**:  
         - Menampilkan alamat IP dan status interface:  
            ```bash
            ip a
            ```  
         - Mengirim 4 ping ke `google.com`:  
            ```bash
            ping -c 4 google.com
            ```  

   6. **Manajemen Paket**
   Perintah dasar untuk manajemen paket adalah:  
      - **Format Perintah**:  
         - Menginstal paket:  
            ```bash
            yum install [nama_paket] -y
            ```  
         - Menghapus paket:  
            ```bash
            yum remove [nama_paket] -y
            ```  
      - **Contoh Perintah**:  
         - Menginstal layanan web server `httpd`:  
            ```bash
            sudo yum install httpd -y
            ```  
         - Menghapus layanan web server `httpd`:  
            ```bash
            sudo yum remove httpd -y
            ```  


2. **Langkah 2: Update Sistem**

   - Jalankan perintah berikut untuk memperbarui semua paket dalam sistem agar sesuai dengan versi terbaru:
     ```bash
     sudo yum update -y
     ```

3. **Langkah 3: Konfigurasi Jaringan**

   - Edit file konfigurasi jaringan di direktori `/etc/sysconfig/network-scripts/` sesuai dengan nama interface yang digunakan, seperti `ifcfg-ens33`. Contoh isi file konfigurasi:
     ```
     TYPE=Ethernet
     BOOTPROTO=static
     IPADDR=192.168.1.10
     NETMASK=255.255.255.0
     GATEWAY=192.168.1.1
     DNS1=8.8.8.8
     ```
   - Setelah melakukan konfigurasi, restart layanan jaringan:
     ```bash
     sudo systemctl restart network
     ```

4. **Langkah 4: Mengatur Hostname**

   - Ubah hostname menggunakan perintah berikut:
     ```bash
     sudo hostnamectl set-hostname centos.moklet-tkj.com
     ```
   - Verifikasi perubahan dengan:
     ```bash
     hostnamectl status
     ```
   - Jelaskan bahwa pengaturan hostname ini membantu dalam identifikasi sistem di jaringan dan digunakan oleh layanan seperti DNS untuk resolusi nama.


5. **Tugas Praktikum**:

   - Dokumentasikan semua perintah yang dipelajari, termasuk:
     1. **Penjelasan**: Tujuan dan fungsi setiap perintah.
     2. **Hasil Eksekusi**: Screenshot atau deskripsi hasil dari setiap perintah.
     3. **Penerapan**: Contoh penerapan perintah dalam situasi nyata, seperti mengelola file konfigurasi jaringan atau memantau koneksi server.
   - Laporan harus mencakup tangkapan layar berikut:
     - Hasil konfigurasi jaringan.
     - Hasil pengujian koneksi menggunakan `ping`.
     - Daftar proses yang berjalan menggunakan `ps aux`.

---

### **Pekan 4: Instalasi dan Konfigurasi BIND (DNS Server)**

DNS Server merupakan layanan penting dalam jaringan yang bertanggung jawab untuk menerjemahkan nama domain menjadi alamat IP. Pada praktikum ini, siswa akan mempelajari langkah-langkah instalasi dan konfigurasi DNS Server menggunakan BIND di CentOS.

Apa itu domain dan nama domain?
-------------------------------
Sebelum kita mempelajari konfigurasi DNS Server, mari kita pahami terlebih dahulu konsep dasar tentang domain dan nama domain.

Domain adalah nama unik yang digunakan untuk mengidentifikasi situs web atau server di internet. Nama domain adalah alamat yang digunakan oleh pengguna untuk mengakses sumber daya di internet, seperti `www.google.com` atau `mail.yahoo.com`. Nama domain terdiri dari dua bagian: nama utama **(top-level domain)** dan nama spesifik **(second-level domain)**. Contoh top-level domain adalah `.com`, `.org`, atau `.net`, sedangkan second-level domain adalah nama unik yang diberikan kepada situs web atau server. Nama domain memungkinkan pengguna untuk mengakses sumber daya dengan mudah tanpa perlu mengingat alamat IP yang rumit. 

![TLD dan SLD](https://iili.io/2i1xiil.md.jpg)

Kenapa DNS Server Penting?
-------------------------
DNS Server memainkan peran kunci dalam jaringan komputer modern. Beberapa alasan mengapa DNS Server penting adalah:
- **Mengurangi Ketergantungan pada IP**: Dengan menggunakan nama domain, pengguna tidak perlu mengingat alamat IP yang panjang dan rumit.
- **Memudahkan Manajemen Jaringan**: DNS Server memungkinkan pengelolaan domain dan subdomain dengan mudah.
- **Meningkatkan Keamanan**: DNS Server dapat digunakan untuk mengarahkan lalu lintas ke server yang aman dan mencegah serangan phishing.
- **Meningkatkan Kinerja**: DNS Server dapat mempercepat proses pengalihan lalu lintas dengan mengoptimalkan resolusi nama.
- **Meningkatkan Fleksibilitas**: DNS Server memungkinkan penggunaan subdomain dan konfigurasi yang kompleks sesuai kebutuhan.
- **Meningkatkan Kualitas Layanan**: DNS Server memungkinkan penyedia layanan untuk menyediakan layanan yang andal dan mudah diakses.

Cara kerja DNS Server:
----------------------
1. **Resolusi Nama**: Ketika pengguna memasukkan nama domain (misalnya `www.google.com`) ke dalam browser, DNS Server bertugas untuk menerjemahkan nama domain tersebut menjadi alamat IP yang sesuai (misalnya `11.12.13.14`).
2. **Zona DNS**: DNS Server menyimpan informasi tentang domain dalam zona DNS, yang berisi catatan tentang nama domain, alamat IP, dan konfigurasi lainnya.
3. **Pertanyaan DNS**: Ketika pengguna meminta akses ke sumber daya dengan nama domain, DNS Server menerima pertanyaan DNS dan mencari informasi yang sesuai dalam zona DNS.
4. **Balasan DNS**: Setelah menemukan informasi yang diperlukan, DNS Server mengirimkan balasan DNS ke pengguna dengan alamat IP yang sesuai.
5. **Penggunaan**: Pengguna dapat mengakses sumber daya dengan menggunakan alamat IP yang diberikan oleh DNS Server.
6. **Pengelolaan**: DNS Server dapat diatur dan dikelola untuk memperbarui informasi zona DNS, menambahkan subdomain, dan mengatur kebijakan akses.
7. **Pengujian**: DNS Server dapat diuji untuk memastikan bahwa informasi yang diberikan sesuai dengan yang diharapkan dan layanan berjalan dengan baik.
8. **Pemeliharaan**: DNS Server perlu dipelihara secara teratur untuk memastikan ketersediaan dan keandalan layanan.
9. **Pengembangan**: DNS Server dapat dikembangkan untuk menambahkan fitur baru, meningkatkan kinerja, dan memperluas fungsionalitas.

Gambar cara kerja DNS Server: 
---------------------------
![DNS Server](https://cf-assets.www.cloudflare.com/slt3lc6tev37/1NzaAqpEFGjqTZPAS02oNv/bf7b3f305d9c35bde5c5b93a519ba6d5/what_is_a_dns_server_dns_lookup.png)

#### **Materi Pembelajaran**  

1. **Langkah 1: Instalasi BIND**  
   - Jalankan perintah berikut untuk menginstal layanan BIND:  
     ```bash
     sudo yum install bind bind-utils -y
     ```  
   - Pastikan paket BIND terinstal dengan memeriksa versinya:  
     ```bash
     named -v
     ```

2. **Langkah 2: Konfigurasi `named.conf`**  
   - File utama untuk konfigurasi BIND adalah `/etc/named.conf`.  
   - Buka file untuk diedit:  
     ```bash
     sudo nano /etc/named.conf
     ```  
   - Sesuaikan pengaturan agar hanya perangkat tertentu dapat mengakses DNS Server:  
     ```bash
     options {
         listen-on port 53 { 127.0.0.1; 192.168.1.0/24; }; // Ubah IP sesuai jaringan
         allow-query     { localhost; 192.168.1.0/24; }; // IP yang diizinkan untuk query
         recursion yes;
     };
     ```  
   - Tambahkan konfigurasi zona untuk domain "moklet-tkj.com":  
     ```bash
     zone "moklet-tkj.com" IN {
         type master;
         file "/var/named/moklet-tkj.com.zone";
         allow-update { none; };
     };
     ```  

3. **Langkah 3: Membuat File Zona DNS**  
   - File zona berisi informasi tentang domain yang dilayani oleh DNS Server.  
   - Buat file zona di direktori `/var/named/`:  
     ```bash
     sudo nano /var/named/moklet-tkj.com.zone
     ```  
   - Isi file dengan konfigurasi berikut:  
     ```bash
     $TTL 86400
     @   IN  SOA     ns1.moklet-tkj.com. admin.moklet-tkj.com. (
                 2025011301 ; Serial
                 3600       ; Refresh
                 1800       ; Retry
                 604800     ; Expire
                 86400 )    ; Minimum TTL
     ;
     @   IN  NS      ns1.moklet-tkj.com.
     ns1 IN  A       192.168.1.1
     www IN  A       192.168.1.2
     ```  

4. **Langkah 4: Menyesuaikan Permissions**  
   - Pastikan file zona memiliki izin yang benar:  
     ```bash
     sudo chown root:named /var/named/moklet-tkj.com.zone
     sudo chmod 640 /var/named/moklet-tkj.com.zone
     ```  

5. **Langkah 5: Menjalankan dan Menguji DNS Server**  
   - Mulai layanan BIND:  
     ```bash
     sudo systemctl start named
     sudo systemctl enable named
     ```  
   - Periksa status layanan:  
     ```bash
     sudo systemctl status named
     ```  
   - Tambahkan aturan firewall untuk DNS:  
     ```bash
     sudo firewall-cmd --permanent --add-port=53/udp
     sudo firewall-cmd --permanent --add-port=53/tcp
     sudo firewall-cmd --reload
     ```  
   - Uji DNS menggunakan perintah berikut:  
     ```bash
     dig @192.168.1.1 www.moklet-tkj.com
     nslookup www.moklet-tkj.com 192.168.1.1
     ```  

#### **Tugas Praktikum**  

1. **Konfigurasi DNS Server**  
   - Konfigurasikan DNS Server menggunakan BIND untuk domain "moklet-tkj.com".  
   - Buat subdomain tambahan seperti `mail.moklet-tkj.com` dan pastikan dapat diakses.  

2. **Pengujian DNS**  
   - Gunakan perintah `dig` dan `nslookup` untuk memastikan DNS Server dapat melayani query.  
   - Dokumentasikan hasil pengujian, termasuk tangkapan layar dari perintah berikut:  
     - `dig @<IP_Server> <domain>`  
     - `nslookup <domain> <IP_Server>`  

3. **Laporan Praktikum**  
   - Buat laporan berisi:  
     - Konfigurasi file `/etc/named.conf` dan file zona.  
     - Hasil pengujian DNS Server.  
     - Penjelasan fungsi DNS Server dalam jaringan dan manfaatnya.  

---

### **Pekan 5: Integrasi DNS dan Web Server**

1. **Langkah 1: Instalasi Web Server**

   - Instal Apache menggunakan perintah berikut:
     ```bash
     sudo yum install httpd -y
     ```

2. **Langkah 2: Konfigurasi Virtual Host**

   - Tambahkan virtual host untuk domain "moklet-tkj.com" di `/etc/httpd/conf.d/moklet-tkj.com.conf` dengan isi konfigurasi berikut:

      ```apache
      <VirtualHost *:80>
         ServerName moklet-tkj.com
         ServerAlias www.moklet-tkj.com
         DocumentRoot /var/www/moklet-tkj.com

         <Directory /var/www/moklet-tkj.com>
            Options Indexes FollowSymLinks
            AllowOverride All
            Require all granted
         </Directory>

         ErrorLog /var/log/httpd/moklet-tkj.com-error.log
         CustomLog /var/log/httpd/moklet-tkj.com-access.log combined
      </VirtualHost>
      ```

      Jangan lupa membuat direktori `/var/www/moklet-tkj.com` dan menambahkan file `index.html` untuk pengujian awal. Restart Apache setelah melakukan konfigurasi.

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

### **Pekan 6: Troubleshooting DNS dan Web Server**

1. **Langkah 1: Analisis Log**

   - Periksa log error DNS di `/var/log/messages` dan log Apache di `/var/log/httpd/error_log`.

2. **Langkah 2: Uji Konektivitas**

   - Gunakan perintah `ping`, `dig`, dan `curl` untuk memeriksa koneksi dan respons server.

3. **Langkah 3: Perbaikan Masalah Umum**

   - Perbaiki kesalahan konfigurasi berdasarkan log dan hasil pengujian.

4. **Tugas Praktikum**:

   - Buat laporan troubleshooting dengan solusi yang diterapkan.

---

## **Studi Kasus Pekan 7-12**

### **Pekan 7: Konfigurasi DNS Server untuk Domain Lokal**

**Deskripsi Kasus**:  
Sebuah perusahaan kecil membutuhkan layanan DNS lokal untuk mengelola domain internal mereka, yaitu `moklet.local`. Siswa diminta mengonfigurasi DNS Server menggunakan BIND. 

**Tugas Siswa**:  
1. Instal layanan BIND di server CentOS.  
2. Konfigurasi file `named.conf` untuk zona `moklet.local`.  
3. Buat file zona untuk domain `moklet.local` dengan entri berikut:
   - `A Record`: `www.moklet.local` mengarah ke IP `192.168.1.10`.  
   - `MX Record`: Menunjukkan mail server `mail.moklet.local` dengan prioritas 10.  
4. Verifikasi DNS menggunakan perintah `dig` dan `nslookup`.  

**Hasil yang Diharapkan**:  
Dokumentasikan proses konfigurasi, file konfigurasi yang digunakan, hasil pengujian, dan tangkapan layar output perintah.  

---

### **Pekan 8: Membangun Web Server dengan Apache**

**Deskripsi Kasus**:  
Sebuah tim pengembang ingin meng-host aplikasi web mereka di server lokal. Siswa diminta untuk mengonfigurasi Web Server Apache pada CentOS.  

**Tugas Siswa**:  
1. Instal layanan Apache (`httpd`) di server.  
2. Konfigurasi file `httpd.conf` untuk:
   - Mengatur direktori dokumen root di `/var/www/html`.  
   - Menambahkan direktori virtual untuk domain `moklet.local`.  
3. Buat halaman web sederhana di `/var/www/html/index.html` yang menampilkan:  
   - Nama siswa.  
   - Pesan “Web Server berhasil dikonfigurasi!”  
4. Pastikan layanan berjalan dan dapat diakses melalui browser di jaringan lokal.  

**Hasil yang Diharapkan**:  
Dokumentasi konfigurasi, file yang diubah, tangkapan layar akses web, dan penjelasan langkah-langkah.  

---

### **Pekan 9: Konfigurasi Firewall dan Keamanan Server**

**Deskripsi Kasus**:  
Administrator jaringan ingin memastikan server hanya dapat diakses melalui layanan yang diizinkan. Siswa diminta untuk mengonfigurasi firewall menggunakan `firewalld`.  

**Tugas Siswa**:  
1. Aktifkan dan konfigurasikan `firewalld` untuk:  
   - Mengizinkan port `80` (HTTP), `443` (HTTPS), dan `53` (DNS).  
   - Menolak akses untuk port lainnya.  
2. Tambahkan aturan untuk mengizinkan akses SSH hanya dari IP tertentu.  
3. Verifikasi aturan firewall menggunakan perintah `firewall-cmd --list-all`.  

**Hasil yang Diharapkan**:  
Tulis laporan berisi langkah konfigurasi, daftar aturan firewall yang diterapkan, dan hasil pengujian akses menggunakan `curl` atau perintah lainnya.  

---

### **Pekan 10: Mengintegrasikan DNS dan Web Server**

**Deskripsi Kasus**:  
Perusahaan membutuhkan integrasi antara DNS Server dan Web Server untuk mempermudah akses aplikasi web mereka melalui nama domain.  

**Tugas Siswa**:  
1. Integrasikan DNS yang sudah dikonfigurasi di Pekan 7 dengan Web Server dari Pekan 8.  
2. Pastikan domain `www.moklet.local` dapat diakses melalui browser dengan mengarahkan ke IP server yang benar.  
3. Tambahkan subdomain `admin.moklet.local` yang mengarah ke direktori `/var/www/admin` dan buat halaman `admin.html`.  

**Hasil yang Diharapkan**:  
Laporan berisi file konfigurasi DNS dan Apache yang diubah, tangkapan layar pengujian akses domain dan subdomain.  

---

### **Pekan 11: Troubleshooting Server**

**Deskripsi Kasus**:  
Sebuah perusahaan mengalami masalah di server mereka. Aplikasi web tidak dapat diakses, dan DNS tampaknya tidak berfungsi. Siswa diminta untuk menganalisis dan memperbaiki masalah.  

**Tugas Siswa**:  
1. Identifikasi penyebab masalah pada:  
   - Layanan DNS (periksa file zona dan status layanan).  
   - Layanan Web Server (periksa file log Apache).  
2. Perbaiki kesalahan konfigurasi yang ditemukan, seperti:  
   - Kesalahan dalam file zona DNS.  
   - Konfigurasi yang salah pada `httpd.conf`.  
3. Dokumentasikan langkah troubleshooting dan perbaikan.  

**Hasil yang Diharapkan**:  
Laporan troubleshooting berisi:  
- Masalah yang ditemukan.  
- Langkah perbaikan.  
- Hasil pengujian setelah perbaikan dilakukan.  

---

### **Pekan 12: Proyek Akhir**

**Deskripsi Kasus**:  
Siswa diminta untuk menyelesaikan proyek akhir yang mengintegrasikan layanan jaringan dan server. Skenarionya adalah:  
- Perusahaan memerlukan server yang menyediakan layanan DNS dan Web Server untuk domain `moklet-project.local`.  
- Web Server harus memiliki dua subdomain:  
  - `www.moklet-project.local` mengarah ke direktori `/var/www/html`.  
  - `api.moklet-project.local` mengarah ke direktori `/var/www/api`.  

**Tugas Siswa**:  
1. Konfigurasi DNS Server untuk domain `moklet-project.local` beserta subdomainnya.  
2. Instal dan konfigurasi Web Server untuk mendukung subdomain.  
3. Terapkan aturan firewall untuk mengizinkan hanya layanan DNS dan HTTP/HTTPS.  
4. Buat halaman web untuk masing-masing subdomain yang menunjukkan:  
   - Nama siswa.  
   - Deskripsi layanan di subdomain tersebut.  

**Hasil yang Diharapkan**:  
- Dokumentasi lengkap dari konfigurasi hingga pengujian.  
- File konfigurasi DNS dan Apache yang digunakan.  
- Tangkapan layar akses domain dan subdomain melalui browser.  
- Laporan dalam format PDF.  
