# Dashboard Monitoring Karhutla — PT Telaga Mas Kalimantan

Dashboard statis berbasis HTML, Chart.js, Leaflet, dan GitHub Pages. Bisa mengimpor file Excel (.xlsx/.xls) atau CSV langsung di browser.

## Isi paket
- `index.html` — dashboard utama.
- `template_excel/template_monitoring_karhutla_tmk.xlsx` — template sumber data Excel.
- `README.md` — petunjuk instalasi dan penggunaan.

## Publikasi ke GitHub Pages
1. Buat repository GitHub, misalnya `dashboard-karhutla-tmk`.
2. Upload `index.html`, folder `template_excel`, dan `README.md` ke root repository.
3. Buka **Settings → Pages**.
4. Di **Build and deployment**, pilih **Deploy from a branch**.
5. Pilih branch `main` dan folder `/ (root)`, lalu klik **Save**.
6. Setelah selesai, buka URL yang ditampilkan GitHub Pages, biasanya `https://USERNAME.github.io/dashboard-karhutla-tmk/`.

## Menggunakan Excel
1. Unduh atau buka `template_excel/template_monitoring_karhutla_tmk.xlsx`.
2. Isi sheet `Data_Karhutla`. Pertahankan nama kolom di baris pertama.
3. Buka dashboard yang sudah dipublikasikan.
4. Klik **Import Excel** dan pilih file.
5. Grafik, KPI, tabel, dan marker peta diperbarui berdasarkan file yang diimpor.
6. Tombol **Unduh data CSV** mengekspor data yang sedang terfilter.

## Kolom yang dibaca
`Tanggal`, `ID`, `Lokasi`, `Latitude`, `Longitude`, `Hotspot`, `Luas_ha`, `Risiko`, `Status`, `Patroli_pct`, `PIC`.

## Catatan penting
- Data di dashboard bawaan hanyalah **data simulasi**, bukan data kejadian aktual PT TMK. Ganti dengan data terverifikasi.
- Import Excel berjalan di browser pengguna. File tidak otomatis tersimpan ke GitHub atau server.
- Untuk memperbarui data, impor ulang Excel saat membuka dashboard. Jika ingin data langsung tersedia untuk semua pengguna, siapkan dataset publik terpisah atau backend/database dengan kontrol akses.
- Peta memakai tile OpenStreetMap dan memerlukan internet.
- Dashboard GitHub Pages bersifat publik bila repository dipublikasikan secara publik. Jangan unggah data sensitif, koordinat titik rawan yang dibatasi, nomor kontak pribadi, atau informasi operasional rahasia.
- Ini alat bantu monitoring, bukan pengganti prosedur tanggap darurat, validasi lapangan, atau sumber resmi hotspot.
