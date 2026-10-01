<h2>Penjelasan DOM dengan Kasus Perpustakaan</h2>
<h3>1. querySelector dan querySelectorAll</h3>

querySelector adalah metode DOM yang digunakan untuk memilih satu elemen HTML pertama yang sesuai dengan selector tertentu, seperti id, class, atau nama tag.

querySelectorAll digunakan untuk memilih semua elemen HTML yang sesuai dengan selector tertentu.

Contoh pada perpustakaan:
querySelector dapat digunakan untuk memilih judul halaman perpustakaan, sedangkan querySelectorAll dapat digunakan untuk memilih seluruh daftar buku.

<h3>2. innerHTML, textContent, dan innerText</h3>

Ketiga metode ini digunakan untuk mengakses atau mengubah isi dari sebuah elemen HTML.

innerHTML → digunakan untuk mengubah isi elemen sekaligus dapat memasukkan tag HTML.
textContent → digunakan untuk mengubah atau mengambil seluruh teks yang terdapat di dalam elemen.
innerText → digunakan untuk mengubah atau mengambil teks yang terlihat oleh pengguna pada halaman.

Contoh pada perpustakaan:
Ketiganya dapat digunakan untuk menampilkan informasi seperti nama buku, jumlah buku, atau status ketersediaan buku.

<h3>3. Manipulasi Attribute dan Style</h3>

Manipulasi Attribute adalah proses mengubah atribut yang terdapat pada elemen HTML menggunakan JavaScript. Contohnya seperti mengubah src gambar, href link, atau alt pada gambar.

Manipulasi Style adalah proses mengubah tampilan elemen HTML menggunakan JavaScript, seperti mengubah warna, ukuran, border, dan posisi.

Contoh pada perpustakaan:
Attribute dapat digunakan untuk mengganti gambar sampul buku, sedangkan style dapat digunakan untuk mengubah ukuran atau tampilan gambar tersebut.

Berikut penjelasan **teks** untuk poin 4–6 dengan contoh pada **sistem perpustakaan (perpus)**:

### 4. Membuat & Menghapus Elemen

DOM memungkinkan JavaScript untuk **membuat elemen HTML baru dan menghapus elemen yang sudah ada**. Dalam sistem perpustakaan, contohnya ketika admin menambahkan buku baru, JavaScript dapat membuat elemen berupa data buku dan menampilkannya ke daftar. Sebaliknya, ketika sebuah buku dihapus dari data perpustakaan, elemen buku tersebut juga dapat dihapus dari halaman.

### 5. Event Listener: click, input, submit

Event Listener digunakan agar JavaScript dapat **merespons tindakan yang dilakukan pengguna**. `click` digunakan ketika pengguna menekan tombol, misalnya tombol **Tambah Buku**. `input` digunakan ketika pengguna mengetik, misalnya saat mencari judul buku. `submit` digunakan ketika pengguna mengirim formulir, misalnya saat mengisi data buku baru untuk dimasukkan ke daftar perpustakaan.

### 6. Event Bubbling & StopPropagation

**Event Bubbling** adalah kondisi ketika suatu event dari elemen anak dapat diteruskan ke elemen induknya. Contohnya, ketika tombol **Hapus Buku** berada di dalam sebuah elemen daftar buku, klik pada tombol tersebut juga dapat dianggap sebagai klik pada elemen daftar. `stopPropagation()` digunakan untuk **menghentikan penyebaran event tersebut**, sehingga event hanya dijalankan pada elemen yang diinginkan. Dalam sistem perpustakaan, ini berguna agar tombol Hapus tidak sekaligus menjalankan event lain pada kartu atau daftar buku.

