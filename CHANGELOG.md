# Changelog

Semua perubahan penting pada proyek ini akan dicatat dalam file ini.

## [1.0.0] - 2026-04-02

### Ditambahkan

- Implementasi awal aplikasi `Folder Compare & Delete`.
- Fitur pemindaian dan perbandingan isi dari beberapa folder sekaligus.
- Antarmuka pengguna visual berbasis Treeview menggunakan pustaka bawaan `Tkinter/ttk` (tanpa dependensi UI eksternal).
- Dua mode pembandingan: mode cepat (Nama + Ukuran) & mode akurat (Hash SHA-256 + Ukuran).
- Sistem pemrosesan pemindaian berjalan secara asinkron (*thread-based background scanning*) sehingga antarmuka tetap responsif.
- Fitur penghapusan *recycle bin* untuk memastikan file terhapus dengan aman (menggunakan paket `send2trash`).
- Konfirmasi penghapusan massal untuk meminimalisasi kesalahan.
- Tabel hasil warna warni untuk hasil perbandingan yang intuitif (Hijau untuk duplikat sama persis, Merah untuk nama sama isi berbeda, Oranye untuk file unik).
- Fitur ekspor hasil perbandingan log lengkap ke format CSV dan Excel (`openpyxl`).

### Diperbarui

- Pengoptimasian kode dan penyesuaian GUI agar dapat dijalankan di Windows, macOS, dan Linux.
