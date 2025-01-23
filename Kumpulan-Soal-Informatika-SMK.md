### **BK (Berpikir Komputasi)**
**1. Sebuah perusahaan ingin menentukan pola pelanggan berdasarkan data penjualan harian selama 6 bulan terakhir. Data memiliki ribuan baris. Strategi algoritmik mana yang paling sesuai digunakan untuk menyelesaikan masalah ini?**  
a. Linear Search  
b. Divide and Conquer  
c. Sorting and Filtering  
d. Exhaustive Search  
e. Dynamic Programming  

**Kunci Jawaban:** c. Sorting and Filtering  
**Pembahasan:** Sorting dan filtering adalah strategi optimal untuk menganalisis data dengan volume besar. Teknik ini membantu menyusun data sehingga pola dapat diidentifikasi dengan lebih mudah. Divide and Conquer lebih cocok untuk masalah rekursif, sedangkan Dynamic Programming lebih sesuai untuk masalah dengan submasalah yang berulang.

---

**2. Dalam algoritma komputasi, bagaimana cara menentukan jalur terpendek antara dua titik pada peta dengan menggunakan konsep graf?**  
a. Menggunakan algoritma DFS  
b. Menggunakan algoritma BFS  
c. Menggunakan algoritma Dijkstra  
d. Menggunakan algoritma Sorting  
e. Menggunakan Brute Force  

**Kunci Jawaban:** c. Menggunakan algoritma Dijkstra  
**Pembahasan:** Algoritma Dijkstra dirancang khusus untuk menemukan jalur terpendek dalam graf berbobot. DFS dan BFS hanya mencakup pencarian tanpa memperhitungkan bobot. Sorting tidak relevan dalam konteks jalur graf.

---

**3. Diberikan array berikut: `[12, 7, 9, 15, 3]`. Bagaimana urutan array ini setelah diurutkan secara descending menggunakan algoritma sorting bubble?**  
a. `[3, 7, 9, 12, 15]`  
b. `[15, 12, 9, 7, 3]`  
c. `[7, 12, 3, 15, 9]`  
d. `[15, 9, 12, 7, 3]`  
e. `[3, 15, 12, 9, 7]`

**Kunci Jawaban:** b. `[15, 12, 9, 7, 3]`  
**Pembahasan:** Bubble sort mengurutkan dengan membandingkan elemen berdekatan. Karena urutan descending, elemen terbesar di "gelembungkan" ke posisi akhir, sehingga menghasilkan urutan `[15, 12, 9, 7, 3]`.

---

**4. Anda diminta membuat algoritma untuk menentukan apakah sebuah angka adalah bilangan prima. Pendekatan mana yang paling efisien untuk data besar?**  
a. Memeriksa semua angka dari 1 hingga N  
b. Memeriksa hanya angka dari 2 hingga N  
c. Menggunakan metode Sieve of Eratosthenes  
d. Menggunakan pendekatan rekursif  
e. Menggunakan algoritma brute force  

**Kunci Jawaban:** c. Menggunakan metode Sieve of Eratosthenes  
**Pembahasan:** Sieve of Eratosthenes adalah metode yang sangat efisien untuk menemukan bilangan prima dalam rentang besar karena mampu menghilangkan bilangan non-prima secara sistematis. Metode brute force terlalu lambat untuk skala besar.

---

**5. Dalam proses debug algoritma, Anda menemukan bahwa kode berikut menghasilkan output yang salah. Identifikasi penyebabnya.**  

```python
def hitung_pangkat(basis, pangkat):
    hasil = 1
    for i in range(pangkat):
        hasil += basis
    return hasil
```

Bagaimana memperbaiki fungsi ini?  
a. Mengganti `hasil += basis` dengan `hasil *= basis`  
b. Menambah kondisi base case  
c. Menggunakan pendekatan rekursif  
d. Mengganti loop menjadi `while`  
e. Tidak perlu perubahan  

**Kunci Jawaban:** a. Mengganti `hasil += basis` dengan `hasil *= basis`  
**Pembahasan:** Kesalahan terdapat pada baris `hasil += basis`, yang menambah nilai basis alih-alih mengalikan. Operasi pangkat membutuhkan perkalian berulang, sehingga perubahan ke `hasil *= basis` memperbaiki logika.

---

### **TIK (Teknologi Informasi dan Komunikasi)**  
**6. Anda diminta membuat laporan pemasaran menggunakan aplikasi pengolah kata, angka, dan presentasi. Langkah optimal untuk memastikan laporan ini terintegrasi dengan data real-time adalah:**  
a. Menyalin data secara manual dari spreadsheet ke dokumen presentasi.  
b. Menggunakan fitur merge di aplikasi pengolah kata.  
c. Menghubungkan data spreadsheet ke presentasi menggunakan link dinamis.  
d. Membuat diagram di aplikasi pengolah angka dan mengimpor gambarnya.  
e. Mengetik ulang semua data di setiap aplikasi.  

**Kunci Jawaban:** c. Menghubungkan data spreadsheet ke presentasi menggunakan link dinamis  
**Pembahasan:** Link dinamis memungkinkan data diperbarui secara otomatis di presentasi saat terjadi perubahan pada spreadsheet. Metode ini lebih efisien dibandingkan pengolahan manual.

---

**7. Dalam aplikasi pengolah angka, Anda ingin menghitung total keuntungan bulanan dari tabel yang memiliki ratusan baris data. Fungsi apa yang paling tepat digunakan?**  
a. COUNT  
b. AVERAGE  
c. SUM  
d. VLOOKUP  
e. IF  

**Kunci Jawaban:** c. SUM  
**Pembahasan:** Fungsi `SUM` dirancang untuk menjumlahkan semua nilai dalam rentang tertentu. COUNT hanya menghitung jumlah data, sementara fungsi lain seperti VLOOKUP dan IF memiliki kegunaan berbeda.

---

**8. Anda sedang membuat template dokumen di aplikasi pengolah kata. Fitur apa yang dapat digunakan untuk memastikan format dokumen seragam di seluruh halaman?**  
a. Menggunakan tabel manual.  
b. Memanfaatkan fitur style/template bawaan.  
c. Menyalin format dari dokumen lain.  
d. Membuat teks secara manual di setiap halaman.  
e. Menggunakan screenshot sebagai header.  

