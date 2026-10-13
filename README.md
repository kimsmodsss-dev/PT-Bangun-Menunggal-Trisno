<!DOCTYPE html>
<html lang="id" class="scroll-smooth">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <!-- UBAH TEKS JUDUL WEBSITE DI SINI -->
    <title>PT. Bangun Manunggal Trisno | Kontraktor & Suplier</title>
    
    <!-- Menggunakan Tailwind CSS untuk Styling -->
    <script src="https://cdn.tailwindcss.com"></script>
    
    <!-- Menggunakan FontAwesome untuk Ikon -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <!-- Menggunakan Font Google (Inter) -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
    
    <style>
        body { font-family: 'Inter', sans-serif; }
        .fade-in { opacity: 0; transform: translateY(20px); transition: all 0.8s ease-out; }
        .fade-in.visible { opacity: 1; transform: translateY(0); }
        .bg-hero-pattern {
            /* UBAH URL GAMBAR LATAR BELAKANG (HERO) DI SINI. Rekomendasi ukuran: 1920x1080px */
            background-image: linear-gradient(rgba(10, 37, 88, 0.8), rgba(10, 37, 88, 0.8)), url('https://images.unsplash.com/photo-1541888081622-1ce0890f8450?ixlib=rb-4.0.3&auto=format&fit=crop&w=1920&q=80');
            background-size: cover;
            background-position: center;
        }
    </style>
    
    <!-- Konfigurasi Warna Khusus (Biru Tua & Biru Muda) -->
    <script>
        tailwind.config = {
            theme: {
                extend: {
                    colors: {
                        primary: '#0B2559', /* Biru Tua */
                        secondary: '#3B82F6', /* Biru Muda */
                    }
                }
            }
        }
    </script>
