[index (5).html](https://github.com/user-attachments/files/33395835/index.5.html)
<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- UBAH TEKS JUDUL WEBSITE DI SINI -->
    <title>PT. Bangun Manunggal Trisno | Kontraktor &amp; Suplier</title>
    <meta name="description" content="PT. Bangun Manunggal Trisno - jasa kontraktor dan suplier profesional untuk konstruksi gedung, renovasi, infrastruktur, dan pematangan lahan di Tangerang dan sekitarnya.">
    <meta name="theme-color" content="#0B2559">
    <!-- Favicon sederhana (huruf B). Ganti dengan file logo Anda jika ada -->
    <link rel="icon" href="data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 100 100'%3E%3Crect width='100' height='100' rx='20' fill='%230B2559'/%3E%3Ctext x='50' y='70' font-size='64' font-family='Arial' font-weight='bold' text-anchor='middle' fill='white'%3EB%3C/text%3E%3C/svg%3E">

    <!-- Tailwind CSS -->
    <script src="https://cdn.tailwindcss.com"></script>

    <!-- FontAwesome untuk ikon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <!-- Font Google (Inter) -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">

    <!-- Konfigurasi Warna Khusus (Biru Tua & Biru Muda) -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#0B2559',   /* Biru Tua */
                        secondary: '#3B82F6', /* Biru Muda */
                    }
                }
            }
        }
    </script>

    <style>
        html { scroll-padding-top: 5rem; } /* agar judul section tidak tertutup navbar saat klik menu */
        body { font-family: 'Inter', sans-serif; }

        /* Animasi muncul. Memakai properti "translate" (bukan "transform")
           supaya tidak bentrok dengan efek hover kartu. */
        .fade-in {
            opacity: 0;
            translate: 0 20px;
            transition: opacity .8s ease-out var(--d, 0s), translate .8s ease-out var(--d, 0s),
                        transform .3s ease-out, box-shadow .3s ease-out;
        }
        .fade-in.visible { opacity: 1; translate: 0 0; }
        .delay-100 { --d: .1s; }
        .delay-200 { --d: .2s; }
        .delay-300 { --d: .3s; }

        .card-hover:hover { transform: translateY(-8px); }

        .bg-hero-pattern {
            /* UBAH URL GAMBAR LATAR BELAKANG (HERO) DI SINI. Rekomendasi ukuran: 1920x1080px */
            background-color: #0B2559;
            background-image: linear-gradient(rgba(10, 37, 88, 0.8), rgba(10, 37, 88, 0.8)), url('https://images.unsplash.com/photo-1541888081622-1ce0890f8450?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
        }

        /* Hormati pengguna yang mematikan animasi, dan tampilkan konten jika JS mati */
        @media (prefers-reduced-motion: reduce) {
            .fade-in { opacity: 1; translate: 0 0; transition: none; }
            html { scroll-behavior: auto; }
        }
    </style>
    <noscript><style>.fade-in { opacity: 1; translate: 0 0; }</style></noscript>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- ============================================== -->
    <!-- BAGIAN HEADER & NAVIGASI                       -->
    <!-- ============================================== -->
    <header id="navbar" class="fixed w-full top-0 z-50 bg-white shadow-sm transition-shadow duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">

                <!-- UBAH LOGO PERUSAHAAN DI SINI -->
                <a href="#beranda" class="flex-shrink-0 flex items-center gap-2" aria-label="PT. Bangun Manunggal Trisno - ke Beranda">
                    <!-- Logo: ganti nama file di src di bawah. Jika file tidak ditemukan, otomatis tampil kotak "B". -->
                    <img src="WhatsApp%20Image%202026-10-11%20at%2000.49.47.png" alt="Logo PT. Bangun Manunggal Trisno" class="h-10 w-auto"
                         onerror="this.style.display='none';this.nextElementSibling.style.display='flex'">
                    <div class="w-10 h-10 bg-primary text-white rounded-lg items-center justify-center font-bold text-2xl" style="display:none">B</div>
                    <!-- UBAH NAMA PERUSAHAAN DI SINI -->
                    <span class="font-bold text-lg sm:text-xl text-primary">
                        <span class="hidden sm:inline">PT. Bangun Manunggal Trisno</span>
                        <span class="sm:hidden">PT. BMT</span>
                    </span>
                </a>

                <!-- Menu Navigasi (Desktop) -->
                <nav class="hidden md:flex space-x-8" aria-label="Navigasi utama">
                    <a href="#beranda" class="text-gray-600 hover:text-secondary font-semibold transition">Beranda</a>
                    <a href="#tentang" class="text-gray-600 hover:text-secondary font-semibold transition">Tentang Kami</a>
                    <a href="#layanan" class="text-gray-600 hover:text-secondary font-semibold transition">Layanan</a>
                    <a href="#proyek" class="text-gray-600 hover:text-secondary font-semibold transition">Proyek</a>
                    <a href="#kontak" class="text-gray-600 hover:text-secondary font-semibold transition">Kontak</a>
                </nav>

                <!-- Tombol CTA Navigasi (Desktop) -->
                <div class="hidden md:flex items-center">
                    <a href="https://wa.me/6281284186229?text=Halo%20PT.%20Bangun%20Manunggal%20Trisno%2C%20saya%20ingin%20berkonsultasi." target="_blank" rel="noopener noreferrer" class="bg-secondary text-white px-6 py-2 rounded-full font-semibold hover:bg-primary transition shadow-lg">
                        Hubungi Kami
                    </a>
                </div>

                <!-- Tombol Menu (Mobile) -->
                <button id="menu-btn" type="button" class="md:hidden w-10 h-10 flex items-center justify-center rounded-lg text-primary hover:bg-gray-100 transition" aria-label="Buka menu" aria-expanded="false" aria-controls="mobile-menu">
                    <i id="menu-icon" class="fa-solid fa-bars text-xl"></i>
                </button>
            </div>
        </div>

        <!-- Menu Mobile -->
        <div id="mobile-menu" class="hidden md:hidden bg-white border-t border-gray-100 shadow-lg">
            <nav class="max-w-7xl mx-auto px-4 py-4 flex flex-col gap-1" aria-label="Navigasi seluler">
                <a href="#beranda" class="px-3 py-3 rounded-lg text-gray-700 font-semibold hover:bg-blue-50 hover:text-secondary transition">Beranda</a>
                <a href="#tentang" class="px-3 py-3 rounded-lg text-gray-700 font-semibold hover:bg-blue-50 hover:text-secondary transition">Tentang Kami</a>
                <a href="#layanan" class="px-3 py-3 rounded-lg text-gray-700 font-semibold hover:bg-blue-50 hover:text-secondary transition">Layanan</a>
                <a href="#proyek" class="px-3 py-3 rounded-lg text-gray-700 font-semibold hover:bg-blue-50 hover:text-secondary transition">Proyek</a>
                <a href="#kontak" class="px-3 py-3 rounded-lg text-gray-700 font-semibold hover:bg-blue-50 hover:text-secondary transition">Kontak</a>
                <a href="https://wa.me/6281284186229?text=Halo%20PT.%20Bangun%20Manunggal%20Trisno%2C%20saya%20ingin%20berkonsultasi." target="_blank" rel="noopener noreferrer" class="mt-2 text-center bg-secondary text-white px-6 py-3 rounded-full font-semibold hover:bg-primary transition">
                    Hubungi Kami
                </a>
            </nav>
        </div>
    </header>

    <main>
    <!-- ============================================== -->
    <!-- BAGIAN HERO (BERANDA)                          -->
    <!-- ============================================== -->
    <section id="beranda" class="pt-20 bg-hero-pattern min-h-screen flex items-center">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center fade-in">
            <!-- UBAH TEKS HEADLINE DI SINI -->
            <h1 class="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">
                Membangun Masa Depan yang <br class="hidden sm:block"><span class="text-secondary">Kokoh &amp; Terpercaya</span>
            </h1>
            <!-- UBAH TEKS SUB-HEADLINE DI SINI -->
            <p class="text-lg md:text-2xl text-gray-200 mb-10 max-w-3xl mx-auto">
                Solusi terbaik untuk jasa kontraktor dan penyediaan material proyek Anda secara profesional dan tepat waktu.
            </p>
            <a href="#layanan" class="bg-white text-primary px-8 py-3 rounded-full font-bold text-lg hover:bg-gray-100 transition shadow-xl inline-block">
                Lihat Layanan Kami
            </a>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN TENTANG KAMI                            -->
    <!-- ============================================== -->
    <section id="tentang" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-12 fade-in">
                <h2 class="text-3xl font-bold text-primary mb-4">Tentang Kami</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 gap-12 items-center fade-in">
                <div>
                    <!-- UBAH DESKRIPSI TENTANG KAMI DI SINI -->
                    <h3 class="text-2xl font-bold mb-4 text-gray-800">Mitra Terpercaya Konstruksi Anda</h3>
                    <p class="text-gray-600 leading-relaxed mb-6">
                        PT. Bangun Manunggal Trisno adalah perusahaan yang bergerak di bidang jasa kontraktor dan suplier profesional. Kami berkomitmen memberikan hasil terbaik dengan standar kualitas tinggi untuk setiap proyek pembangunan, renovasi, hingga infrastruktur Anda.
                    </p>
                </div>
                <!-- BAGIAN VISI MISI -->
                <div class="bg-blue-50 p-8 rounded-3xl shadow-sm border border-blue-100 relative overflow-hidden">
                    <div class="absolute -right-10 -top-10 w-32 h-32 bg-secondary opacity-10 rounded-full"></div>
                    <!-- UBAH VISI & MISI DI SINI -->
                    <h4 class="font-bold text-xl text-primary mb-3"><i class="fa-solid fa-eye text-secondary mr-2" aria-hidden="true"></i>Visi</h4>
                    <p class="text-gray-600 mb-6">Menjadi perusahaan kontraktor dan suplier terdepan yang mengutamakan kualitas, inovasi, dan kepercayaan.</p>

                    <h4 class="font-bold text-xl text-primary mb-3"><i class="fa-solid fa-bullseye text-secondary mr-2" aria-hidden="true"></i>Misi</h4>
                    <ul class="text-gray-600 list-disc list-inside space-y-2">
                        <li>Memberikan layanan tepat waktu dan berkualitas.</li>
                        <li>Menggunakan material terbaik sesuai standar.</li>
                        <li>Mengedepankan profesionalitas dan transparansi.</li>
                    </ul>
                </div>
            </div>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN LAYANAN KAMI                            -->
    <!-- ============================================== -->
    <section id="layanan" class="py-20 bg-gray-50">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl font-bold text-primary mb-4">Layanan Kami</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">

                <!-- UBAH LAYANAN 1 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl card-hover fade-in">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-building text-2xl text-secondary" aria-hidden="true"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Konstruksi Bangunan &amp; Gedung</h3>
                    <p class="text-gray-600">Pembangunan rumah tinggal, ruko, gedung perkantoran, dan fasilitas umum dari perencanaan hingga selesai.</p>
                </div>

                <!-- UBAH LAYANAN 2 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl card-hover fade-in delay-100">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-hammer text-2xl text-secondary" aria-hidden="true"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Renovasi &amp; Restorasi</h3>
                    <p class="text-gray-600">Perbaikan, perluasan, dan pembaruan struktur maupun interior bangunan agar kembali optimal.</p>
                </div>

                <!-- UBAH LAYANAN 3 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl card-hover fade-in delay-200">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-road text-2xl text-secondary" aria-hidden="true"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Pekerjaan Infrastruktur &amp; Sipil</h3>
                    <p class="text-gray-600">Pengerjaan jalan, saluran air, dan pekerjaan tanah (earthwork) untuk berbagai kebutuhan.</p>
                </div>

                <!-- UBAH LAYANAN 4 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl card-hover fade-in">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-file-signature text-2xl text-secondary" aria-hidden="true"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Manajemen &amp; Konsultasi</h3>
                    <p class="text-gray-600">Pengawasan, perencanaan anggaran (RAB), dan pengelolaan tata kelola proyek secara efektif.</p>
                </div>

                <!-- UBAH LAYANAN 5 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl card-hover fade-in delay-100">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-tractor text-2xl text-secondary" aria-hidden="true"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Pematangan Lahan</h3>
                    <p class="text-gray-600">Layanan land clearing, cut and fill, pemadatan (compaction), dan pembuatan sistem drainase.</p>
                </div>

            </div>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN KEUNGGULAN (MENGAPA MEMILIH KAMI)       -->
    <!-- ============================================== -->
    <section class="py-20 bg-primary text-white relative overflow-hidden">
        <!-- Dekorasi geometris background -->
        <div class="absolute -left-20 -top-20 w-64 h-64 bg-secondary opacity-20 rounded-full blur-3xl" aria-hidden="true"></div>
        <div class="absolute -right-20 -bottom-20 w-80 h-80 bg-secondary opacity-20 rounded-full blur-3xl" aria-hidden="true"></div>

        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl font-bold mb-4">Mengapa Memilih Kami?</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 text-center">
                <div class="p-6 fade-in">
                    <i class="fa-solid fa-user-tie text-4xl text-secondary mb-4" aria-hidden="true"></i>
                    <h4 class="text-xl font-bold mb-2">Tenaga Ahli Berpengalaman</h4>
                    <p class="text-gray-300 text-sm">Dikerjakan oleh tim profesional yang berpengalaman di bidangnya.</p>
                </div>
                <div class="p-6 fade-in delay-100">
                    <i class="fa-solid fa-shield-halved text-4xl text-secondary mb-4" aria-hidden="true"></i>
                    <h4 class="text-xl font-bold mb-2">Mutu &amp; Kualitas Terjamin</h4>
                    <p class="text-gray-300 text-sm">Menggunakan material berkualitas sesuai standar keamanan bangunan.</p>
                </div>
                <div class="p-6 fade-in delay-200">
                    <i class="fa-solid fa-clock text-4xl text-secondary mb-4" aria-hidden="true"></i>
                    <h4 class="text-xl font-bold mb-2">Tepat Waktu &amp; Transparan</h4>
                    <p class="text-gray-300 text-sm">Perencanaan pengerjaan terstruktur dan estimasi biaya yang jelas.</p>
                </div>
                <div class="p-6 fade-in delay-300">
                    <i class="fa-solid fa-file-contract text-4xl text-secondary mb-4" aria-hidden="true"></i>
                    <h4 class="text-xl font-bold mb-2">Legalitas Lengkap</h4>
                    <p class="text-gray-300 text-sm">Perusahaan resmi dan berbadan hukum (PT) yang dapat dipercaya.</p>
                </div>
            </div>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN PORTOFOLIO PROYEK                       -->
    <!-- ============================================== -->
    <section id="proyek" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl font-bold text-primary mb-4">Portofolio Proyek Kami</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
            </div>

            <!-- GANTI FOTO PROYEK DI BAWAH INI (Rekomendasi ukuran: 800x600 px).
                 Caption selalu terlihat di HP/tablet, dan muncul saat hover di layar besar. -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Proyek 1 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in">
                    <img src="1.jpeg" alt="Pembangunan gedung kantor" loading="lazy" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-100 lg:opacity-0 lg:group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pembangunan Gedung Kantor</h4>
                        <p class="text-gray-300 text-sm">Jakarta Selatan</p>
                    </div>
                </div>
                <!-- Proyek 2 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-100">
                    <img src="2.jpeg" alt="Pekerjaan infrastruktur jalan" loading="lazy" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-100 lg:opacity-0 lg:group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pekerjaan Infrastruktur Jalan</h4>
                        <p class="text-gray-300 text-sm">Tangerang</p>
                    </div>
                </div>
                <!-- Proyek 3 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-200">
                    <img src="3.jpeg" alt="Renovasi fasilitas umum" loading="lazy" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-100 lg:opacity-0 lg:group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Renovasi Fasilitas Umum</h4>
                        <p class="text-gray-300 text-sm">Banten</p>
                    </div>
                </div>
                <!-- Proyek 4 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in">
                    <img src="4.jpeg" alt="Pematangan lahan cut and fill" loading="lazy" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-100 lg:opacity-0 lg:group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pematangan Lahan (Cut &amp; Fill)</h4>
                        <p class="text-gray-300 text-sm">Kawasan Industri</p>
                    </div>
                </div>
                <!-- Proyek 5 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-100">
                    <img src="5.jpeg" alt="Pembangunan gudang" loading="lazy" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-100 lg:opacity-0 lg:group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pembangunan Gudang</h4>
                        <p class="text-gray-300 text-sm">Cikarang</p>
                    </div>
                </div>
                <!-- Proyek 6 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-200">
                    <img src="6.jpeg" alt="Perumahan cluster" loading="lazy" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-100 lg:opacity-0 lg:group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Perumahan Cluster</h4>
                        <p class="text-gray-300 text-sm">Depok</p>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN KLIEN / MITRA                           -->
    <!-- ============================================== -->
    <section class="py-12 bg-gray-50 border-y border-gray-200">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center fade-in">
            <h3 class="text-gray-500 font-semibold mb-8 uppercase tracking-wider text-sm">Telah Dipercaya Oleh</h3>
            <!-- GANTI LOGO KLIEN DI BAWAH INI (satu logo, ukuran besar seperti kartu portofolio) -->
            <div class="group max-w-md mx-auto bg-white rounded-3xl shadow-lg overflow-hidden">
                <img src="WhatsApp%20Image%202026-10-11%20at%2003.04.06.png" alt="Logo klien" loading="lazy" class="w-full h-64 object-contain p-6 transform group-hover:scale-105 transition duration-500">
            </div>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN KONTAK & MAPS                           -->
    <!-- ============================================== -->
    <section id="kontak" class="py-20 bg-white">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl font-bold text-primary mb-4">Hubungi Kami</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 lg:grid-cols-2 gap-12">
                <!-- Informasi Kontak -->
                <div class="space-y-8 fade-in">
                    <!-- UBAH ALAMAT DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-location-dot text-xl" aria-hidden="true"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Alamat Kantor</h4>
                            <p class="text-gray-600 mt-1">Jl. Green Lake City Boulevard, Jl. West Europe VIII No.69, RT.001/RW.001, Ketapang, Kec. Cipondoh, Kota Tangerang, Banten 15147</p>
                        </div>
                    </div>

                    <!-- UBAH NOMOR TELEPON/WA DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-phone text-xl" aria-hidden="true"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Telepon / WhatsApp</h4>
                            <p class="text-gray-600 mt-1">Telp: <a href="tel:+622123096007" class="hover:text-secondary transition">021-2309-6007</a></p>
                            <p class="text-gray-600">WA: <a href="https://wa.me/6281284186229" target="_blank" rel="noopener noreferrer" class="hover:text-secondary transition">0812-8418-6229</a></p>
                        </div>
                    </div>

                    <!-- UBAH EMAIL DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-envelope text-xl" aria-hidden="true"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Email</h4>
                            <p class="text-gray-600 mt-1 break-all"><a href="mailto:sutrisno.bmt@gmail.com" class="hover:text-secondary transition">sutrisno.bmt@gmail.com</a></p>
                        </div>
                    </div>

                    <!-- UBAH JAM OPERASIONAL DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-clock text-xl" aria-hidden="true"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Jam Operasional</h4>
                            <p class="text-gray-600 mt-1">Senin – Sabtu (08.00 - 17.00)</p>
                        </div>
                    </div>

                    <!-- Tombol WhatsApp Langsung -->
                    <a href="https://wa.me/6281284186229?text=Halo%20PT.%20Bangun%20Manunggal%20Trisno%2C%20saya%20ingin%20berkonsultasi." target="_blank" rel="noopener noreferrer" class="inline-flex items-center gap-2 bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-8 rounded-full transition shadow-lg mt-4">
                        <i class="fa-brands fa-whatsapp text-2xl" aria-hidden="true"></i>
                        Chat WhatsApp Sekarang
                    </a>
                </div>

                <!-- Google Maps (ubah isi q= di URL untuk mengganti lokasi) -->
                <div class="h-96 rounded-3xl overflow-hidden shadow-lg fade-in border border-gray-100">
                    <iframe
                        title="Lokasi kantor PT. Bangun Manunggal Trisno"
                        src="https://maps.google.com/maps?q=Jl.%20West%20Europe%20VIII%20No.69%2C%20Green%20Lake%20City%2C%20Cipondoh%2C%20Tangerang&amp;hl=id&amp;z=16&amp;output=embed"
                        width="100%"
                        height="100%"
                        style="border:0;"
                        allowfullscreen
                        loading="lazy"
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </div>
        </div>
    </section>
    </main>

    <!-- ============================================== -->
    <!-- BAGIAN FOOTER                                  -->
    <!-- ============================================== -->
    <footer class="bg-primary text-gray-300 py-12">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-3 gap-8 text-center md:text-left">
            <div>
                <h4 class="text-white font-bold text-2xl mb-4">PT. Bangun Manunggal Trisno</h4>
                <p class="text-sm text-gray-400">Penyedia jasa kontraktor dan suplier terpercaya untuk kebutuhan proyek infrastruktur dan bangunan Anda.</p>
            </div>
            <div>
                <h4 class="text-white font-bold text-lg mb-4">Tautan Cepat</h4>
                <ul class="space-y-2 text-sm">
                    <li><a href="#beranda" class="hover:text-secondary transition">Beranda</a></li>
                    <li><a href="#tentang" class="hover:text-secondary transition">Tentang Kami</a></li>
                    <li><a href="#layanan" class="hover:text-secondary transition">Layanan Kami</a></li>
                    <li><a href="#proyek" class="hover:text-secondary transition">Portofolio Proyek</a></li>
                    <li><a href="#kontak" class="hover:text-secondary transition">Kontak</a></li>
                </ul>
            </div>
            <div>
                <h4 class="text-white font-bold text-lg mb-4">Kontak</h4>
                <p class="text-sm text-gray-400 mb-2"><a href="tel:+622123096007" class="hover:text-secondary transition">021-2309-6007</a></p>
                <p class="text-sm text-gray-400 mb-2"><a href="https://wa.me/6281284186229" target="_blank" rel="noopener noreferrer" class="hover:text-secondary transition">0812-8418-6229</a></p>
                <p class="text-sm text-gray-400 break-all"><a href="mailto:sutrisno.bmt@gmail.com" class="hover:text-secondary transition">sutrisno.bmt@gmail.com</a></p>
            </div>
        </div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mt-12 pt-8 border-t border-gray-700 text-center text-sm text-gray-400">
            <p>&copy; 2026 PT. Bangun Manunggal Trisno. All rights reserved.</p>
        </div>
    </footer>

    <!-- ============================================== -->
    <!-- JAVASCRIPT: NAVBAR, MENU MOBILE & ANIMASI      -->
    <!-- ============================================== -->
    <script>
        // Bayangan navbar menebal saat halaman di-scroll
        const navbar = document.getElementById('navbar');
        function onScroll() {
            const scrolled = window.scrollY > 50;
            navbar.classList.toggle('shadow-md', scrolled);
            navbar.classList.toggle('shadow-sm', !scrolled);
        }
        window.addEventListener('scroll', onScroll, { passive: true });
        onScroll();

        // Menu mobile (buka/tutup)
        const menuBtn = document.getElementById('menu-btn');
        const menu = document.getElementById('mobile-menu');
        const menuIcon = document.getElementById('menu-icon');
        function setMenu(open) {
            menu.classList.toggle('hidden', !open);
            menuBtn.setAttribute('aria-expanded', String(open));
            menuBtn.setAttribute('aria-label', open ? 'Tutup menu' : 'Buka menu');
            menuIcon.classList.toggle('fa-bars', !open);
            menuIcon.classList.toggle('fa-xmark', open);
        }
        menuBtn.addEventListener('click', () => setMenu(menu.classList.contains('hidden')));
        menu.querySelectorAll('a').forEach(a => a.addEventListener('click', () => setMenu(false)));
        window.addEventListener('resize', () => { if (window.innerWidth >= 768) setMenu(false); });

        // Animasi fade-in saat elemen muncul di layar
        const observer = new IntersectionObserver((entries, obs) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    obs.unobserve(entry.target);
                }
            });
        }, { threshold: 0.1 });

        document.querySelectorAll('.fade-in').forEach(el => observer.observe(el));
    </script>
</body>
</html>
