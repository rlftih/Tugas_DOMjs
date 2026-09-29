. querySelector dan querySelectorAll

Pengertian:

querySelector() → memilih 1 elemen pertama yang sesuai selector.
querySelectorAll() → memilih semua elemen yang sesuai selector.

Contoh kasus perpustakaan:

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

Pengertian:

innerHTML → mengambil/mengubah isi HTML sekaligus tag HTML.
textContent → mengambil/mengubah seluruh teks.
innerText → mengambil/mengubah teks yang terlihat di halaman.

Contoh:

<div id="info"></div>

<script>
const info = document.querySelector("#info");

info.innerHTML = "<b>Buku tersedia: 25</b>";

Hasilnya:

Buku tersedia: 25

Contoh textContent:

info.textContent = "Buku tersedia: 25";

Contoh innerText:

info.innerText = "Buku tersedia: 25";
3. Manipulasi Attribute dan Style

Pengertian:
Manipulasi attribute digunakan untuk mengubah atribut HTML, sedangkan manipulasi style digunakan untuk mengubah tampilan elemen menggunakan JavaScript.

Contoh kasus perpustakaan:

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

DOM memungkinkan JavaScript mengambil, mengubah, dan mengatur elemen HTML secara langsung. Dalam kasus perpustakaan, DOM dapat digunakan untuk mengubah daftar buku, informasi buku, gambar sampul, serta tampilan halaman secara dinamis.# Tugas_DOMjs