</head>
<body class="bg-gray-50 text-gray-800">

    <!-- ============================================== -->
    <!-- BAGIAN HEADER & NAVIGASI                       -->
    <!-- ============================================== -->
    <header id="navbar" class="fixed w-full top-0 z-50 bg-white shadow-md transition-all duration-300">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
            <div class="flex justify-between items-center h-20">
                
                <!-- UBAH LOGO PERUSAHAAN DI SINI -->
                <div class="flex-shrink-0 flex items-center gap-2">
                    <!-- Jika ingin memakai gambar logo, hapus ikon <i...> dan gunakan tag <img> di bawah ini: -->
                    <img src="WhatsApp Image 2026-10-11 at 00.49.47.png" alt="Logo PT" class="h-10 w-auto"> (Rekomendasi: 200x60px) -->
                    
                    <div class="w-10 h-10 bg-primary text-white rounded-lg flex items-center justify-center font-bold text-2xl">
                        B
                    </div>
                    <!-- UBAH NAMA PERUSAHAAN DI SINI -->
                    <span class="font-bold text-xl text-primary hidden sm:block">PT. Bangun Manunggal Trisno</span>
                </div>

                <!-- Menu Navigasi -->
                <nav class="hidden md:flex space-x-8">
                    <a href="#beranda" class="text-gray-600 hover:text-secondary font-semibold transition">Beranda</a>
                    <a href="#tentang" class="text-gray-600 hover:text-secondary font-semibold transition">Tentang Kami</a>
                    <a href="#layanan" class="text-gray-600 hover:text-secondary font-semibold transition">Layanan</a>
                    <a href="#proyek" class="text-gray-600 hover:text-secondary font-semibold transition">Proyek</a>
                    <a href="#kontak" class="text-gray-600 hover:text-secondary font-semibold transition">Kontak</a>
                </nav>

                <!-- Tombol CTA Navigasi -->
                <div class="hidden md:flex items-center">
                    <a href="https://wa.me/6281284186229" target="_blank" class="bg-secondary text-white px-6 py-2 rounded-full font-semibold hover:bg-primary transition shadow-lg">
                        Hubungi Kami
                    </a>
                </div>
            </div>
        </div>
    </header>

    <!-- ============================================== -->
    <!-- BAGIAN HERO (BERANDA)                          -->
    <!-- ============================================== -->
    <section id="beranda" class="pt-20 bg-hero-pattern min-h-screen flex items-center">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 text-center fade-in">
            <!-- UBAH TEKS HEADLINE DI SINI -->
            <h1 class="text-4xl md:text-6xl font-bold text-white mb-6 leading-tight">
                Membangun Masa Depan yang <br><span class="text-secondary">Kokoh & Terpercaya</span>
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
                <!-- UBAH JUDUL SECTION DI SINI -->
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
                    <h4 class="font-bold text-xl text-primary mb-3"><i class="fa-solid fa-eye text-secondary mr-2"></i>Visi</h4>
                    <p class="text-gray-600 mb-6">Menjadi perusahaan kontraktor dan suplier terdepan yang mengutamakan kualitas, inovasi, dan kepercayaan.</p>
                    
                    <h4 class="font-bold text-xl text-primary mb-3"><i class="fa-solid fa-bullseye text-secondary mr-2"></i>Misi</h4>
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
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl transition duration-300 transform hover:-translate-y-2 fade-in">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-building text-2xl text-secondary"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Konstruksi Bangunan & Gedung</h3>
                    <p class="text-gray-600">Pembangunan rumah tinggal, ruko, gedung perkantoran, dan fasilitas umum dari perencanaan hingga selesai.</p>
                </div>

                <!-- UBAH LAYANAN 2 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl transition duration-300 transform hover:-translate-y-2 fade-in delay-100">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-hammer text-2xl text-secondary"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Renovasi & Restorasi</h3>
                    <p class="text-gray-600">Perbaikan, perluasan, dan pembaruan struktur maupun interior bangunan agar kembali optimal.</p>
                </div>

                <!-- UBAH LAYANAN 3 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl transition duration-300 transform hover:-translate-y-2 fade-in delay-200">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-road text-2xl text-secondary"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Pekerjaan Infrastruktur & Sipil</h3>
                    <p class="text-gray-600">Pengerjaan jalan, saluran air, dan pekerjaan tanah (earthwork) untuk berbagai kebutuhan.</p>
                </div>

                <!-- UBAH LAYANAN 4 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl transition duration-300 transform hover:-translate-y-2 fade-in">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-file-signature text-2xl text-secondary"></i>
                    </div>
                    <h3 class="text-xl font-bold text-primary mb-3">Manajemen & Konsultasi</h3>
                    <p class="text-gray-600">Pengawasan, perencanaan anggaran (RAB), dan pengelolaan tata kelola proyek secara efektif.</p>
                </div>

                <!-- UBAH LAYANAN 5 DI SINI -->
                <div class="bg-white p-8 rounded-3xl shadow-md hover:shadow-2xl transition duration-300 transform hover:-translate-y-2 fade-in delay-100">
                    <div class="w-14 h-14 bg-blue-100 rounded-2xl flex items-center justify-center mb-6">
                        <i class="fa-solid fa-tractor text-2xl text-secondary"></i>
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
        <div class="absolute -left-20 -top-20 w-64 h-64 bg-secondary opacity-20 rounded-full blur-3xl"></div>
        <div class="absolute -right-20 -bottom-20 w-80 h-80 bg-secondary opacity-20 rounded-full blur-3xl"></div>
        
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
            <div class="text-center mb-16 fade-in">
                <h2 class="text-3xl font-bold mb-4">Mengapa Memilih Kami?</h2>
                <div class="w-24 h-1 bg-secondary mx-auto rounded-full"></div>
            </div>

            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 text-center">
                <!-- Keunggulan 1 -->
                <div class="p-6 fade-in">
                    <i class="fa-solid fa-user-tie text-4xl text-secondary mb-4"></i>
                    <h4 class="text-xl font-bold mb-2">Tenaga Ahli Berpengalaman</h4>
                    <p class="text-gray-300 text-sm">Dikerjakan oleh tim profesional yang berpengalaman di bidangnya.</p>
                </div>
                <!-- Keunggulan 2 -->
                <div class="p-6 fade-in delay-100">
                    <i class="fa-solid fa-shield-halved text-4xl text-secondary mb-4"></i>
                    <h4 class="text-xl font-bold mb-2">Mutu & Kualitas Terjamin</h4>
                    <p class="text-gray-300 text-sm">Menggunakan material berkualitas sesuai standar keamanan bangunan.</p>
                </div>
                <!-- Keunggulan 3 -->
                <div class="p-6 fade-in delay-200">
                    <i class="fa-solid fa-clock text-4xl text-secondary mb-4"></i>
                    <h4 class="text-xl font-bold mb-2">Tepat Waktu & Transparan</h4>
                    <p class="text-gray-300 text-sm">Perencanaan pengerjaan terstruktur dan estimasi biaya yang jelas.</p>
                </div>
                <!-- Keunggulan 4 -->
                <div class="p-6 fade-in delay-300">
                    <i class="fa-solid fa-file-contract text-4xl text-secondary mb-4"></i>
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

            <!-- GANTI FOTO PROYEK DI BAWAH INI (Rekomendasi ukuran: 800x600 px) -->
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
                <!-- Proyek 1 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in">
                    <img src="1.jpeg" alt="Proyek 1" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-0 group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pembangunan Gedung Kantor</h4>
                        <p class="text-gray-300 text-sm">Jakarta Selatan</p>
                    </div>
                </div>
                <!-- Proyek 2 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-100">
                    <img src="2.jpeg" alt="Proyek 2" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-0 group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pekerjaan Infrastruktur Jalan</h4>
                        <p class="text-gray-300 text-sm">Tangerang</p>
                    </div>
                </div>
                <!-- Proyek 3 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-200">
                    <img src="3.jpeg" alt="Proyek 3" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-0 group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Renovasi Fasilitas Umum</h4>
                        <p class="text-gray-300 text-sm">Banten</p>
                    </div>
                </div>
                <!-- Proyek 4 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in">
                    <img src="4.jpeg" alt="Proyek 4" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-0 group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pematangan Lahan (Cut & Fill)</h4>
                        <p class="text-gray-300 text-sm">Kawasan Industri</p>
                    </div>
                </div>
                <!-- Proyek 5 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-100">
                    <img src="5.jpeg" alt="Proyek 5" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-0 group-hover:opacity-100 transition duration-300">
                        <h4 class="text-white font-bold text-lg">Pembangunan Gudang</h4>
                        <p class="text-gray-300 text-sm">Cikarang</p>
                    </div>
                </div>
                <!-- Proyek 6 -->
                <div class="group relative overflow-hidden rounded-3xl shadow-lg fade-in delay-200">
                    <img src="6.jpeg" alt="Proyek 6" class="w-full h-64 object-cover transform group-hover:scale-110 transition duration-500">
                    <div class="absolute inset-0 bg-gradient-to-t from-black/80 to-transparent flex flex-col justify-end p-6 opacity-0 group-hover:opacity-100 transition duration-300">
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
            <div class="flex justify-center items-center gap-12 flex-wrap">
                <!-- GANTI FOTO LOGO KLIEN DI BAWAH INI (Rekomendasi ukuran: 200x100 px, format PNG Transparan) -->
                <img src="WhatsApp Image 2026-10-11 at 03.04.06.png" alt="Klien 1" class="h-12 grayscale hover:grayscale-0 transition duration-300">
                <img src="WhatsApp Image 2026-10-11 at 03.04.06.png" alt="Klien 2" class="h-12 grayscale hover:grayscale-0 transition duration-300">
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
                            <i class="fa-solid fa-location-dot text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Alamat Kantor</h4>
                            <p class="text-gray-600 mt-1">Jl. Green Lake City Boulevard Jl. West Europe VIII No.69, RT.001/RW.001, Ketapang, Kec. Cipondoh, Kota Tangerang, Banten 15147</p>
                        </div>
                    </div>
                    
                    <!-- UBAH NOMOR TELEPON/WA DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-phone text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Telepon / WhatsApp</h4>
                            <p class="text-gray-600 mt-1">Telp: 021-2309-6007</p>
                            <p class="text-gray-600">WA: 0812-8418-6229</p>
                        </div>
                    </div>

                    <!-- UBAH EMAIL DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-envelope text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Email</h4>
                            <p class="text-gray-600 mt-1">sutrisno.bmt@gmail.com</p>
                        </div>
                    </div>

                    <!-- UBAH JAM OPERASIONAL DI SINI -->
                    <div class="flex items-start gap-4">
                        <div class="w-12 h-12 bg-blue-50 rounded-full flex items-center justify-center flex-shrink-0 text-secondary">
                            <i class="fa-solid fa-clock text-xl"></i>
                        </div>
                        <div>
                            <h4 class="font-bold text-lg text-primary">Jam Operasional</h4>
                            <p class="text-gray-600 mt-1">Senin – Sabtu (08.00 - 17.00)</p>
                        </div>
                    </div>

                    <!-- Tombol WhatsApp Langsung -->
                    <a href="https://wa.me/6281284186229" target="_blank" class="inline-flex items-center gap-2 bg-green-500 hover:bg-green-600 text-white font-bold py-3 px-8 rounded-full transition shadow-lg mt-4">
                        <i class="fa-brands fa-whatsapp text-2xl"></i>
                        Chat WhatsApp Sekarang
                    </a>
                </div>

                <!-- Google Maps (Anda bisa mengubah link embed map dari Google Maps jika diperlukan) -->
                <div class="h-96 rounded-3xl overflow-hidden shadow-lg fade-in border border-gray-100">
                    <iframe 
                        src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1m3!1d3966.52904838647!2d106.7027376!3d-6.1936996!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x2e69f9a2baaaaaab%3A0x6b801cf9119bd236!2sGreen%20Lake%20City!5e0!3m2!1sid!2sid!4v1690000000000!5m2!1sid!2sid" 
                        width="100%" 
                        height="100%" 
                        style="border:0;" 
                        allowfullscreen="" 
                        loading="lazy" 
                        referrerpolicy="no-referrer-when-downgrade">
                    </iframe>
                </div>
            </div>
        </div>
    </section>

    <!-- ============================================== -->
    <!-- BAGIAN FOOTER                                  -->
    <!-- ============================================== -->
    <footer class="bg-primary text-gray-300 py-12 border-t border-gray-800">
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 grid grid-cols-1 md:grid-cols-3 gap-8 text-center md:text-left">
            <div>
                <!-- LOGO/NAMA FOOTER -->
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
                </ul>
            </div>
            <div>
                <h4 class="text-white font-bold text-lg mb-4">Kontak</h4>
                <p class="text-sm text-gray-400 mb-2">021-2309-6007</p>
                <p class="text-sm text-gray-400 mb-2">0812-8418-6229</p>
                <p class="text-sm text-gray-400">sutrisno.bmt@gmail.com</p>
            </div>
        </div>
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 mt-12 pt-8 border-t border-gray-700 text-center text-sm text-gray-400">
            <p>&copy; 2026 PT. Bangun Manunggal Trisno. All rights reserved.</p>
        </div>
    </footer>

    <!-- ============================================== -->
    <!-- JAVASCRIPT UNTUK ANIMASI & NAVBAR EFEK         -->
    <!-- ============================================== -->
    <script>
        // Efek transparan/putih pada Navbar saat di-scroll
        window.addEventListener('scroll', function() {
            const navbar = document.getElementById('navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('shadow-md', 'bg-white');
                navbar.classList.remove('bg-white/90', 'shadow-none');
            } else {
                navbar.classList.remove('shadow-md', 'bg-white');
                navbar.classList.add('bg-white/90', 'shadow-none');
            }
        });

        // Animasi Fade-in saat elemen muncul di layar
        const observerOptions = {
            root: null,
            rootMargin: '0px',
            threshold: 0.1
        };

        const observer = new IntersectionObserver((entries, observer) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.classList.add('visible');
                    observer.unobserve(entry.target);
                }
            });
        }, observerOptions);

        document.querySelectorAll('.fade-in').forEach(element => {
            observer.observe(element);
        });
    </script>
</body>
</html>
