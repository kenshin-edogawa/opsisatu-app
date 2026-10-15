# opsisatu - Android WebView Project

Proyek aplikasi Android native yang menampilkan situs Google Sites Anda:
**URL:** `https://sites.google.com/view/opsisatu`  
**Package:** `com.opsisatu.android`  
**Version:** `1.0.0` (Code: 1)

---

## 🚀 Cara 1: Build APK Otomatis Lewat GitHub Actions (100% Gratis & Tanpa Install Android Studio)
Jika Anda tidak memiliki PC dengan spek tinggi untuk menjalankan Android Studio:
1. Buat repository baru di [GitHub](https://github.com/new).
2. Upload semua file dalam project ini ke repository tersebut (bisa drag-and-drop atau via git push).
3. Buka tab **Actions** di repository GitHub Anda.
4. GitHub Actions akan otomatis meng-compile APK dalam 2-3 menit.
5. Klik workflow yang selesai, lalu download file **opsisatu-Debug-APK.zip** di bagian Artifacts.
6. Extract dan install file `app-debug.apk` ke HP Android Anda!

---

## 💻 Cara 2: Buka & Build di Android Studio
1. Install [Android Studio](https://developer.android.com/studio) (versi Flamingo / Hedgehog / Iguana / Koala atau lebih baru).
2. Buka Android Studio, pilih **Open**, lalu arahkan ke folder hasil extract ZIP project ini.
3. Tunggu hingga proses **Gradle Sync** selesai.
4. Hubungkan HP Android Anda via kabel USB (aktifkan USB Debugging) ATAU buat Emulator.
5. Klik tombol **Run (Segitiga Hijau)** di pojok kanan atas untuk langsung mencoba di HP.
6. Untuk membuat file APK final siap pasang:
   - Klik menu **Build** > **Build Bundle(s) / APK(s)** > **Build APK(s)**.
   - Setelah selesai, klik notifikasi **locate** untuk mendapatkan file `app-debug.apk`.

---

## 💡 Fitur Unggulan yang Sudah Terpasang:
- ✅ **Google Sites Compatible:** WebView dikonfigurasi dengan User-Agent Chrome mobile agar tidak terkena error "disallowed_useragent" saat pengunjung login Google.
- ✅ **Swipe to Refresh:** Tarik layar ke bawah untuk memuat ulang konten situs.
- ✅ **Deep Links Otomatis:** Tautan tombol WhatsApp (`wa.me`), Telepon (`tel:`), dan Email (`mailto:`) langsung membuka aplikasi native di HP pengunjung.
- ✅ **Halaman Offline Ramah Pengguna:** Jika pengguna kehilangan sinyal/internet, aplikasi menampilkan layar offline dengan tombol "Coba Muat Ulang".
- ✅ **File Upload Support:** Pengunjung dapat mengupload foto / dokumen jika Google Sites Anda memiliki formulir.
- ✅ **Download Manager:** Tautan download file PDF/dokumen otomatis diproses oleh sistem Android.
