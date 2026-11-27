MyMoney — Paket iPhone / GitHub Pages

ISI PAKET
- index.html: aplikasi utama
- manifest.json: konfigurasi PWA
- sw.js: cache/offline shell aplikasi
- icon-192.png dan icon-512.png: ikon aplikasi

PEMASANGAN
1. Buat cadangan JSON dari aplikasi lama sebelum mengganti file.
2. Ekstrak ZIP.
3. Unggah SEMUA file di dalam paket ke root repository GitHub Pages (folder utama), timpa file versi lama.
4. Tunggu GitHub Pages selesai deploy.
5. Buka situs di Safari. Jika masih versi lama, tutup tab situs, buka kembali; bila perlu hapus data situs/cache lalu pulihkan cadangan JSON.
6. Untuk memasang ke layar utama iPhone: Safari > Bagikan > Tambahkan ke Layar Utama.

FITUR
- Saldo awal dan dompet Tunai, Bank, E-Wallet.
- Pemasukan, pengeluaran, transfer antar-dompet, edit/hapus.
- Foto bukti terkompresi, pratinjau, hapus foto; OCR struk via Tesseract.js (butuh internet, hasil wajib diperiksa).
- Anggaran bulanan keseluruhan dan per kategori, peringatan batas.
- Safe-to-Spend (perkiraan sederhana dari saldo tersedia dan sisa hari bulan berjalan).
- Analisis pengeluaran menurut tingkat kegunaan, rincian barang, kalender, evaluasi pembelian berulang.
- Tabungan terpisah, setoran/penarikan, target, aturan persentase otomatis untuk pemasukan baru, indikator target mingguan/bulanan.
- Wishlist dan daftar pengeluaran rutin dengan pencatatan manual serta penanda periode yang perlu dicatat.
- Ekspor CSV, cetak/simpan PDF melalui dialog cetak browser, cadangkan/pulihkan JSON.

BATASAN PENTING
- Data tersimpan di browser/perangkat ini (localStorage), tidak tersinkron otomatis antarperangkat.
- Foto bukti ikut disimpan di localStorage setelah dikompres. Kapasitas browser terbatas; bila penyimpanan penuh, perubahan dibatalkan dan aplikasi meminta pengguna mengurangi foto/membuat cadangan.
- OCR memerlukan koneksi internet dan dapat salah membaca nominal/tanggal; selalu verifikasi manual.
- Pengeluaran rutin tidak dibukukan otomatis. Aplikasi menandai periode yang perlu dicatat ketika dibuka.
- Pengingat latar belakang/notifikasi terjadwal tidak disediakan; iOS dapat membatasi notifikasi web.
- Target mingguan/bulanan adalah indikator progres, bukan setoran otomatis.
- Safe-to-Spend bukan nasihat keuangan atau prediksi arus kas; periksa tagihan dan kebutuhan mendatang secara manual.
- Belum ada sinkronisasi cloud, multi-user, atau enkripsi khusus untuk data lokal. Gunakan kunci layar perangkat dan jangan bagikan file cadangan.

PENTING
Lakukan uji dengan transaksi contoh terlebih dahulu. Simpan cadangan JSON secara berkala. Jangan mengandalkan aplikasi sebagai satu-satunya arsip keuangan.