**Kunci Jawaban:** b. Memanfaatkan fitur style/template bawaan  
**Pembahasan:** Fitur template memastikan format dokumen seragam tanpa perlu pengaturan manual di setiap halaman, meningkatkan konsistensi dan efisiensi kerja.

---

### **SK (Sistem Komputer)**  
**9. Ketika komputer tidak dapat membaca perangkat USB yang terhubung, langkah pertama yang paling efektif untuk mengidentifikasi masalah adalah:**  
a. Menginstal ulang sistem operasi.  
b. Memeriksa pengaturan BIOS.  
c. Mengecek driver perangkat di Device Manager.  
d. Mengganti kabel USB.  
e. Melakukan reset pabrik.  

**Kunci Jawaban:** c. Mengecek driver perangkat di Device Manager  
**Pembahasan:** Masalah perangkat USB yang tidak terbaca seringkali terkait dengan driver. Device Manager memungkinkan pengguna untuk memeriksa, menginstal, atau memperbarui driver perangkat.

---

**10. Apa fungsi utama dari kernel dalam sistem operasi?**  
a. Menyediakan antarmuka pengguna grafis.  
b. Mengelola sumber daya perangkat keras.  
c. Menghubungkan aplikasi dengan internet.  
d. Menyimpan data di cloud.  
e. Menjalankan aplikasi langsung tanpa sistem operasi.  

**Kunci Jawaban:** b. Mengelola sumber daya perangkat keras  
**Pembahasan:** Kernel adalah inti dari sistem operasi yang bertugas mengelola sumber daya perangkat keras seperti CPU, memori, dan perangkat input/output, serta menyediakan layanan untuk aplikasi.

---

**11. Sebuah sistem operasi memerlukan mekanisme untuk menjalankan beberapa proses secara bersamaan. Istilah yang tepat untuk teknik ini adalah:**  
a. Multi-threading  
b. Multi-user  
c. Virtualisasi  
d. Virtual Memory  
e. File Sharing  

**Kunci Jawaban:** a. Multi-threading  
**Pembahasan:** Multi-threading memungkinkan sistem menjalankan beberapa utas eksekusi secara bersamaan dalam satu proses, meningkatkan efisiensi dan performa aplikasi.

---

### **JKI (Jaringan Komputer dan Internet)**  
**12. Anda ingin mengamankan data yang dikirimkan melalui jaringan Wi-Fi publik. Teknik keamanan apa yang paling efektif digunakan?**  
a. Menggunakan protokol HTTP  
b. Menggunakan jaringan VPN  
c. Menonaktifkan firewall  
d. Menghubungkan perangkat langsung tanpa kata sandi  
e. Membagikan data melalui email tanpa enkripsi  

**Kunci Jawaban:** b. Menggunakan jaringan VPN  
**Pembahasan:** VPN (Virtual Private Network) mengenkripsi data yang dikirimkan, membuatnya lebih aman bahkan saat menggunakan jaringan Wi-Fi publik yang rentan terhadap serangan.  

---

**13. Sebuah perangkat memiliki IP address 192.168.1.10 dengan subnet mask 255.255.255.0. Berapa banyak perangkat maksimum yang dapat terhubung dalam jaringan yang sama?**  
a. 254  
b. 255  
c. 256  
d. 128  
e. 64  

**Kunci Jawaban:** a. 254  
**Pembahasan:** Dengan subnet mask 255.255.255.0, ada 8 bit host yang tersedia. Jumlah perangkat maksimum dalam subnet ini adalah \(2^8 - 2 = 254\) (mengurangi satu untuk network address dan satu untuk broadcast).

---

### **AD (Analisis Data)**  
**14.** Dalam analisis data, langkah pertama untuk memastikan data siap diolah adalah:  
a. Menghapus data kosong  
b. Membersihkan data dari duplikasi  
c. Melakukan visualisasi data  
d. Normalisasi data  
e. Menentukan tujuan analisis  

**Kunci Jawaban:** e. Menentukan tujuan analisis  
**Pembahasan:** Menentukan tujuan analisis memastikan seluruh langkah selanjutnya terarah, termasuk pembersihan, normalisasi, dan visualisasi data.

---

### **AP (Algoritma dan Pemrograman)**  
**15.** Apa output dari program berikut?  
```python
def faktorial(n):
    if n == 0:
        return 1
    return n * faktorial(n-1)

print(faktorial(5))
```  
a. 120  
b. 24  
c. 60  
d. 15  
e. 6  

**Kunci Jawaban:** a. 120  
**Pembahasan:** Program menghitung faktorial menggunakan rekursi. Faktorial 5 adalah \(5 \times 4 \times 3 \times 2 \times 1 = 120\).

---

### **DSI (Dampak Sosial Informatika)**  
**16.** Apa dampak negatif utama dari penggunaan algoritma AI yang bias?  
a. Menghemat waktu analisis  
b. Meningkatkan efisiensi bisnis  
c. Diskriminasi terhadap kelompok tertentu  
d. Memperlambat proses pengambilan keputusan  
e. Meningkatkan kualitas produk  

**Kunci Jawaban:** c. Diskriminasi terhadap kelompok tertentu  

---

### **PLB (Projek Literasi Berbasis Informatika)**  
**17.** Dalam sebuah projek berbasis informatika, apa langkah pertama yang harus dilakukan oleh tim?  
a. Membagi tugas ke setiap anggota tim  
b. Menentukan ide atau masalah yang akan diselesaikan  
c. Mencari aplikasi untuk implementasi  
d. Membuat laporan akhir  
e. Menyiapkan presentasi  

**Kunci Jawaban:** b. Menentukan ide atau masalah yang akan diselesaikan  

---

### **AD (Analisis Data)**  
**18.** Apa tujuan utama normalisasi dalam pengolahan data?  
a. Menghilangkan data redundan  
b. Meningkatkan kecepatan pengolahan data  
c. Menyesuaikan data ke format standar  
d. Membuat data lebih mudah divisualisasikan  
e. Meningkatkan akurasi algoritma  

**Kunci Jawaban:** a. Menghilangkan data redundan  
**Pembahasan:** Normalisasi bertujuan menghilangkan redundansi dan memastikan data tidak memiliki duplikasi, sehingga lebih efisien untuk pengolahan.

---

