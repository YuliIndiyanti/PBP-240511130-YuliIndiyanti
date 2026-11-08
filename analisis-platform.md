# Analisis Komparatif Platform: Web, Desktop, dan Mobile

- **Mata Kuliah:** Pemrograman Berbasis Platform
- **Pertemuan:** 1 (Setup Environment & Eksplorasi Platform)
- **Nama Mahasiswa:** Yuli Indiyanti
- **NIM:** 240511130
- **Program Studi:** S1 Teknik Informatika - Universitas Muhammadiyah Cirebon

---

## Tabel Analisis Platform

| Aspek | Web | Desktop | Mobile |
| :--- | :--- | :--- | :--- |
| **Arsitektur** | **Client-Server Architecture:**<br>- Terbagi atas Front-End (Client) yang dieksekusi di web browser dan Back-End (Server) penyedia data/logika bisnis.<br>- Pola umum: Single Page Application (SPA), Multi-Page Application (MPA), Server-Side Rendering (SSR). | **Stand-alone / Client Architecture (Event-Driven):**<br>- Terinstal dan dieksekusi langsung di atas sistem operasi lokal (OS runtime Win32/macOS/Linux).<br>- Akses langsung memori & periferal (Fat-Client), opsional terhubung API remote. | **Sandboxed Mobile Client Architecture (Event-Driven):**<br>- Berbasis *Application Lifecycle* ketat (Foreground, Background, Suspended).<br>- Berjalan di dalam lingkungan terisolasi (*sandbox*) demi keamanan OS & baterai. |
| **Bahasa Utama** | HTML5, CSS3, JavaScript, TypeScript, WebAssembly (Wasm). Backend: Node.js, Python, PHP, Java, Go. | Java (JavaFX, Swing), C# (.NET / WPF), C++, Python, Rust, Swift (macOS). | Kotlin / Java (Android), Swift / Objective-C (iOS), Dart (Flutter), JavaScript/TypeScript (React Native). |
| **Distribusi** | Web Server / Cloud Hosting via protokol HTTP/HTTPS & CDN. Pengguna mengakses instan melalui URL browser tanpa proses instalasi (*zero-installation*). | File installer executable (`.exe`, `.msi`, `.dmg`, `.deb`, `.rpm`) atau melalui Desktop Store (Microsoft Store, Mac App Store). | Toko aplikasi resmi (*Google Play Store*, *Apple App Store*) dengan format paket `.apk`/`.aab` (Android) atau `.ipa` (iOS). |
| **Keunggulan** | 1. Akses mudah lintas perangkat tanpa instalasi.<br>2. Update aplikasi terpusat secara real-time di server.<br>3. Pemeliharaan efisien dan kompatibel multi-OS. | 1. Performa sangat tinggi dengan akses komputasi CPU/GPU native.<br>2. Dapat beroperasi penuh tanpa koneksi internet (*offline-first*).<br>3. Akses hardware menyeluruh (storage, port USB, driver spesifik). | 1. Portabilitas tinggi, selalu menyertai mobilitas pengguna.<br>2. Akses kaya sensor perangkat (GPS, Kamera, Akselerometer, Biometrik).<br>3. Kemampuan interaksi real-time (*Push Notification*). |
| **Keterbatasan** | 1. Akses hardware dibatasi oleh *browser security sandbox*.<br>2. Kinerja komputasi berat grafis/3D lebih terbatas dibanding native.<br>3. Sangat bergantung pada ketersediaan koneksi internet. | 1. Harus disesuaikan dengan arsitektur & dependensi masing-masing OS.<br>2. Distribusi & update versi baru memerlukan instalasi ulang oleh pengguna.<br>3. Tidak portabel untuk perangkat bergerak. | 1. Sumber daya perangkat terbatas (baterai, kapasitas memori, daya prosesor).<br>2. Proses rilis terikat regulasi dan kurasi ketat toko aplikasi.<br>3. Fragmentasi perangkat keras dan resolusi layar yang beragam. |
| **Contoh Aplikasi** | Tokopedia, Facebook, Gmail, Spotify Web Player, Google Docs | Visual Studio Code, Adobe Photoshop, Spotify Desktop, Blender, IntelliJ IDEA | WhatsApp, Gojek, Instagram, Google Maps, Mobile Banking |

---

## Kesimpulan
Setiap platform dirancang untuk memenuhi kebutuhan komputasi dan skenario penggunaan yang berbeda:
1. **Web Platform** sangat ideal untuk layanan informasi dan transaksi yang memprioritaskan kemudahan akses dan jangkauan luas tanpa instalasi.
2. **Desktop Platform** sangat cocok untuk aplikasi profesional dengan tuntutan komputasi intensif, manipulasi file lokal, dan kinerja perangkat keras maksimal.
3. **Mobile Platform** unggul dalam portabilitas dan personalisasi pengguna dengan memanfaatkan sensor fisik dan konektivitas seluler.
