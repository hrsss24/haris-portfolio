# Laporan Pemeriksaan

## Pemeriksaan yang dilakukan
- Struktur halaman statis dibuat untuk beranda, profil, pengalaman, portofolio, kontak, indeks blog, dan templat artikel.
- Jalur aset memakai path relatif.
- Menu mobile, filter kategori portofolio, dan tahun footer memakai JavaScript vanilla.
- Gaya responsif mencakup breakpoint tablet dan ponsel serta dukungan `prefers-reduced-motion`.
- Tautan WhatsApp dan unduhan CV yang belum dikonfigurasi tidak ditampilkan sebagai tombol aktif.
- Blog kosong tanpa artikel contoh yang seolah-olah telah diterbitkan.
- Templat artikel memakai `noindex,nofollow` dan diberi label internal.
- Dokumen institusi asli tidak digunakan sebagai sampel proyek.

## Belum diverifikasi secara otomatis / manual di browser
- Uji visual lintas browser dan perangkat fisik.
- Audit keyboard lengkap dengan pembaca layar.
- Pemeriksaan konsol browser dan pengukuran Lighthouse.
- Validasi metadata sosial setelah domain produksi diketahui.
- Uji deploy aktual di akun Netlify.

Karena pengujian browser langsung dan deployment tidak dilakukan di lingkungan ini, laporan ini tidak menyatakan bahwa semua uji penerimaan telah lulus. Lakukan checklist final sebelum publikasi.