**19.** Dataset Anda berisi nilai dari 1 hingga 1000. Untuk menyoroti pola tertentu, Anda memilih menggunakan histogram. Apa alasan utama penggunaan histogram dalam visualisasi ini?  
a. Menampilkan distribusi data  
b. Membandingkan kategori  
c. Menentukan korelasi antar variabel  
d. Menampilkan data kronologis  
e. Mengukur tren  

**Kunci Jawaban:** a. Menampilkan distribusi data  
**Pembahasan:** Histogram adalah metode visualisasi yang efektif untuk memahami distribusi data dalam suatu rentang nilai.

---

**20.** Anda memiliki dataset besar yang berisi data sensor suhu dari 100 lokasi. Untuk mendeteksi anomali, algoritma apa yang paling sesuai digunakan?  
a. K-Means Clustering  
b. Linear Regression  
c. Decision Tree  
d. Anomaly Detection  
e. Random Forest  

**Kunci Jawaban:** d. Anomaly Detection  
**Pembahasan:** Algoritma deteksi anomali dirancang untuk mengidentifikasi data yang berbeda signifikan dari pola umum.

---

### **AP (Algoritma dan Pemrograman)**  
**21.** Apa output dari kode Python berikut?  
```python
for i in range(1, 6):
    if i % 2 == 0:
        continue
    print(i, end=" ")
```  
a. 1 2 3 4 5  
b. 2 4  
c. 1 3 5  
d. 1 3  
e. Tidak ada output  

**Kunci Jawaban:** c. 1 3 5  
**Pembahasan:** Perintah `continue` melewati iterasi saat kondisi `i % 2 == 0` terpenuhi, sehingga hanya angka ganjil yang dicetak.

---

**22.** Apa keluaran dari program berikut?  
```python
x = [2, 4, 6, 8]
print(sum(x[:2]) + len(x))
```  
a. 12  
b. 10  
c. 16  
d. 20  
e. 18  

**Kunci Jawaban:** c. 16  
**Pembahasan:** `x[:2]` mengambil dua elemen pertama `[2, 4]`, sehingga `sum([2, 4])` menghasilkan 6. Panjang `x` adalah 4. Maka, outputnya adalah \(6 + 4 = 16\).

---

**23.** Sebuah fungsi menerima parameter berupa daftar angka, dan Anda diminta untuk menulis kode Python untuk mengembalikan nilai maksimum dalam daftar tersebut. Pilih kode yang benar:  
a. `return list.sort()[-1]`  
b. `return max(list)`  
c. `return list[-1]`  
d. `return sum(list)`  
e. `return len(list)`  

**Kunci Jawaban:** b. `return max(list)`  
**Pembahasan:** Fungsi bawaan `max()` adalah cara paling langsung untuk mendapatkan nilai maksimum dari sebuah daftar.

---

### **DSI (Dampak Sosial Informatika)**  
**24.** Bagaimana cara menghindari pelanggaran hak cipta saat menggunakan konten digital dalam projek informatika?  
a. Mengunduh konten secara bebas dari internet  
b. Menambahkan nama pembuat dalam projek tanpa izin  
c. Menggunakan konten dengan lisensi Creative Commons yang sesuai  
d. Membeli perangkat lunak tanpa lisensi resmi  
e. Membagikan ulang konten tanpa perubahan  

**Kunci Jawaban:** c. Menggunakan konten dengan lisensi Creative Commons yang sesuai  
**Pembahasan:** Lisensi Creative Commons memungkinkan penggunaan konten dengan batasan tertentu, membantu menghindari pelanggaran hak cipta.

---

**25.** Apa dampak utama penyebaran informasi hoaks melalui media sosial?  
a. Meningkatkan kredibilitas pengguna  
b. Mengurangi polarisasi masyarakat  
c. Membantu masyarakat memahami informasi  
d. Memicu disinformasi dan konflik sosial  
e. Meningkatkan literasi digital  

**Kunci Jawaban:** d. Memicu disinformasi dan konflik sosial  

---

### **PLB (Projek Literasi Berbasis Informatika)**  
**26.** Dalam projek berbasis informatika, tim Anda mengidentifikasi bahwa aplikasi yang dikembangkan sulit digunakan oleh pengguna. Apa langkah pertama untuk mengatasi masalah ini?  
a. Melakukan riset kebutuhan pengguna (user research)  
b. Menambahkan lebih banyak fitur  
c. Mengurangi ukuran file aplikasi  
d. Meningkatkan keamanan aplikasi  
e. Mempublikasikan aplikasi ke lebih banyak platform  

**Kunci Jawaban:** a. Melakukan riset kebutuhan pengguna (user research)  
**Pembahasan:** User research membantu memahami kebutuhan dan preferensi pengguna untuk meningkatkan kegunaan aplikasi.

---

**27.** Anda sedang mengembangkan aplikasi untuk mempermudah pembayaran parkir di daerah perkotaan. Data apa yang harus diprioritaskan dalam tahap perancangan?  
a. Informasi pemilik kendaraan  
b. Lokasi parkir dan tarif  
c. Informasi kontak pemilik parkir  
d. Data pribadi pengemudi  
e. Riwayat perjalanan pengguna  

**Kunci Jawaban:** b. Lokasi parkir dan tarif  
**Pembahasan:** Informasi lokasi dan tarif adalah inti dari fitur aplikasi, memastikan kemudahan dan efisiensi bagi pengguna.

---

### **TIK (Teknologi Informasi dan Komunikasi)**  
**28.** Dalam sebuah aplikasi pengolah angka, Anda ingin secara otomatis menghitung total penjualan berdasarkan kategori produk tertentu. Fungsi apa yang paling tepat digunakan?  
a. SUM  
b. IF  
c. VLOOKUP  
d. SUMIF  
e. AVERAGE  

**Kunci Jawaban:** d. SUMIF  
**Pembahasan:** Fungsi `SUMIF` dirancang untuk menjumlahkan nilai berdasarkan kriteria tertentu, seperti kategori produk tertentu.

---

**29.** Anda ingin mengonversi dokumen PDF menjadi format Word agar dapat diedit. Aplikasi atau metode apa yang paling efisien digunakan?  
a. Mengetik ulang dokumen secara manual  
b. Menggunakan alat konversi online terpercaya  
c. Menggunakan tangkapan layar dan OCR  
d. Menyalin teks dan menempelkannya ke Word  
e. Menggunakan fitur cetak ulang di Word  

