# Filter Dashboard – NG Inspeksi Permukaan SPL (Coupling Station)

Dashboard interaktif untuk menelusuri data NG hasil inspeksi permukaan SPL (PLC Splitter) per hari, minggu, bulan, operator, pemeriksa, jenis NG, tipe produk, dan No. PO.

**Demo:** https://bagusbernadi.github.io/filter-dashboard/

> Versi ini **statis** dan memakai **data demo**: No. PO dan SN sudah disamarkan. Pola datanya (jumlah, tanggal, jenis NG, SN berulang) sama dengan data asli. Fitur **Input data** belum diaktifkan dan akan menampilkan pesan *Coming soon*.

## Fitur
- **Slicer multi-pilih:** Bulan, Operator, Pemeriksa, Jenis NG, NG Lainnya, Tipe, Tindakan, Status, Nama hari, No. PO.
- **Filter periode:** rentang tanggal dan tombol cepat (7H, 30H, Bulan ini, Bulan lalu, Semua). Ada juga pencarian SN, PO, atau catatan.
- **KPI:** total NG, hari kerja, rata-rata per hari, NG terbanyak, operator terbanyak, SN berulang (rework), dan baris bermasalah.
- **Tren NG:** per hari, minggu, atau bulan, dengan tampilan Total, Per jenis NG (*small multiples*), atau Heatmap.
- **Pareto NG** per Jenis NG, Operator, Tindakan, NG Lainnya, atau No. PO. Pada Pareto per No. PO, batang diwarnai sesuai Tipe dan Tipe bisa di-highlight.
- **Grafik pendukung:** Jenis NG, Operator, Pemeriksa, Tindakan, NG Lainnya, Tipe produk (pie), serta matriks Operator × Jenis NG.
- **Tabel tracing per SN:** filter di setiap header kolom, riwayat per SN, dan Export CSV.
- **Export PDF** A4 portrait. Bagian yang dimasukkan bisa dipilih, ringkasan dibuat otomatis, dan bahasanya mengikuti tampilan.
- **Bahasa:** Indonesia, English, 中文.
- **Data sendiri:** bisa memuat file form Excel Rekap NG dengan *drag & drop* file `.xlsx` ke halaman.

## Teknologi
Satu file `index.html` yang berjalan offline, tanpa server. Library yang dipakai (Chart.js, SheetJS, jsPDF, html2canvas) sudah tertanam di file.

## Catatan
Versi lengkap dengan login, input data dari PC/HP, validasi, dan log aktivitas berjalan di server lokal (Flask + SQLite) dan tidak termasuk dalam repo publik ini.

---
Dibuat oleh **Bagus Bernadi**.
