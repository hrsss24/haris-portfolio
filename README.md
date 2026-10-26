# Website Personal — Harits Abdurrohman Alfauzan

Website portofolio statis dengan HTML5, CSS3, dan JavaScript vanilla. Tidak memerlukan backend, CMS, framework, atau proses build.

## Struktur

- `index.html` — Beranda
- `profil.html` — Biografi, pendidikan, keterampilan, dan minat
- `pengalaman.html` — Pengalaman kerja, administrasi pendidikan, dan organisasi
- `portofolio.html` — Ringkasan proyek dengan filter kategori dan galeri foto
- `kontak.html` — Tautan Instagram dan informasi konfigurasi kontak
- `blog/index.html` — Indeks blog dengan empty state
- `blog/posts/article-template.html` — Templat artikel internal (noindex; jangan diterbitkan sebagai artikel nyata)
- `assets/css/style.css` — Gaya responsif
- `assets/js/main.js` — Menu mobile, filter portofolio, dan tahun footer
- `assets/images/` — Foto yang dipakai website dan referensi visual
- `robots.txt`, `sitemap.xml` — Berkas dasar untuk pengindeksan
- `TESTING-REPORT.md` — Catatan pemeriksaan yang dilakukan
- `ASSET-CHECKLIST.md` — Daftar aset tersedia dan yang masih dibutuhkan

## Menjalankan secara lokal

1. Ekstrak ZIP.
2. Buka `index.html` langsung di browser modern. Karena semua rute menggunakan berkas relatif, tidak diperlukan server untuk peninjauan dasar.
3. Untuk pengujian yang lebih representatif, jalankan server statis lokal dari folder proyek, misalnya `python -m http.server 8000`, lalu buka `http://localhost:8000`. Perintah ini hanya untuk pratinjau lokal, bukan proses build.

## Mengedit konten

- Ubah teks pada berkas HTML terkait.
- Navigasi dibuat langsung di setiap halaman agar dapat dipakai tanpa build. Jika menambah atau mengganti halaman, perbarui navigasi yang relevan secara konsisten.
- Gaya global ada di `assets/css/style.css`; interaksi kecil ada di `assets/js/main.js`.
- Jangan menambahkan jabatan, tanggal, metrik, sertifikat, hasil proyek, atau klaim yang belum diverifikasi.

## Menambahkan artikel blog

1. Siapkan naskah final asli yang memang ditulis dan disetujui pemilik website.
2. Salin `blog/posts/article-template.html` ke nama berkas baru, misalnya `blog/posts/judul-artikel.html`.
3. Ganti judul, deskripsi, tanggal terbit, kategori, isi, dan metadata. Hapus `noindex,nofollow` hanya setelah artikel siap dipublikasikan.
4. Tambahkan kartu artikel ke `blog/index.html` dan, jika relevan, cuplikan di `index.html`.
5. Pastikan tautan kembali, metadata, sumber, dan ejaan benar. Jangan gunakan tanggal fiktif.
6. Perbarui sitemap setelah domain produksi dan URL artikel tersedia.

Blog sengaja diluncurkan tanpa artikel contoh, karena belum ada naskah asli yang disediakan.

## Mengganti/menambah aset

- Foto profil: ganti `assets/images/harits-portrait.jpg` dengan foto yang disetujui, sambil mempertahankan nama berkas atau perbarui semua referensi `src`.
- Foto pendakian: `pendakian-01.jpg`, `pendakian-02.jpg`, dan `pendakian-03.jpg`.
- `referensi-portfolio.jpg` dan `referensi-cv.jpg` hanya disertakan sebagai referensi dari unggahan. Keduanya tidak ditampilkan sebagai karya nyata di halaman publik.
- Tambahkan teks alternatif yang mendeskripsikan gambar secara akurat.

## Kontak WhatsApp

Nomor WhatsApp belum disediakan. Karena itu, website tidak menampilkan tombol `wa.me` yang belum valid. Setelah nomor diberikan dan disetujui untuk publikasi, tambahkan tautan dengan format `https://wa.me/` diikuti nomor internasional tanpa tanda `+`, spasi, atau tanda hubung; kemudian tampilkan komponen kontak di `kontak.html`. Verifikasi tautan sebelum diterbitkan.

## CV dan domain

CV yang dapat diunduh belum dikonfigurasi. Berkas gambar CV referensi bukan pengganti otomatis untuk CV final yang disetujui untuk publikasi. Setelah CV final disetujui, letakkan berkasnya di folder aset dan tambahkan tautan unduh pada `profil.html`.

Domain khusus belum diketahui. Metadata canonical sengaja tidak ditambahkan dan sitemap belum berisi URL absolut. Setelah domain produksi ditetapkan, perbarui judul/deskripsi bila perlu, metadata Open Graph, canonical URL, `robots.txt`, dan `sitemap.xml`.

## Deploy ke Netlify

1. Ekstrak arsip ZIP.
2. Masuk ke Netlify dan buat situs baru dengan metode deploy manual/drag-and-drop yang tersedia di akun.
3. Unggah folder `harits-portfolio` (atau isi folder proyek) dengan `index.html` berada di root direktori publik.
4. Tidak diperlukan build command. Publish directory adalah root folder proyek yang berisi `index.html`.
5. Setelah situs terbit, uji semua halaman, gambar, menu mobile, filter portofolio, serta tautan eksternal.
6. Untuk pembaruan, edit file lokal dan unggah/deploy ulang folder yang telah diperbarui sesuai alur Netlify yang digunakan.
7. Domain khusus dapat dihubungkan melalui pengaturan domain Netlify setelah domain dimiliki/dikonfigurasi.

## Privasi dan akurasi

Portofolio hanya berisi deskripsi umum dan foto personal yang diberikan. Jangan mengunggah dokumen institusi asli, data mahasiswa, surat internal, arsip, dokumen perizinan, atau korespondensi privat. Keterangan proyek bukan klaim persetujuan atau endorsement dari institusi.
