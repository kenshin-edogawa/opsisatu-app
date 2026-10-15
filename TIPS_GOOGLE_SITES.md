# Tips Spesial Menjalankan Google Sites di Android WebView

1. **Mengapa Google Sites sering tidak bisa dibuka di iframe browser komputer, tapi BISA di Android WebView?**
   Google Sites menggunakan header proteksi `X-Frame-Options: SAMEORIGIN` untuk mencegah serangan clickjacking di web browser umum. Namun, komponen **Android Native WebView** tidak membatasi X-Frame-Options ini secara default karena WebView memuat URL secara langsung sebagai origin utama (`loadUrl`), bukan sebagai tag `<iframe>` dalam website lain!

2. **Login Akun Google (Google Sign-In) di WebView:**
   Google memblokir login akun Google di WebView biasa dengan pesan *403: disallowed_useragent*.
   Project ini sudah otomatis mengatasi ini dengan menghapus string `; wv` dari User-Agent bawaan Android, sehingga Google mendeteksinya sebagai browser Google Chrome Mobile asli!

3. **Tombol WhatsApp (Chat CS):**
   Jika situs Anda memiliki tombol WhatsApp (`https://wa.me/62812...`), project ini sudah dilengkapi handler otomatis untuk mengalihkan tautan langsung ke aplikasi WhatsApp di ponsel pengguna.

4. **Formulir & Unggah Berkas (Google Forms / Input File):**
   Project ini sudah menyertakan `WebChromeClient.onShowFileChooser` sehingga jika pengunjung membuka formulir atau upload berkas di Google Sites Anda, galeri foto dan kamera HP dapat terbuka otomatis.
