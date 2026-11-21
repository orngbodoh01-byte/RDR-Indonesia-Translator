# RDR Indonesia Translator — Android 13

Aplikasi prototipe Android untuk mendeteksi teks subtitle di area bawah layar dengan ML Kit OCR, menerjemahkan Inggris ke Indonesia, dan menampilkan hasil di floating overlay.

## Build APK melalui GitHub
1. Unduh dan ekstrak ZIP proyek.
2. Buat repository baru di https://github.com/new.
3. Upload seluruh isi folder proyek ke repository (pastikan `.github/workflows/build.yml` ikut terunggah).
4. Buka tab **Actions** dan pilih **Build Android APK**.
5. Klik **Run workflow** jika belum berjalan otomatis.
6. Setelah selesai, buka hasil workflow dan unduh artifact `RDR-Indonesia-Translator-Android13`.
7. Ekstrak artifact dan pasang `app-debug.apk` di HP Android 13.

## Cara pakai
1. Instal APK.
2. Buka aplikasi dan izinkan tampil di atas aplikasi lain.
3. Setujui izin notifikasi jika diminta.
4. Tekan **MULAI TERJEMAHAN**, lalu setujui perekaman layar.
5. Buka game. Hasil terjemahan akan muncul sebagai overlay di bagian bawah.
6. Untuk berhenti, buka kembali aplikasi dan tekan **HENTIKAN TERJEMAHAN**; jika aplikasi sudah tertutup, hentikan layanan dari pengaturan aplikasi Android.

## Batasan prototipe
- Belum dikompilasi atau diuji pada perangkat pengguna; GitHub Actions diperlukan untuk menghasilkan APK.
- Model terjemahan diunduh saat pertama kali digunakan, jadi koneksi internet diperlukan.
- OCR hanya memfilter teks di area bawah layar. Subtitle yang posisinya berbeda, teks HUD, atau menu dapat menyebabkan hasil kurang akurat.
- Kecepatan OCR/terjemahan bergantung pada performa perangkat.
- Android akan menampilkan indikator dan notifikasi perekaman layar. Aplikasi tidak menyimpan rekaman video.
- Pastikan penggunaan perekaman layar sesuai aturan game dan privasi.
