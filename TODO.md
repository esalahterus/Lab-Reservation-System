# TODO - pembatasan booking 2 jam sebelum sesi

- [x] Ubah `api/reservasi.php`: tambahkan validasi server-side di fungsi `buat()` agar slot hanya boleh dipilih jika waktu mulai sesi >= 2 jam dari sekarang.
- [x] Ubah `api/reservasi.php`: modifikasi output `slot_status()` agar field `expired` juga menandai slot yang kurang dari 2 jam dari sekarang (bukan hanya sesi yang sudah lewat).
- [x] Ubah `dosen/reservasi.php`: nonaktifkan slot yang `expired === 1` (agar tidak memanggil `pickSlot()` dan tombol tampil merah).
- [ ] Testing manual: pilih sesi < 2 jam harus gagal/ tidak bisa dipilih; sesi >= 2 jam sukses.
- [ ] Testing manual: batal reservasi < 2 jam harus gagal; batal >= 2 jam sukses.



