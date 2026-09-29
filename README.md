1. querySelector dan querySelectorAll
Penjelasan

querySelector() digunakan untuk memilih satu elemen pertama berdasarkan selector seperti id, class, atau tag HTML.

querySelectorAll() digunakan untuk memilih semua elemen yang memiliki selector yang sama.

Contoh kasus: Pada perpustakaan, kita dapat memilih judul perpustakaan dan semua daftar buku.

Kode
<h2 id="judul">Daftar Buku</h2>

<ul>
    <li class="buku">Laskar Pelangi</li>
    <li class="buku">Bumi Manusia</li>
    <li class="buku">Negeri 5 Menara</li>
</ul>

<script>
const judul = document.querySelector("#judul");
const buku = document.querySelectorAll(".buku");

judul.textContent = "Koleksi Buku Perpustakaan";

buku.forEach(item => {
    item.style.color = "blue";
});
</script>
2. innerHTML, textContent, dan innerText
Penjelasan

Ketiganya digunakan untuk mengambil atau mengubah isi suatu elemen HTML.

innerHTML → dapat mengubah isi sekaligus menggunakan tag HTML.
textContent → mengubah atau mengambil seluruh teks di dalam elemen.
innerText → mengubah atau mengambil teks yang terlihat oleh pengguna.

Contoh kasus: Menampilkan jumlah buku yang tersedia di perpustakaan.

Kode innerHTML
<div id="info"></div>

<script>
const info = document.querySelector("#info");

info.innerHTML = "<b>Buku tersedia: 25</b>";
</script>
Kode textContent
info.textContent = "Buku tersedia: 25";
Kode innerText
info.innerText = "Buku tersedia: 25";
3. Manipulasi Attribute dan Style
Penjelasan

Manipulasi attribute digunakan untuk mengubah atribut HTML, seperti src, href, alt, dan lainnya.

Manipulasi style digunakan untuk mengubah tampilan elemen, seperti ukuran, warna, border, dan sebagainya.

Contoh kasus: Mengubah gambar sampul buku dan mengatur ukurannya.

Kode
<img id="cover" src="buku-lama.jpg" alt="Buku">

<script>
const cover = document.querySelector("#cover");

// Manipulasi attribute
cover.setAttribute("src", "buku-baru.jpg");
cover.setAttribute("alt", "Cover Buku Baru");

// Manipulasi style
cover.style.width = "200px";
cover.style.border = "2px solid black";
</script>
Kesimpulan

DOM memungkinkan JavaScript untuk memilih, mengubah isi, atribut, dan tampilan elemen HTML. Dalam sistem perpustakaan, DOM dapat digunakan untuk mengelola daftar buku dan informasi buku secara dinamis.
