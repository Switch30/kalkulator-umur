# Kalkulator Umur

Kalkulator umur satu halaman yang kelihatannya biasa aja — masukin tahun lahir, dapet umur. Tapi umur yang muncul pertama kali sengaja salah (acak 15–22 tahun), sebelum akhirnya dikoreksi ke umur asli dan berlanjut ke refleksi soal ekspektasi umur ("harusnya udah nikah di umur segini", dst) yang dipersonalisasi sesuai umur asli pengguna.

Dibangun sebagai satu file statis (HTML + CSS + JS vanilla), tanpa dependency atau build step.

## Menjalankan

Buka `index.html` langsung di browser, atau serve dengan server statis apa pun, misalnya:

```bash
npx serve .
```

## Struktur alur

1. **Input** — tahun lahir (bukan tanggal lengkap, demi privasi).
2. **Loading palsu** — animasi "menghitung" yang sengaja berlebihan.
3. **Hasil palsu** — umur acak 15–22 tahun, dijamin beda dari umur asli.
4. **Koreksi** — umur asli ditampilkan (perkiraan berbasis tahun).
5. **Refleksi** — timeline ekspektasi umur (18–50 tahun) yang dipersonalisasi berdasarkan umur asli pengguna.
6. **Umur yang dirasakan** — pertanyaan penutup yang playful, menutup dengan pesan bahwa satu-satunya angka yang valid adalah yang kamu rasakan sendiri.
