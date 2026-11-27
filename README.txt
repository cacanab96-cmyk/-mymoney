MyMoney v14 — pemulihan cadangan foto lebih aman

Basis: MyMoney v13. Desain dan fitur yang ada dipertahankan.

Perbaikan:
- Impor JSON kini memeriksa apakah isi foto benar-benar disertakan.
- Foto cadangan ditulis ke IndexedDB sebelum appState diganti.
- Transaksi yang dipulihkan menyimpan receiptId, bukan base64 besar di localStorage.
- Jika penulisan foto atau penyimpanan state gagal, foto yang sempat tersentuh dikembalikan ke isi sebelumnya dan state lama dipulihkan.
- Cadangan dengan receiptId tanpa data foto ditolak agar tidak memberi kesan pemulihan foto berhasil.
- Foto individual di atas batas 12 MiB ditolak dengan pesan yang jelas.

Pemeriksaan otomatis:
- Semua blok JavaScript inline lolos node --check.
- Tidak ditemukan ID HTML duplikat.
- Arsip ZIP lolos tes integritas.

Belum diuji:
- Pengujian browser nyata/Safari iPhone.
- Pengujian IndexedDB lintas sesi dan saat ruang penyimpanan hampir penuh.
- Uji end-to-end transaksi, transfer, tabungan, serta impor-ekspor memakai data simulasi.
- Sinkronisasi cloud dan notifikasi latar belakang belum tersedia.

Sebelum mengganti versi utama, ekspor cadangan JSON dari aplikasi yang sedang dipakai.
Paket ini masih beta.
