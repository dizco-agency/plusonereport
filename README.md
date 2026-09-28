# Plus One Advisory — Performance Reports

Homepage interaktif berisi daftar laporan performa Plus One Advisory (by DIZCO).

## Struktur
```
index.html              → homepage (list per bulan + link ke report)
agustus/monthly.html    → Laporan Bulanan Agustus 2026
september/week-2.html   → Laporan September Week 2 (periode 1–22 Sep 2026)
september/week-4.html   → Laporan September Week 4 (belum di-upload → tampil "Segera")
```

## Nambah report baru
1. Taruh file report di folder bulannya dengan nama sesuai config, mis. `september/week-4.html`.
   Homepage otomatis mendeteksi file itu & mengaktifkan tombol "Buka report".
2. Oktober sudah ada di config `index.html` (array `MONTHS`) sebagai `oktober/monthly.html`.
   Kalau Oktober juga per 2 minggu, ganti isi `weeks` Oktober jadi Week 2 & Week 4 seperti September.
3. Bulan lain? Tambahin 1 objek di array `MONTHS` dalam `index.html`.

## Deploy (GitHub Pages)
- Push semua file ke repo, aktifkan GitHub Pages (Settings → Pages → branch `main`, root).
- Buka `https://<user>.github.io/<repo>/`.

## Catatan
- Tanpa password.
- Report interaktif — paling enak dibuka di browser (Chrome). Video creative tampil via Google Drive preview; supaya bisa diputar publik, set file video-nya "Anyone with the link" di Drive.
- Jangan ikut upload `desktop.ini` (file bawaan Google Drive).
