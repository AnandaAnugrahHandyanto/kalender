# Kalender Interaktif - Libur Nasional & Acara Pribadi

![Lisensi MIT](https://img.shields.io/badge/Lisensi-MIT-blue.svg)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS%203-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)

Sebuah aplikasi kalender berbasis web yang modern dan responsif. Dibuat dengan Vanilla JavaScript, aplikasi ini menampilkan hari libur nasional Indonesia, memungkinkan pengguna mengelola acara pribadi, dan menyertakan penanggalan Jawa (pasaran).

![Screenshot Kalender](https://github-production-user-asset-6210df.s3.amazonaws.com/168060635/477422537-2e2f83b9-3fbd-4ce0-b024-2e6a42ec8c28.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20250813%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20250813T075729Z&X-Amz-Expires=300&X-Amz-Signature=3f1fd821c66fe26e0f4cc7dade2a211ae2981f70e1f0e490ee601599c845388a&X-Amz-SignedHeaders=host)

## 🚀 Tentang Proyek

Proyek ini adalah sebuah kalender digital yang dibuat *from scratch* tanpa *framework* atau *library* eksternal. Tujuannya adalah untuk menyediakan kalender yang fungsional, mudah digunakan, dan kaya akan fitur, baik untuk kebutuhan umum maupun pribadi.

Aplikasi ini sepenuhnya *client-side* dan menyimpan semua data acara pribadi pengguna di `localStorage` peramban, sehingga tidak memerlukan *backend* atau basis data.

## ✨ Fitur Utama

-   **🗓️ Kalender Libur Nasional:** Terintegrasi langsung dengan **Google Calendar API** untuk menampilkan daftar hari libur nasional Indonesia yang selalu *up-to-date*.
-   **📝 Manajemen Acara Pribadi:** Pengguna dapat **membuat, melihat, mengubah, dan menghapus (CRUD)** acara pribadi mereka sendiri, lengkap dengan judul, deskripsi, dan waktu.
-   **💾 Penyimpanan Lokal:** Semua acara pribadi disimpan dengan aman di `localStorage` peramban, sehingga data tidak akan hilang saat halaman ditutup.
-   **KALENDERJAWA Kalender Jawa:** Menampilkan hari **Pasaran** (Legi, Pahing, Pon, Wage, Kliwon) untuk setiap tanggalnya.
-   **🎨 Tema Warna Dinamis:** Pilih dari beberapa tema warna (Biru, Hijau, Ungu) untuk menyesuaikan tampilan kalender sesuai selera.
-   **🔔 Notifikasi Pengingat:** Aktifkan pengingat untuk acara yang memiliki waktu spesifik. Aplikasi akan mengirimkan **notifikasi web** saat acara akan dimulai.
-   **📱 Desain Responsif:** Tampilan yang optimal di berbagai perangkat, mulai dari desktop hingga ponsel.
-   **🔍 Filter Tampilan:** Sembunyikan atau tampilkan kategori acara (libur nasional atau acara pribadi) sesuai kebutuhan.
-   **👆 Navigasi Intuitif:** Pindah antar bulan dengan mudah menggunakan tombol atau *swipe* (geser) pada perangkat sentuh.

## 🛠️ Teknologi yang Digunakan

-   **Frontend:** HTML5, CSS3 (Flexbox, Grid, Custom Variables), JavaScript (ES6+)
-   **API Eksternal:**
    -   [Google Calendar API](https://developers.google.com/calendar) untuk data hari libur.
    -   [Web Storage API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Storage_API) (`localStorage`) untuk data acara.
    -   [Notifications API](https://developer.mozilla.org/en-US/docs/Web/API/Notifications_API) untuk sistem pengingat.

## ⚙️ Instalasi & Penggunaan

Proyek ini tidak memerlukan proses instalasi atau *build* yang rumit. Cukup ikuti langkah-langkah berikut:

1.  **Clone repositori ini:**
    ```bash
    git clone https://github.com/AnandaAnugrahHandyanto/kalender.git
    ```
2.  **Buka file `index.html`:**
    Navigasikan ke direktori proyek dan buka file `index.html` langsung di peramban web pilihan Anda (misalnya: Google Chrome, Mozilla Firefox).

### Konfigurasi Kunci API

Proyek ini menggunakan Google Calendar API untuk data hari libur. Jika data tidak muncul, kemungkinan besar kunci API yang ada di dalam kode sudah tidak aktif atau dibatasi.

Anda bisa menggantinya dengan kunci API Anda sendiri:
1.  Dapatkan kunci API dari [Google Cloud Console](https://console.cloud.google.com/).
2.  Buka file `index.html` dan cari baris berikut di dalam tag `<script>`:
    ```javascript
    const apiKey = "AIzaSyCHdJfqVSd-1rQ1wbbp7uaJwk9Ty2iWRAE"; 
    ```
3.  Ganti nilai `apiKey` dengan kunci API milik Anda.

## 🤝 Berkontribusi

Kontribusi Anda sangat kami hargai! Jika Anda ingin berkontribusi, silakan lakukan *fork* pada repositori ini dan buat *pull request* dengan perubahan yang Anda usulkan.

1.  Fork repositori ini.
2.  Buat *branch* baru (`git checkout -b fitur/NamaFiturBaru`).
3.  *Commit* perubahan Anda (`git commit -m 'fitur: Menambahkan NamaFiturBaru'`).
4.  *Push* ke *branch* Anda (`git push origin fitur/NamaFiturBaru`).
5.  Buka *Pull Request*.

## 📄 Lisensi

Proyek ini didistribusikan di bawah Lisensi MIT. Lihat file `LICENSE` untuk informasi lebih lanjut (jika ada) atau kunjungi [MIT License](https://opensource.org/licenses/MIT).