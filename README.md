# Marchiano Valen Savano — CV & Portofolio

Website CV dan portofolio pribadi Marchiano Valen Savano. Situs ini memperkenalkan profil, keahlian, pendidikan, pengalaman, dan proyek yang pernah dibuat, lalu menyediakan tautan untuk menghubungi pemilik portofolio.

## Isi website

- **Beranda** — nama, peran sebagai pelajar Rekayasa Perangkat Lunak di SMKN 20 Jakarta, pengenalan singkat, foto profil, dan tautan ke bagian Tentang serta Kontak.
- **Tentang saya** — informasi singkat tentang minat pada teknologi, komunikasi, dan bahasa Inggris.
- **Keahlian** — menampilkan HTML, CSS (Tailwind), JavaScript, React (dasar), dan minat komunikasi bahasa Inggris.
- **Proyek pilihan** — menampilkan screenshot, deskripsi, teknologi yang dicantumkan, serta tautan ke website proyek:
  - **AutoEnglish** — website promosi pusat belajar bahasa Inggris untuk anak-anak, remaja, dan orang dewasa. Website proyek memperkenalkan program Calistung, AutoToddler, AutoKids, AutoTeens, dan AutoSpeak; menjelaskan metode belajar; menampilkan galeri; serta mengarahkan pengunjung ke informasi kontak dan pendaftaran. Auto AI menjawab pertanyaan umum tentang program, harga, pendaftaran, lokasi, dan keterjangkauan. Situs ini merupakan website informasi dan promosi, bukan LMS atau kelas online.
  - **EventFlow** — aplikasi untuk koordinasi acara sekolah dan komunitas. Pengguna dapat mengelola jadwal, membagi dan melacak tugas, melihat kalender pribadi, menerima notifikasi dalam aplikasi, dan secara opsional mengekspor acara ke Google Calendar. Area admin mengelola pengguna, acara, tugas, kategori, dan riwayat audit. Portofolio menampilkan screenshot desktop dan mobile.
- **Pengalaman** — kegiatan Taekwondo, partisipasi dalam lomba berbahasa Inggris, peran sebagai wakil ketua English Club, dan keanggotaan Japanese Club.
- **Pendidikan** — riwayat pendidikan dari MI Mumtaza hingga SMKN 20 Jakarta, jurusan Rekayasa Perangkat Lunak.
- **Kontak** — tautan WhatsApp, Instagram, dan LinkedIn. Bagian ini menggunakan tautan eksternal; tidak ada formulir kontak di dalam website.
- **Footer** — identitas pemilik, tahun hak cipta, dan tautan kembali ke atas.

Informasi dan tautan proyek di atas adalah konten portofolio. Fitur AutoEnglish dan EventFlow berjalan pada website proyek masing-masing, bukan sebagai fitur backend di dalam situs portofolio ini.

## Interaksi dan tampilan

- Navigasi menggunakan tautan ke bagian-bagian pada halaman yang sama.
- Pada layar sempit, navigasi berubah menjadi menu yang dapat dibuka dan ditutup; menu juga dapat ditutup dengan tombol Escape.
- Bagian halaman dianimasikan saat masuk ke area pandang menggunakan `IntersectionObserver`; jika API tersebut tidak tersedia, konten tetap ditampilkan.
- Foto profil disembunyikan jika berkas gambar tidak dapat dimuat, sehingga inisial profil tetap terlihat.
- Tata letak menyesuaikan ukuran layar dan menghormati preferensi `prefers-reduced-motion`.
- Menyediakan tautan lewati ke konten utama dan teks alternatif pada gambar.
- Menggunakan Google Fonts untuk Cormorant Garamond dan DM Sans. Jika font eksternal tidak tersedia, font pengganti dari sistem digunakan.

## Teknologi

Website portofolio ini dibuat sebagai situs statis dengan:

- HTML5
- CSS3
- JavaScript tanpa framework
- Google Fonts

Label teknologi pada kartu proyek merujuk pada teknologi proyek yang dipamerkan, bukan teknologi yang digunakan untuk membangun website portofolio.

## Menjalankan secara lokal

Tidak diperlukan instalasi package atau proses build. Jalankan server file statis dari folder proyek, misalnya dengan Python:

```powershell
py -m http.server 8080
```

Buka [http://localhost:8080](http://localhost:8080) di browser. Alternatifnya, buka `index.html` secara langsung; server lokal lebih sesuai untuk pengujian aset dan perilaku halaman.

## Struktur berkas

```text
.
├── index.html                 # Halaman utama CV dan portofolio
├── CV.html                    # Alamat alternatif yang mengarahkan ke index.html
├── style.css                  # Gaya, tata letak responsif, dan animasi
├── script.js                  # Menu, animasi saat scroll, dan penanganan foto profil
├── valen.jpeg                 # Foto profil
└── assets/
    ├── autoenglish.png        # Screenshot AutoEnglish
    ├── eventflow-desktop.png  # Screenshot desktop EventFlow
    └── eventflow-mobile.png   # Screenshot mobile EventFlow
```

Pastikan folder `assets/` dan `valen.jpeg` tetap berada pada lokasi relatif yang sama dengan `index.html` saat situs dipindahkan atau dipublikasikan.
