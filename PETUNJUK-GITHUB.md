# Aplikasi Keuangan Komite SD The Naff

## Isi paket
- `index.html` — aplikasi keuangan
- `logo-the-naff.png` — identitas visual gabungan logo sekolah dan buku terbuka
- `manifest.webmanifest`, `icon-192.png`, `icon-512.png` — dukungan instalasi PWA
- `service-worker.js` — cache agar aplikasi dapat dibuka kembali saat offline

## Penyempurnaan versi 2
- Logo The Naff dicantumkan pada hasil cetak laporan.
- Filter laporan tersedia untuk semua periode, bulanan, dan tahunan.
- Laporan menampilkan saldo awal periode, penerimaan, pengeluaran, saldo akhir, rincian penerimaan, dan pengeluaran per kelompok.
- Ekspor CSV mengikuti periode laporan yang dipilih.
- Pemulihan backup dan penghapusan seluruh data memakai konfirmasi dua tahap.

## Cara menerbitkan melalui GitHub Pages
1. Masuk ke GitHub dan buat repository baru, misalnya `keuangan-komite-the-naff`.
2. Pilih repository **Public** (atau pastikan paket GitHub Anda mendukung Pages untuk repository Private).
3. Unggah seluruh isi folder paket ini ke folder utama repository (root), bukan folder ZIP-nya.
4. Buka **Settings → Pages**.
5. Pada **Build and deployment**, pilih **Deploy from a branch**.
6. Pilih branch `main` dan folder `/(root)`, lalu klik **Save**.
7. Tunggu proses publikasi selesai. GitHub akan menampilkan alamat website pada halaman Pages.

## Cara memasang di HP
1. Buka alamat GitHub Pages melalui Chrome.
2. Pilih menu browser ⋮ lalu **Install app** atau **Tambahkan ke layar utama**.
3. Jalankan aplikasi dari ikon **Kas The Naff**.

## Penting tentang database lokal
- Data transaksi disimpan di penyimpanan browser pada perangkat yang digunakan (`localStorage`).
- GitHub Pages hanya meng-host file aplikasi; GitHub bukan database transaksi.
- Data di HP dan komputer **tidak otomatis sama atau tersinkronisasi**.
- Gunakan menu **Backup Data → Unduh Backup Data (JSON)** pada perangkat sumber, lalu pindahkan file tersebut ke perangkat lain dan gunakan **Pulihkan dari Backup**.
- Jangan hapus data situs/browser atau uninstall browser sebelum membuat backup.
- Jika beberapa perangkat mengedit data masing-masing, backup dari satu perangkat yang dipulihkan ke perangkat lain akan mengganti data lokal di perangkat tujuan. Simpan backup berkala dan beri nama file berdasarkan tanggal/perangkat.

## Privasi
Paket ini tidak mengirim transaksi ke server. Setiap perangkat menyimpan datanya sendiri. Siapa pun yang dapat membuka aplikasi pada perangkat dan browser yang sama berpotensi mengakses data lokalnya; GitHub Pages tidak menyediakan login pengguna untuk database lokal.


## Versi 12.1
- Menambahkan kredit kecil di sudut kanan bawah aplikasi: Design by: yb_wiguna · Versi 12.1.

## Versi 12.2
- Kredit Design by: yb_wiguna · Versi 12.2 ditempatkan langsung di footer aplikasi agar selalu terlihat di bagian kanan bawah.
- Cache PWA diperbarui agar browser mengambil file terbaru setelah deployment.

## Versi 12.3
- Menghapus kredit duplikat di bawah footer; hanya satu kredit tersisa di sisi kanan footer.
