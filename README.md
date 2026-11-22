# Kas Konten: 500 Judul Konten Finansial (PWA)

Checklist 500 judul konten finansial lengkap dengan caption YouTube. Tandai judul yang sudah dirender dan yang sudah diposting, lihat progresnya di peta 500 kotak, lalu salin caption saat mau mengunggah. Bisa dipasang seperti aplikasi dan jalan offline.

## Isi folder
- `index.html`: aplikasi (seluruh judul dan caption ada di dalamnya)
- `manifest.webmanifest`, `sw.js`, `icons/`, `.nojekyll`: kebutuhan PWA dan GitHub Pages

## Deploy ke GitHub Pages
1. Upload seluruh isi folder ke root repo (pastikan `.nojekyll` ikut).
2. Settings, Pages, Deploy from a branch, branch `main`, folder `/ (root)`.
3. Alamatnya: `https://USERNAME.github.io/NAMA-REPO/`

## Cara pakai
- Tiap tiket punya dua centang: **Dirender** dan **Diposting**. Merender banyak video sekaligus lalu memposting bertahap pun bisa dilacak.
- Mencentang Diposting otomatis menandai Dirender. Membatalkan Dirender juga membatalkan Diposting.
- Peta 500 kotak: redup belum dirender, sedang sudah dirender, pekat sudah diposting. Klik kotak untuk melompat ke judulnya.
- Filter: kategori, status (Semua, Belum dirender, Siap diposting, Sudah diposting), dan pencarian. Tombol **Acak judul** memilih satu judul yang belum dirender.
- Menu ⋯: salin daftar belum dirender atau siap diposting, unduh semua caption (.txt), cadangkan atau pulihkan progres, reset.

## Data progres
Tanda disimpan di browser (localStorage), terpisah antar perangkat. Pindahkan lewat menu ⋯, Cadangkan progres, lalu Pulihkan progres. Menghapus data situs akan menghapus tanda.

## Update
Mengubah `index.html` otomatis terbaca saat online. Jika mengganti ikon atau manifest, ubah angka `VERSION` di `sw.js` agar cache lama diganti.
