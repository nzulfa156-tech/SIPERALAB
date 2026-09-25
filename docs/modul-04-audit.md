# Audit Modul 4 - Flexbox, Grid, dan Responsive Design

## Hasil uji viewport

| Viewport | Gejala awal | Penyebab | Perbaikan | Hasil uji ulang |
|---|---|---|---|---|
| 360 px | Form harus tetap terbaca dalam satu kolom | Ruang layar sempit | Menggunakan CSS Grid mobile-first dengan satu kolom | Form tersusun satu kolom dan tidak ada horizontal scroll |
| 768 px | Form masih membutuhkan susunan yang lebih rapi | Ruang layar sudah cukup untuk dua kolom | Menambahkan `grid-template-columns: repeat(2, minmax(0, 1fr))` pada media query | Form berubah menjadi dua kolom dan tetap rapi |
| 1280 px | Perlu memastikan layout tetap stabil pada layar lebar | Lebar layar lebih besar | Menggunakan Grid dan Flexbox yang fleksibel | Layout tetap rapi dan tidak ada horizontal scroll |

## Audit overflow

- Elemen yang menyebabkan overflow: Tidak ditemukan.
- Bukti dari DevTools: Tidak ada horizontal scroll pada viewport yang diuji.
- Aturan penyebab: Tidak ada aturan yang menyebabkan overflow.
- Perbaikan: Menggunakan layout Flexbox dan Grid yang fleksibel serta aturan media yang responsif.
- Hasil uji ulang: Layout tetap dapat digunakan pada 360 px, 768 px, dan 1280 px.

## Kesimpulan

Flexbox digunakan untuk menyusun elemen dalam satu arah seperti header, navigasi, hero, dan tombol. Grid digunakan untuk menyusun katalog dan kelompok field pada form. Layout diuji pada beberapa ukuran viewport agar tetap terbaca dan dapat digunakan.