**Kunci Jawaban:** b. Menggunakan alat konversi online terpercaya  
**Pembahasan:** Alat konversi online terpercaya dapat mengonversi dokumen PDF ke Word dengan format yang tetap terjaga.

---

**30.** Anda diminta untuk mempresentasikan data secara interaktif kepada klien. Fitur aplikasi apa yang dapat membantu memberikan pengalaman presentasi yang interaktif?  
a. Grafik statis  
b. Hyperlink antar slide  
c. Gambar dekoratif  
d. Video tanpa teks pendukung  
e. Slide dengan hanya teks  

**Kunci Jawaban:** b. Hyperlink antar slide  
**Pembahasan:** Hyperlink antar slide memungkinkan presentasi lebih interaktif, memudahkan navigasi sesuai kebutuhan audiens.

---

### **SK (Sistem Komputer)**  
**31.** Sebuah komputer tidak dapat melakukan booting. Apa langkah pertama yang harus dilakukan untuk mengidentifikasi masalah?  
a. Mengganti sistem operasi  
b. Mengecek kabel daya dan koneksi perangkat keras  
c. Membongkar perangkat keras  
d. Menghapus data di hard drive  
e. Menginstal ulang aplikasi  

**Kunci Jawaban:** b. Mengecek kabel daya dan koneksi perangkat keras  
**Pembahasan:** Masalah fisik seperti kabel yang tidak terhubung adalah langkah pertama yang harus diperiksa sebelum melanjutkan ke diagnostik yang lebih kompleks.

---

**32.** Apa fungsi utama dari BIOS (Basic Input/Output System) dalam komputer?  
a. Mengatur sistem file  
b. Mengelola koneksi internet  
c. Menginisialisasi perangkat keras saat booting  
d. Menyimpan data sementara  
e. Menjalankan aplikasi  

**Kunci Jawaban:** c. Menginisialisasi perangkat keras saat booting  
**Pembahasan:** BIOS bertugas memeriksa perangkat keras komputer dan memastikan sistem siap untuk memuat sistem operasi.

---

### **JKI (Jaringan Komputer dan Internet)**  
**33.** Perangkat Anda terhubung ke jaringan lokal dengan alamat IP 192.168.0.5/24. Berapa alamat IP broadcast untuk jaringan tersebut?  
a. 192.168.0.0  
b. 192.168.0.1  
c. 192.168.0.255  
d. 192.168.1.0  
e. 192.168.255.255  

**Kunci Jawaban:** c. 192.168.0.255  
**Pembahasan:** Dengan subnet mask /24, alamat IP broadcast adalah alamat terakhir dalam jaringan, yaitu 192.168.0.255.

---

**34.** Apa perbedaan utama antara HTTP dan HTTPS dalam komunikasi jaringan?  
a. HTTPS hanya digunakan untuk email  
b. HTTP lebih cepat dari HTTPS  
c. HTTPS menggunakan enkripsi untuk keamanan data  
d. HTTP tidak membutuhkan browser  
e. HTTPS hanya digunakan untuk jaringan lokal  

**Kunci Jawaban:** c. HTTPS menggunakan enkripsi untuk keamanan data  
**Pembahasan:** HTTPS (Hypertext Transfer Protocol Secure) mengenkripsi data menggunakan SSL/TLS untuk melindungi komunikasi.

---

### **DSI (Dampak Sosial Informatika)**  
**35.** Anda menemukan bahwa aplikasi media sosial Anda menggunakan data pribadi Anda untuk iklan tanpa persetujuan. Apa langkah hukum yang dapat diambil?  
a. Melaporkan ke lembaga perlindungan data  
b. Menghapus aplikasi tanpa tindakan lain  
c. Mengubah pengaturan privasi  
d. Membeli versi premium aplikasi  
e. Membagikan pengalaman di media sosial  

**Kunci Jawaban:** a. Melaporkan ke lembaga perlindungan data  
**Pembahasan:** Melaporkan ke lembaga perlindungan data adalah langkah hukum yang tepat sesuai dengan regulasi privasi seperti GDPR atau UU Perlindungan Data Pribadi.

---

**36.** Bagaimana informatika dapat membantu meningkatkan kesadaran lingkungan?  
a. Meningkatkan konsumsi listrik melalui perangkat keras  
b. Membuat simulasi pemanasan global  
c. Menyebarkan informasi melalui media sosial  
d. Mengembangkan aplikasi pendukung keberlanjutan  
e. Semua jawaban benar  

**Kunci Jawaban:** e. Semua jawaban benar  
**Pembahasan:** Semua opsi memberikan kontribusi pada peningkatan kesadaran lingkungan melalui teknologi informatika.

---

### **PLB (Projek Literasi Berbasis Informatika)**  
**37.** Dalam tahap akhir projek informatika, apa langkah terakhir yang perlu dilakukan sebelum publikasi?  
a. Menguji ulang hasil projek  
b. Membuat desain logo  
c. Menambah fitur baru  
d. Menulis dokumentasi teknis  
e. Menghapus data sementara  

**Kunci Jawaban:** a. Menguji ulang hasil projek  
**Pembahasan:** Pengujian ulang memastikan produk akhir bebas dari kesalahan sebelum dirilis ke pengguna.

---

**38.** Dalam projek berbasis algoritma, bagaimana cara terbaik untuk memastikan solusi yang dikembangkan relevan dengan masalah pengguna?  
a. Melibatkan pengguna dalam tahap desain  
b. Membuat algoritma tanpa masukan pengguna  
c. Menambahkan teknologi terbaru  
d. Membuat laporan akhir projek  
e. Membagikan prototype langsung  

**Kunci Jawaban:** a. Melibatkan pengguna dalam tahap desain  
**Pembahasan:** Melibatkan pengguna membantu mengidentifikasi kebutuhan spesifik yang harus dipenuhi oleh solusi.

---

### **AD (Analisis Data)**  
**39.** Anda memiliki dataset besar dengan ratusan ribu baris data. Apa metode terbaik untuk membersihkan data yang memiliki nilai yang hilang (missing values)?  
a. Menghapus semua baris dengan nilai yang hilang  
b. Mengisi nilai yang hilang dengan rata-rata kolom terkait  
c. Mengabaikan data yang hilang  
d. Mengganti nilai yang hilang dengan nilai maksimum  
e. Mengisi data dengan nilai sembarang  

