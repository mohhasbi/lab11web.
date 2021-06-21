# lab11web.

# Nama : Moh. Hasbi Hasbiyah
# NIM : 311910711
# Kelas : TI 19 B2

# Praktikum 12


Sebelum memulai menggunakan Framework Codeigniter, perlu dilakukan konfigurasi pada webserver. Beberapa ekstensi PHP perlu diaktifkan untuk kebutuhan pengembangan Codeigniter 4. Dengan cara di bawah ini : 

![2](https://user-images.githubusercontent.com/81578584/122822528-630e1b00-d308-11eb-8221-aaeba046a73a.png)


Hapus tanda ; (titik koma) pada bagian extension yang akan diaktifkan.

![1](https://user-images.githubusercontent.com/81578584/122822630-83d67080-d308-11eb-91e0-4a193ae47fce.png)


Instalasi CodeIgniter 4 • Codeigniter dapat didownload dari website https://codeigniter.com/download • Extrak file zip Codeigniter ke direktori htdocs/lab11_php_ci • Ubah nama direktory framework-4.x.xx menjadi ci4 • Buka browser dengan alamat http://localhost/lab11_php_ci/ci4/public/

![3](https://user-images.githubusercontent.com/81578584/122822792-c009d100-d308-11eb-8b4b-610557f5c590.png)


Codeigniter menyediakan CLI, untuk mengaksesnya buka terminal lalu arahkan ke direktori project yang akan dibuat. Kemudian jalankan perintah php spark untuk memanggil CLI codeigniter.

![4](https://user-images.githubusercontent.com/81578584/122823080-1e36b400-d309-11eb-9bc9-55c96e58f60c.png)


Codeigniter juga menyediakan mode debugging/development yang dapat menampilkan error/kesalahan dalam kode program. Cara mengaktifkannya dengan mengubah nama file env menjadi .env kemudian buka filenya dan ubah nilai CI_ENVIRONMENT menjadi development.

![122778082-dac35200-d2d6-11eb-8556-7f6e839ae6d3](https://user-images.githubusercontent.com/81578584/122823215-458d8100-d309-11eb-8d54-fcff7d119415.png)


Maka pesan kesalahan akan ditampilkan.

![6](https://user-images.githubusercontent.com/81578584/122823311-63f37c80-d309-11eb-9993-dd87c72e17da.png)


Langkah 1 - Membuat Route • Router terletak pada file app/config/Routes.php • Untuk mengetahui route yg ada atau telah berjalan dapat menggunakan perintah php spark routes

![7](https://user-images.githubusercontent.com/81578584/122823386-7f5e8780-d309-11eb-8473-10d197425c20.png)


• Selanjutnya mencoba akses route yang telah dibuat dengan mengakses http://localhost:8080/contact • Terjadi error file not found dikarenakan tidak ada file/page untuk halaman contact

![8](https://user-images.githubusercontent.com/81578584/122823565-b9c82480-d309-11eb-9ce4-8a67ccf86f82.png)


Langkah 2 - Membuat Controller • Membuat file page.php di dalam direktori Controller (/app/Controllers)

• Kemudian refresh browser maka halaman sudah dapat diakses dan menampilkan hasilnya.

![9](https://user-images.githubusercontent.com/81578584/122823709-e5e3a580-d309-11eb-9468-36e53ac5f4db.png)


• Menambahkan method baru pada controller page. • Method ini dapat diakses dengan menggunakan alamat: http://localhost:8080/page/tos

![10](https://user-images.githubusercontent.com/81578584/122823806-001d8380-d30a-11eb-8b54-eb5991e2644c.png)


Langkah 4 - Membuat Layout Web dengan CSS • Buat file css pada direktori public dengan nama style.css (copy file dari praktikum lab4_layout). • Kemudian buat folder template pada direktori view, lalu buat file header.php dan footer.php. header.php

![11](https://user-images.githubusercontent.com/81578584/122823926-2511f680-d30a-11eb-861b-058752c23bf1.png)

footer.php

![12](https://user-images.githubusercontent.com/81578584/122823991-3bb84d80-d30a-11eb-88b3-58915733e7ef.png)


• Kemudian ubah file about.php (/app/view/about.php) seperti berikut.

![13](https://user-images.githubusercontent.com/81578584/122824059-538fd180-d30a-11eb-906c-b9d916b149e0.png)


Pertanyaan dan Tugas Lengkapi kode program untuk menu lainnya yang ada pada Controller Page, sehingga semua link pada navigasi header dapat menampilkan tampilan dengan layout yang sama.

Hasil tugas • Tampilan page about

![14](https://user-images.githubusercontent.com/81578584/122824138-71f5cd00-d30a-11eb-9f70-80a6edaeb638.png)


• Tampilan page artikel

![15](https://user-images.githubusercontent.com/81578584/122824193-88038d80-d30a-11eb-82fb-9995197d93ea.png)


• Tampilan page kontak

![16](https://user-images.githubusercontent.com/81578584/122824251-9e114e00-d30a-11eb-8c62-ac6cb0222295.png)


Praktikum 12 Jalankan MySQL dan buat sebuah database sebagai berikut:

![17](https://user-images.githubusercontent.com/81578584/122824347-b7b29580-d30a-11eb-8af1-b87593fcb6b3.png)


1 - Konfigurasi Database Membuat konfigurasi hubungan ke database server dengan menggunakan file .env

![19](https://user-images.githubusercontent.com/81578584/122824646-25f75800-d30b-11eb-9765-142a7e9b4767.png)


Lalu buka alamat http://localhost:8080/artikel untuk melihat hasilnya

![20](https://user-images.githubusercontent.com/81578584/122825631-65727400-d30c-11eb-916c-b0d5910c8e00.png)


Tidak ada data yang ditampilkan karena database masih kosong. Tambahkan data pada database untuk ditampilkan datanya pada phpmyadmin

![gambar](https://user-images.githubusercontent.com/81578584/122825693-79b67100-d30c-11eb-92e0-fc66247a9226.png)
Maka akan muncul tampilan seperti ini ketika browser direfresh.











