# Audit Modul 03 — CSS dan Box Model

## 1. Audit Box Model

Elemen yang diperiksa: `article.equipment-card` (Mikroskop)

| Bagian | Hasil |
|---|---|
| Content | 336 × 495.500 px |
| Padding | 16 px |
| Border | 2 px |
| Margin | 16 px |

## 2. Temuan Sebelum Perbaikan

1. Kartu peralatan belum menggunakan class `equipment-card`.
2. Border dan padding kartu belum menggunakan style khusus.
3. Input, select, dan textarea belum memiliki lebar dan border yang konsisten.

## 3. Perbaikan yang Dilakukan

1. Menambahkan `class="equipment-card"` pada tiga elemen `<article>` di `peralatan.html`.
2. Menambahkan background, border, radius, padding, dan margin pada `.equipment-card`.
3. Mengatur `input`, `select`, dan `textarea` dengan `width: 100%`, padding, border, dan radius.
4. Menambahkan focus state untuk input, select, textarea, button, dan link.
5. Menambahkan `box-sizing: border-box` secara global.

## 4. Hasil Setelah Perbaikan

- Tiga kartu peralatan memiliki gaya yang konsisten.
- Gambar tidak melewati lebar kartu.
- Kartu memiliki padding, border, radius, dan margin.
- Box Model dapat diperiksa melalui DevTools.