**Kunci Jawaban:** b. Mengisi nilai yang hilang dengan rata-rata kolom terkait  
**Pembahasan:** Mengisi nilai yang hilang dengan rata-rata kolom adalah metode umum untuk menjaga konsistensi data tanpa kehilangan terlalu banyak informasi.

---

**40.** Apa hasil dari langkah berikut dalam siklus pengolahan data?  
1. Pengumpulan data  
2. Pemrosesan data  
3. Visualisasi data  

a. Data terstruktur yang dapat digunakan  
b. Grafik atau diagram untuk analisis lebih lanjut  
c. Laporan hasil pengumpulan data  
d. Analisis deskriptif  
e. Data mentah  

**Kunci Jawaban:** b. Grafik atau diagram untuk analisis lebih lanjut  
**Pembahasan:** Visualisasi data menghasilkan representasi grafik atau diagram untuk membantu analisis data secara lebih mudah dan intuitif.

---

### **AP (Algoritma dan Pemrograman)**  
**41.** Apa output dari kode Python berikut?  
```python
def find_factorial(n):
    if n == 0:
        return 1
    else:
        return n * find_factorial(n-1)

print(find_factorial(4))
```  
a. 10  
b. 16  
c. 20  
d. 24  
e. 120  

**Kunci Jawaban:** d. 24  
**Pembahasan:** Fungsi ini menghitung faktorial menggunakan rekursi. Faktorial dari 4 adalah \(4 \times 3 \times 2 \times 1 = 24\).

---

**42.** Apa hasil dari kode Python berikut?  
```python
list1 = [2, 4, 6, 8]
list2 = [1, 3, 5, 7]
result = [x + y for x, y in zip(list1, list2)]
print(result)
```  
a. [3, 7, 11, 15]  
b. [2, 4, 6, 8, 1, 3, 5, 7]  
c. [3, 5, 7, 9]  
d. [2, 3, 5, 8, 7]  
e. [3, 5, 9, 15]  

**Kunci Jawaban:** a. [3, 7, 11, 15]  
**Pembahasan:** Fungsi `zip` menggabungkan dua daftar elemen demi elemen, sehingga setiap elemen dari kedua daftar dijumlahkan menghasilkan [3, 7, 11, 15].

---

### **DSI (Dampak Sosial Informatika)**  
**43.** Bagaimana cara meningkatkan literasi digital masyarakat?  
a. Membuat aplikasi pendidikan yang mudah diakses  
b. Memberikan akses internet gratis tanpa regulasi  
c. Meningkatkan pengawasan konten online  
d. Membatasi penggunaan teknologi pada anak-anak  
e. Menghapus semua konten negatif dari internet  

**Kunci Jawaban:** a. Membuat aplikasi pendidikan yang mudah diakses  
**Pembahasan:** Literasi digital dapat ditingkatkan melalui aplikasi pendidikan yang dapat diakses oleh berbagai lapisan masyarakat.

---

**44.** Apa dampak negatif dari ketergantungan terhadap algoritma media sosial dalam penyebaran informasi?  
a. Mempercepat penyebaran informasi  
b. Meningkatkan kecepatan kerja algoritma  
c. Memunculkan bias informasi dan "echo chamber"  
d. Mengurangi biaya distribusi informasi  
e. Mempermudah akses ke berita terkini  

**Kunci Jawaban:** c. Memunculkan bias informasi dan "echo chamber"  
**Pembahasan:** Algoritma media sosial sering memprioritaskan konten yang sesuai dengan preferensi pengguna, sehingga memperkuat pandangan tertentu tanpa memberikan perspektif yang beragam.

---

### **PLB (Projek Literasi Berbasis Informatika)**  
**45.** Anda sedang merancang projek informatika untuk meningkatkan kesadaran tentang hemat energi. Fitur apa yang paling relevan untuk disertakan?  
a. Informasi statistik konsumsi energi  
b. Alat simulasi untuk mengurangi konsumsi energi  
c. Tips hemat energi secara harian  
d. Perhitungan biaya listrik yang lebih efisien  
e. Semua jawaban benar  

**Kunci Jawaban:** e. Semua jawaban benar  
**Pembahasan:** Semua fitur tersebut relevan dalam meningkatkan kesadaran hemat energi melalui aplikasi informatika.

---

**46.** Dalam proses pengembangan projek tim, Anda menemukan bahwa tim tidak sejalan dengan tujuan utama projek. Apa langkah pertama yang harus diambil?  
a. Melanjutkan projek tanpa perubahan  
b. Mengubah tujuan projek agar sesuai dengan hasil tim  
c. Melakukan diskusi tim untuk menyelaraskan visi  
d. Membubarkan tim dan memulai dari awal  
e. Mengabaikan masalah tersebut  

**Kunci Jawaban:** c. Melakukan diskusi tim untuk menyelaraskan visi  
**Pembahasan:** Diskusi tim penting untuk menyatukan pemahaman dan menghindari konflik di kemudian hari.

---

**TIK (Teknologi Informasi dan Komunikasi)**  
**47.** Fitur apa yang memungkinkan kolaborasi real-time dalam dokumen berbasis cloud seperti Google Docs?  
a. Penyimpanan offline  
b. Komentar di dokumen  
c. Edit simultan oleh banyak pengguna  
d. Notifikasi email  
e. Template dokumen  

**Kunci Jawaban:** c. Edit simultan oleh banyak pengguna  
**Pembahasan:** Fitur ini memungkinkan pengguna untuk bekerja bersama secara real-time, meningkatkan produktivitas dan kolaborasi.

---

**48.** Apa manfaat utama penggunaan aplikasi pengelola tugas seperti Trello atau Asana dalam projek informatika?  
a. Menyimpan data secara aman  
b. Memantau kemajuan projek secara terstruktur  
c. Menyelesaikan tugas secara otomatis  
d. Mengurangi kebutuhan komunikasi antar anggota tim  
e. Mengatur pengeluaran projek  

**Kunci Jawaban:** b. Memantau kemajuan projek secara terstruktur  
**Pembahasan:** Aplikasi pengelola tugas mempermudah pengorganisasian pekerjaan dan memastikan setiap tugas selesai sesuai jadwal.

---

### **SK (Sistem Komputer)**  
**49.** Ketika komputer Anda tiba-tiba mati karena overheating, apa solusi terbaik untuk mengatasi masalah tersebut?  
a. Memasang antivirus baru  
b. Membersihkan kipas dan ventilasi pendingin  
c. Menginstal ulang sistem operasi  
d. Menambah RAM  
e. Mengganti kabel daya  

