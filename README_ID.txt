DERLYSTOPIA ANDROID - SIAP BUILD APK

Struktur Android (app/, app/src/, dan file konfigurasi) sudah lengkap.
Gradle Wrapper tidak disertakan; workflow GitHub Actions di bawah memakai Gradle 8.7 yang dipasang otomatis, jadi tidak membutuhkan gradlew.

CARA MEMBUAT APK TANPA KOMPUTER (melalui GitHub)
1. Ekstrak ZIP ini.
2. Buat repository baru di https://github.com/ lalu upload seluruh ISI folder DerlysTopia_Android_Project (pastikan .github ikut ter-upload) ke branch main.
3. Buka tab Actions pada repository. Jika diminta, izinkan GitHub Actions.
4. Pilih workflow "Build DerlysTopia APK" lalu tekan Run workflow.
5. Tunggu sampai status workflow hijau/Sukses. Buka proses yang selesai.
6. Di bagian Artifacts, unduh "DerlysTopia-debug-apk" lalu ekstrak ZIP artifact tersebut.
7. Pindahkan app-debug.apk ke HP Android dan buka untuk memasang. Jika diminta, izinkan instalasi dari sumber tersebut di Pengaturan Android.

CARA DENGAN ANDROID STUDIO
Buka folder proyek ini di Android Studio. Pastikan Gradle 8.7, Android SDK Platform 35, dan Build Tools 35.0.0 terpasang. Pilih Build > Build Bundle(s) / APK(s) > Build APK(s).

CATATAN
- APK yang dihasilkan adalah debug APK untuk uji coba/install pribadi, bukan rilis Play Store.
- Package aplikasi: com.derlystopia.game
- Minimum Android: Android 6.0 (API 23).
- Aplikasi saat ini menjalankan game HTML lokal melalui Android WebView.
- Build APK tidak dapat dijalankan di lingkungan ini karena Android SDK/Gradle tidak tersedia; gunakan GitHub Actions sesuai langkah di atas.
