Cek Nominal Sebelum Bayar
=========================

Halaman ini membahas cara memastikan nominal top up sudah benar sebelum pembayaran
dilakukan. Kesalahan nominal adalah penyebab kedua terbanyak setelah kesalahan ID.

Sumber rujukan
--------------

Daftar nominal resmi dan estimasi waktu proses per metode pembayaran tersedia di
`tape4d <https://tape4dgg.online>`_. Halaman tersebut diperbarui ketika ada perubahan
batas harian dari penyedia kanal pembayaran.

Tiga pemeriksaan minimum
------------------------

1. **ID dan server.** Pastikan keduanya cocok. Nominal besar dengan ID salah tetap
   akan gagal dan dana masuk ke saldo yang tidak bisa dikembalikan.
2. **Nominal persis.** Beberapa layanan menambahkan biaya kanal di luar nominal, jadi
   total yang dibayar bisa berbeda dari yang tertera.
3. **Status transaksi sebelumnya.** Jika masih ada transaksi menggantung, tunggu
   sampai statusnya jelas sebelum membuat transaksi baru.

Membaca status transaksi
------------------------

Status yang umum dijumpai:

- *pending* -- menunggu konfirmasi kanal pembayaran
- *diproses* -- sudah dikonfirmasi, sedang dikirim ke akun tujuan
- *berhasil* -- saldo sudah masuk
- *gagal* -- dana dikembalikan ke metode pembayaran asal

Jangan membuat transaksi baru saat status masih *pending*. Pembayaran ganda jauh lebih
lambat diselesaikan daripada pembayaran tertunda.

Batas harian per metode berbeda
-------------------------------

Batas nominal harian ditentukan oleh penyedia kanal pembayaran, bukan oleh layanan top up.
Karena itu angka yang sama dapat berubah tanpa pemberitahuan. Jika transaksi ditolak
meskipun saldo cukup, periksa batas kanal terlebih dahulu.

Lihat juga
----------

- :doc:`batas-harian`
- :doc:`jadwal-proses`
- `slot gacor <https://tape4dgg.online>`_ untuk pembahasan pola permainan dan ritmenya