**Kunci Jawaban:** b. Membersihkan kipas dan ventilasi pendingin  
**Pembahasan:** Overheating biasanya disebabkan oleh penumpukan debu atau masalah pada sistem pendingin, sehingga membersihkan kipas dan ventilasi adalah langkah yang tepat.

---

**50.** Apa peran utama dari kernel dalam sistem operasi?  
a. Menyediakan antarmuka pengguna grafis  
b. Mengelola file dalam sistem  
c. Berkomunikasi antara perangkat keras dan perangkat lunak  
d. Menjalankan aplikasi  
e. Mengelola data dalam database  

**Kunci Jawaban:** c. Berkomunikasi antara perangkat keras dan perangkat lunak  
**Pembahasan:** Kernel adalah bagian inti dari sistem operasi yang mengelola komunikasi antara perangkat keras dan perangkat lunak serta mengatur sumber daya sistem.

---

### **AD (Analisis Data)**  
**51.** Anda ingin memvisualisasikan distribusi data dalam bentuk histogram. Apa informasi utama yang dapat diperoleh dari histogram?  
a. Hubungan antara dua variabel  
b. Pola distribusi frekuensi data  
c. Perbandingan nilai dalam kategori tertentu  
d. Rata-rata data  
e. Nilai ekstrim data  

**Kunci Jawaban:** b. Pola distribusi frekuensi data  
**Pembahasan:** Histogram digunakan untuk menunjukkan distribusi data dalam kelompok atau interval tertentu, memberikan gambaran pola frekuensi data.

---

**52.** Dalam analisis data, apa keuntungan menggunakan diagram boxplot?  
a. Menampilkan distribusi data dalam kelompok  
b. Mengidentifikasi outlier dengan mudah  
c. Menunjukkan hubungan antara dua variabel  
d. Membandingkan data dari waktu ke waktu  
e. Memvisualisasikan persentase data  

**Kunci Jawaban:** b. Mengidentifikasi outlier dengan mudah  
**Pembahasan:** Boxplot efektif untuk mengidentifikasi outlier, karena menampilkan batas atas dan bawah serta distribusi data.

---

### **JKI (Jaringan Komputer dan Internet)**  
**53.** Apa langkah paling aman untuk melindungi data saat menggunakan jaringan Wi-Fi publik?  
a. Menggunakan koneksi HTTPS saja  
b. Mengaktifkan mode pesawat pada perangkat  
c. Menggunakan Virtual Private Network (VPN)  
d. Menonaktifkan firewall  
e. Menghapus cache browser  

**Kunci Jawaban:** c. Menggunakan Virtual Private Network (VPN)  
**Pembahasan:** VPN mengenkripsi lalu lintas internet Anda, melindungi data dari potensi ancaman saat menggunakan Wi-Fi publik.

---

**54.** Perangkat Anda terhubung ke internet melalui router yang menggunakan protokol DHCP. Apa tugas utama dari DHCP?  
a. Mengatur konektivitas jaringan kabel  
b. Mengalokasikan alamat IP secara otomatis  
c. Mengenkripsi data dalam jaringan  
d. Memantau lalu lintas jaringan  
e. Mempercepat koneksi internet  

**Kunci Jawaban:** b. Mengalokasikan alamat IP secara otomatis  
**Pembahasan:** DHCP (Dynamic Host Configuration Protocol) bertugas mengatur alamat IP secara dinamis sehingga perangkat dapat terhubung ke jaringan dengan mudah.

---

### **AP (Algoritma dan Pemrograman)**  
**55.** Apa output dari kode Python berikut?  
```python
def fib(n):
    if n <= 1:
        return n
    else:
        return fib(n-1) + fib(n-2)

print(fib(5))
```  
a. 3  
b. 5  
c. 8  
d. 13  
e. 21  

**Kunci Jawaban:** b. 5  
**Pembahasan:** Fungsi ini menggunakan rekursi untuk menghitung bilangan Fibonacci ke-5, yaitu \(0, 1, 1, 2, 3, 5\). Hasilnya adalah 5.

---

**56.** Apa output dari kode Python berikut?  
```python
x = [1, 2, 3, 4]
y = [5, 6, 7, 8]
result = list(map(lambda a, b: a * b, x, y))
print(result)
```  
a. [5, 12, 21, 32]  
b. [6, 8, 10, 12]  
c. [4, 6, 8, 10]  
d. [1, 2, 3, 4, 5, 6, 7, 8]  
e. [5, 12, 15, 20]  

**Kunci Jawaban:** a. [5, 12, 21, 32]  
**Pembahasan:** Fungsi `map` menggabungkan elemen dari dua daftar menggunakan operasi perkalian, menghasilkan [5, 12, 21, 32].

---

### **DSI (Dampak Sosial Informatika)**  
**57.** Bagaimana teknologi blockchain dapat mendukung keamanan data?  
a. Dengan menyimpan data dalam satu server pusat  
b. Dengan mengenkripsi data menggunakan kunci pribadi  
c. Dengan menggunakan jaringan terdistribusi yang transparan dan sulit dimanipulasi  
d. Dengan membatasi akses ke data tertentu  
e. Dengan menghapus data secara otomatis setelah waktu tertentu  

**Kunci Jawaban:** c. Dengan menggunakan jaringan terdistribusi yang transparan dan sulit dimanipulasi  
**Pembahasan:** Blockchain menyimpan data dalam bentuk terdistribusi, sehingga sulit untuk diubah tanpa konsensus dari semua node dalam jaringan.

---

**58.** Apa dampak positif dari implementasi IoT (Internet of Things) dalam rumah pintar?  
a. Meningkatkan konsumsi energi  
b. Membatasi akses pengguna  
c. Mengotomatisasi kontrol perangkat untuk efisiensi energi  
d. Mengurangi jumlah perangkat elektronik  
e. Menambah kompleksitas sistem  

**Kunci Jawaban:** c. Mengotomatisasi kontrol perangkat untuk efisiensi energi  
**Pembahasan:** IoT memungkinkan perangkat terhubung untuk mengoptimalkan konsumsi energi dan memberikan kenyamanan tambahan.

---

### **PLB (Projek Literasi Berbasis Informatika)**  
**59.** Apa langkah pertama dalam merancang projek berbasis informatika yang melibatkan masyarakat?  
a. Melakukan survei untuk memahami kebutuhan masyarakat  
b. Menyusun laporan akhir projek  
c. Membuat prototipe projek  
d. Mengidentifikasi masalah tanpa melibatkan masyarakat  
e. Mengembangkan solusi langsung  

**Kunci Jawaban:** a. Melakukan survei untuk memahami kebutuhan masyarakat  
**Pembahasan:** Survei membantu memahami kebutuhan dan masalah yang relevan sehingga projek dapat dirancang sesuai konteks.

---

**60.** Dalam projek berbasis informatika, bagaimana cara memastikan bahwa hasil projek dapat diakses oleh semua kelompok masyarakat?  
a. Menambahkan fitur bahasa lokal  
b. Menyediakan antarmuka sederhana yang inklusif  
c. Mengintegrasikan aplikasi dengan perangkat yang mudah diakses  
d. Menyediakan dokumentasi yang jelas  
e. Semua jawaban benar  

**Kunci Jawaban:** e. Semua jawaban benar  
**Pembahasan:** Semua langkah tersebut membantu memastikan projek informatika dapat diakses dan digunakan oleh semua kelompok masyarakat, termasuk mereka yang memiliki kebutuhan khusus.

---

Berikut adalah tambahan soal untuk memenuhi kisi-kisi **gerbang logika**, **sistem bilangan**, dan **input/output device** beserta kunci jawaban dan pembahasannya:  

---

### **Gerbang Logika**  
**61. Sebuah gerbang logika memiliki dua input A dan B, dan menghasilkan output sebagai berikut:**
| A | B | Output |
|---|---|--------|
| 0 | 0 | 0      |
| 0 | 1 | 1      |
| 1 | 0 | 1      |
| 1 | 1 | 0      |  

Gerbang logika apa yang sesuai dengan tabel kebenaran di atas?  
a. AND  
b. OR  
c. XOR  
d. NAND  
e. XNOR  

**Kunci Jawaban:** c. XOR  
**Pembahasan:** Tabel kebenaran menunjukkan bahwa output hanya bernilai 1 jika **salah satu** input bernilai 1 (bukan keduanya). Hal ini sesuai dengan karakteristik gerbang XOR.  

---

**62. Suatu rangkaian logika memiliki tiga input (A, B, C) dan menghasilkan output \(Y = (A \cdot B)' + C\). Jika \(A = 1\), \(B = 0\), dan \(C = 1\), berapakah nilai \(Y\)?**  
a. 0  
b. 1  
c. Tidak dapat ditentukan  
d. -1  
e. 2  

**Kunci Jawaban:** b. 1  
**Pembahasan:** Langkah penyelesaian:  
1. Hitung \(A \cdot B = 1 \cdot 0 = 0\).  
2. Negasi \( (A \cdot B)' = 1\).  
3. \(Y = 1 + C = 1 + 1 = 1\) (karena dalam logika, 1 + apa pun = 1).  

---

### **Sistem Bilangan**  
**63. Konversikan bilangan biner 1101 ke desimal.**  
a. 11  
b. 12  
c. 13  
d. 14  
e. 15  

**Kunci Jawaban:** c. 13  
**Pembahasan:** Bilangan biner 1101 dikonversi ke desimal:  
\[
(1 \cdot 2^3) + (1 \cdot 2^2) + (0 \cdot 2^1) + (1 \cdot 2^0) = 8 + 4 + 0 + 1 = 13
\]  

---

**64. Konversikan bilangan desimal 45 ke bilangan biner.**  
a. 101101  
b. 101011  
c. 100101  
d. 110101  
e. 111001  

**Kunci Jawaban:** a. 101101  
**Pembahasan:** Gunakan metode pembagian desimal ke biner:  
- 45 ÷ 2 = 22 sisa 1  
- 22 ÷ 2 = 11 sisa 0  
- 11 ÷ 2 = 5 sisa 1  
- 5 ÷ 2 = 2 sisa 1  
- 2 ÷ 2 = 1 sisa 0  
- 1 ÷ 2 = 0 sisa 1  
Biner: baca sisa dari bawah ke atas → 101101.  

---

### **Input/Output Device**  
**65. Perangkat manakah yang termasuk ke dalam kategori perangkat input?**  
a. Monitor  
b. Printer  
c. Keyboard  
d. Speaker  
e. Proyektor  

**Kunci Jawaban:** c. Keyboard  
**Pembahasan:** Keyboard adalah perangkat input yang digunakan untuk memasukkan data atau perintah ke dalam komputer. Perangkat lain seperti monitor, printer, dan speaker adalah perangkat output.  

---

**66. Apa fungsi utama dari perangkat output seperti monitor dan printer?**  
a. Memasukkan data ke komputer  
b. Menyimpan data secara permanen  
c. Menampilkan atau mencetak informasi dari komputer  
d. Memproses data menjadi informasi  
e. Menghubungkan perangkat dengan internet  

**Kunci Jawaban:** c. Menampilkan atau mencetak informasi dari komputer  
**Pembahasan:** Perangkat output seperti monitor digunakan untuk menampilkan informasi, sementara printer mencetak informasi ke dalam media fisik (kertas).  

---

### **Gerbang Logika**  
**67. Jika sebuah gerbang logika memiliki dua input (A dan B) dan menghasilkan output \(Y = A \cdot B + A' \cdot B'\), maka gerbang logika apakah itu?**  
a. AND  
b. OR  
c. XOR  
d. XNOR  
e. NAND  

**Kunci Jawaban:** d. XNOR  
**Pembahasan:** Fungsi \(Y = A \cdot B + A' \cdot B'\) menghasilkan output 1 jika kedua input sama (baik 0 atau 1), sehingga sesuai dengan gerbang XNOR.  

---

**68. Dalam sebuah rangkaian logika, output \(Y = (A + B)'\). Jika \(A = 1\) dan \(B = 0\), berapakah nilai \(Y\)?**  
a. 0  
b. 1  
c. 2  
d. -1  
e. Tidak dapat ditentukan  

**Kunci Jawaban:** a. 0  
**Pembahasan:** Langkah penyelesaian:  
1. \(A + B = 1 + 0 = 1\)  
2. Negasi: \((A + B)' = 0\)  

---

### **Sistem Bilangan**  
**69. Konversikan bilangan heksadesimal A3 ke desimal.**  
a. 161  
b. 162  
c. 163  
d. 164  
e. 165  

**Kunci Jawaban:** c. 163  
**Pembahasan:** Bilangan heksadesimal \(A3 = (A \cdot 16^1) + (3 \cdot 16^0)\):  
\[
(10 \cdot 16) + (3 \cdot 1) = 160 + 3 = 163
\]  

---

**70. Konversikan bilangan desimal 255 ke bilangan heksadesimal.**  
a. FF  
b. FE  
c. FD  
d. EF  
e. EE  

**Kunci Jawaban:** a. FF  
**Pembahasan:** Gunakan metode pembagian desimal ke heksadesimal:  
- 255 ÷ 16 = 15 sisa 15 (F)  
- 15 ÷ 16 = 0 sisa 15 (F)  
Heksadesimal: baca dari bawah ke atas → FF.  

---

### **Input/Output Device**  
**71. Apa fungsi dari perangkat input scanner?**  
a. Memasukkan teks atau gambar ke komputer  
b. Mencetak data ke kertas  
c. Menampilkan informasi pada layar  
d. Menyimpan data ke dalam hard disk  
e. Memproses data menjadi informasi  

**Kunci Jawaban:** a. Memasukkan teks atau gambar ke komputer  
**Pembahasan:** Scanner digunakan untuk memindai teks atau gambar dari dokumen fisik menjadi format digital yang dapat diolah oleh komputer.  

---

**72. Perangkat manakah yang termasuk perangkat output?**  
a. Joystick  
b. Microphone  
c. Webcam  
d. Monitor  
e. Keyboard  

**Kunci Jawaban:** d. Monitor  
**Pembahasan:** Monitor adalah perangkat output yang digunakan untuk menampilkan informasi dari komputer ke layar. Perangkat lainnya adalah perangkat input.  

---

### **Microsoft Office Word, Excel, PowerPoint**  
**73. Anda ingin membuat diagram yang secara otomatis diperbarui dengan perubahan data di Excel. Apa langkah terbaik untuk melakukannya di PowerPoint?**  
a. Mengimpor gambar diagram dari Excel.  
b. Membuat diagram manual di PowerPoint.  
c. Menyalin diagram dari Excel dan menggunakan opsi link.  
d. Mengetik ulang data di PowerPoint.  
e. Menggunakan template diagram bawaan PowerPoint.  

**Kunci Jawaban:** c. Menyalin diagram dari Excel dan menggunakan opsi link.  
**Pembahasan:** Opsi link memungkinkan diagram di PowerPoint diperbarui otomatis saat data di Excel diubah.  

---

**74. Fungsi apa yang dapat digunakan di Excel untuk mencari data tertentu di tabel besar?**  
a. SUM  
b. AVERAGE  
c. VLOOKUP  
d. COUNT  
e. CONCATENATE  

**Kunci Jawaban:** c. VLOOKUP  
**Pembahasan:** VLOOKUP digunakan untuk mencari data berdasarkan nilai tertentu di kolom pertama tabel besar.  

---

### **Python Programming**  
**75. Apa output dari kode Python berikut?**  
```python
numbers = [1, 2, 3, 4, 5]
result = [x**2 for x in numbers if x % 2 == 0]
print(result)
```  
a. [1, 4, 9, 16, 25]  
b. [4, 16]  
c. [2, 4]  
d. [1, 9, 25]  
e. Tidak ada output  

**Kunci Jawaban:** b. [4, 16]  
**Pembahasan:** List comprehension menghasilkan kuadrat dari angka genap dalam daftar. Angka genap adalah 2 dan 4, sehingga hasilnya [4, 16].  

---

**76. Apa keluaran dari kode Python berikut?**  
```python
def factorial(n):
    return 1 if n == 0 else n * factorial(n-1)

print(factorial(3))
```  
a. 6  
b. 9  
c. 3  
d. 12  
e. 0  

**Kunci Jawaban:** a. 6  
**Pembahasan:** Fungsi ini menghitung faktorial dengan rekursi:  
\[
3 \times 2 \times 1 = 6
\]  

---

### **Input/Output Device**  
**77. Perangkat apakah yang menggabungkan fungsi input dan output?**  
a. Monitor  
b. Printer  
c. Touchscreen  
d. Keyboard  
e. Speaker  

**Kunci Jawaban:** c. Touchscreen  
**Pembahasan:** Touchscreen dapat menerima input (dengan sentuhan) dan juga memberikan output (menampilkan informasi).  

---

**78. Apa yang dimaksud dengan perangkat I/O?**  
a. Perangkat yang hanya menerima input.  
b. Perangkat yang hanya memberikan output.  
c. Perangkat yang dapat menerima input dan memberikan output.  
d. Perangkat yang menyimpan data.  
e. Perangkat yang menghubungkan komputer ke internet.  

**Kunci Jawaban:** c. Perangkat yang dapat menerima input dan memberikan output.  
**Pembahasan:** Perangkat I/O (Input/Output) seperti touchscreen, printer multifungsi, dan modem dapat melakukan fungsi input dan output secara bersamaan.  

---

### **Sistem Bilangan**  
**79. Konversikan bilangan biner 10101 ke desimal.**  
a. 19  
b. 20  
c. 21  
d. 22  
e. 23  

**Kunci Jawaban:** c. 21  
**Pembahasan:** Bilangan biner 10101 dikonversi ke desimal:  
\[
(1 \cdot 2^4) + (0 \cdot 2^3) + (1 \cdot 2^2) + (0 \cdot 2^1) + (1 \cdot 2^0) = 16 + 0 + 4 + 0 + 1 = 21
\]  

---

**80. Konversikan bilangan desimal 100 ke bilangan biner.**  
a. 1100100  
b. 1110100  
c. 1010100  
d. 1000100  
e. 1101100  

**Kunci Jawaban:** a. 1100100  
**Pembahasan:** Gunakan metode pembagian desimal ke biner:  
- 100 ÷ 2 = 50 sisa 0  
- 50 ÷ 2 = 25 sisa 0  
- 25 ÷ 2 = 12 sisa 1  
- 12 ÷ 2 = 6 sisa 0  
- 6 ÷ 2 = 3 sisa 0  
- 3 ÷ 2 = 1 sisa 1  
- 1 ÷ 2 = 0 sisa 1  
Biner: baca sisa dari bawah ke atas → 1100100.  

