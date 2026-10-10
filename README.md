[index.html](https://github.com/user-attachments/files/33288547/index.html)
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>PT Bangun Manunggal Trisno | Solusi Konstruksi dan Perdagangan Umum</title>
<meta name="description" content="PT Bangun Manunggal Trisno - Mitra terpercaya solusi konstruksi dan perdagangan umum. Konstruksi bangunan, renovasi, infrastruktur, manajemen proyek, dan pematangan lahan.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700;800&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">

<style>
/* ============ VARIABEL WARNA (ubah di sini jika ingin ganti tema) ============ */
:root{
  --navy:#0f2238;
  --navy-2:#16314d;
  --yellow:#f5a623;
  --yellow-dark:#d98c0b;
  --light:#f4f6f8;
  --white:#ffffff;
  --text:#3b4756;
  --wa:#25d366;
  --radius:14px;
  --shadow:0 10px 30px rgba(15,34,56,.12);
}
*{margin:0;padding:0;box-sizing:border-box}
html{scroll-behavior:smooth;scroll-padding-top:76px}
body{font-family:'Open Sans',sans-serif;color:var(--text);line-height:1.7;background:var(--white)}
h1,h2,h3,h4{font-family:'Montserrat',sans-serif;color:var(--navy);line-height:1.25}
img{max-width:100%;display:block}
a{text-decoration:none;color:inherit}
.container{width:min(1150px,92%);margin-inline:auto}
section{padding:90px 0}

.section-head{text-align:center;max-width:680px;margin:0 auto 55px}
.section-head .tag{display:inline-block;color:var(--yellow-dark);font-weight:700;letter-spacing:2px;font-size:.8rem;text-transform:uppercase;margin-bottom:10px}
.section-head h2{font-size:clamp(1.7rem,3.5vw,2.4rem)}
.section-head .bar{width:70px;height:4px;background:var(--yellow);margin:18px auto 0;border-radius:4px}

.btn{display:inline-flex;align-items:center;gap:10px;padding:15px 30px;border-radius:50px;font-weight:700;font-family:'Montserrat',sans-serif;font-size:.95rem;border:none;cursor:pointer;transition:.3s}
.btn-wa{background:var(--wa);color:#fff;box-shadow:0 8px 22px rgba(37,211,102,.4)}
.btn-wa:hover{transform:translateY(-3px);background:#1eb957}
.btn svg{width:22px;height:22px;fill:currentColor}

/* ============ NAVBAR ============ */
header{position:fixed;top:0;left:0;width:100%;z-index:1000;transition:.3s}
header.scrolled{background:rgba(15,34,56,.97);box-shadow:0 4px 20px rgba(0,0,0,.2)}
.nav{display:flex;justify-content:space-between;align-items:center;height:76px}
.logo{display:flex;align-items:center;gap:10px;color:#fff;font-family:'Montserrat',sans-serif;font-weight:800;font-size:1.05rem}
.logo-mark{width:40px;height:40px;background:var(--yellow);color:var(--navy);display:grid;place-items:center;border-radius:10px;font-weight:800}
/* Ganti .logo-mark dengan <img src="logo.png"> jika Anda punya logo */
.menu{display:flex;gap:30px;list-style:none}
.menu a{color:#fff;font-weight:600;font-size:.92rem;position:relative;padding:6px 0}
.menu a::after{content:"";position:absolute;left:0;bottom:0;width:0;height:2px;background:var(--yellow);transition:.3s}
.menu a:hover::after,.menu a.active::after{width:100%}
.burger{display:none;background:none;border:none;cursor:pointer;width:32px;height:24px;position:relative}
.burger span{position:absolute;left:0;width:100%;height:3px;background:#fff;border-radius:3px;transition:.3s}
.burger span:nth-child(1){top:0}.burger span:nth-child(2){top:10px}.burger span:nth-child(3){top:20px}
.burger.open span:nth-child(1){top:10px;transform:rotate(45deg)}
.burger.open span:nth-child(2){opacity:0}
.burger.open span:nth-child(3){top:10px;transform:rotate(-45deg)}

/* ============ HERO ============ */
.hero{position:relative;min-height:100vh;display:flex;align-items:center;color:#fff;
  background:linear-gradient(135deg,var(--navy) 0%,var(--navy-2) 60%,#23496d 100%);overflow:hidden;padding-top:76px}
.hero-bg{position:absolute;inset:0;width:100%;height:100%;object-fit:cover}
.hero::before{content:"";position:absolute;inset:0;z-index:1;background:linear-gradient(100deg,rgba(15,34,56,.93) 25%,rgba(15,34,56,.55) 100%)}
.hero::after{content:"";position:absolute;bottom:0;left:0;width:100%;height:8px;z-index:2;
  background:repeating-linear-gradient(45deg,var(--yellow) 0 22px,var(--navy) 22px 44px)}
.hero-content{position:relative;z-index:3;max-width:720px}
.hero-badge{display:inline-block;background:rgba(245,166,35,.15);border:1px solid var(--yellow);color:var(--yellow);padding:6px 18px;border-radius:50px;font-size:.8rem;font-weight:700;letter-spacing:1.5px;margin-bottom:22px;text-transform:uppercase}
.hero h1{color:#fff;font-size:clamp(2.2rem,6vw,4rem);font-weight:800;margin-bottom:18px}
.hero h1 span{color:var(--yellow)}
.hero p{font-size:clamp(1.05rem,2.2vw,1.3rem);color:#dbe5ef;margin-bottom:36px;max-width:600px}

/* ============ ABOUT ============ */
.about{background:var(--white)}
.about-grid{display:grid;grid-template-columns:1fr 1fr;gap:60px;align-items:center}
.about-img{position:relative}
.about-img .frame{border-radius:var(--radius);overflow:hidden;box-shadow:var(--shadow);aspect-ratio:4/3;background:linear-gradient(135deg,#dfe6ee,#c5d1de);position:relative}
.about-img img{width:100%;height:100%;object-fit:cover}
.about-img::before{content:"";position:absolute;top:-18px;left:-18px;width:120px;height:120px;border:5px solid var(--yellow);border-radius:var(--radius);z-index:-1}
.about-text .tag{color:var(--yellow-dark);font-weight:700;letter-spacing:2px;font-size:.8rem;text-transform:uppercase}
.about-text h2{font-size:clamp(1.7rem,3.5vw,2.3rem);margin:10px 0 20px}
.about-text p{margin-bottom:14px;text-align:justify}

/* Placeholder untuk gambar yang belum diisi */
.ph{position:absolute;inset:0;display:grid;place-items:center;text-align:center;color:#6b7b8d;font-size:.85rem;font-weight:600;padding:10px;z-index:0}
.frame img,.g-item img{position:relative;z-index:1}

/* ============ SERVICES ============ */
.services{background:var(--light)}
.grid-services{display:grid;grid-template-columns:repeat(auto-fit,minmax(320px,1fr));gap:28px}
.card{background:#fff;border-radius:var(--radius);overflow:hidden;box-shadow:0 4px 18px rgba(15,34,56,.07);transition:.35s;display:flex;flex-direction:column;border-bottom:4px solid transparent}
.card:hover{transform:translateY(-8px);box-shadow:var(--shadow);border-bottom-color:var(--yellow)}
.card-img{height:190px;background:linear-gradient(135deg,var(--navy-2),#2b5a86);position:relative;display:grid;place-items:center;overflow:hidden}
.card-img img{position:absolute;inset:0;width:100%;height:100%;object-fit:cover;z-index:1}
.card-img .icon{width:70px;height:70px;fill:none;stroke:var(--yellow);stroke-width:1.6;stroke-linecap:round;stroke-linejoin:round}
.card-body{padding:26px}
.card-body h3{font-size:1.15rem;margin-bottom:10px}
.card-body p{font-size:.95rem}

/* ============ WHY US ============ */
.why{background:var(--navy);position:relative;overflow:hidden}
.why .section-head h2{color:#fff}
.why .section-head .tag{color:var(--yellow)}
.grid-why{display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:26px}
.why-item{background:rgba(255,255,255,.05);border:1px solid rgba(255,255,255,.1);border-radius:var(--radius);padding:34px 26px;text-align:center;transition:.3s}
.why-item:hover{background:rgba(245,166,35,.1);border-color:var(--yellow);transform:translateY(-6px)}
.why-icon{width:68px;height:68px;margin:0 auto 20px;background:var(--yellow);border-radius:50%;display:grid;place-items:center}
.why-icon svg{width:32px;height:32px;fill:none;stroke:var(--navy);stroke-width:2;stroke-linecap:round;stroke-linejoin:round}
.why-item h3{color:#fff;font-size:1.05rem;margin-bottom:10px}
.why-item p{color:#c3d0de;font-size:.92rem}

/* ============ PORTFOLIO ============ */
.gallery{display:grid;grid-template-columns:repeat(3,1fr);gap:18px}
.g-item{position:relative;border-radius:12px;overflow:hidden;aspect-ratio:4/3;cursor:pointer;background:linear-gradient(135deg,#dfe6ee,#c5d1de)}
.g-item img{width:100%;height:100%;object-fit:cover;transition:.5s}
.g-item:hover img{transform:scale(1.1)}
.g-item .overlay{position:absolute;inset:0;z-index:2;background:linear-gradient(to top,rgba(15,34,56,.85),transparent 60%);display:flex;align-items:flex-end;padding:18px;opacity:0;transition:.3s;color:#fff;font-weight:700;font-family:'Montserrat',sans-serif;font-size:.95rem}
.g-item:hover .overlay{opacity:1}
.g-item:nth-child(1),.g-item:nth-child(6){grid-column:span 2;aspect-ratio:auto}

.lightbox{position:fixed;inset:0;background:rgba(0,0,0,.9);z-index:3000;display:none;place-items:center;padding:20px}
.lightbox.show{display:grid}
.lightbox img{max-height:88vh;max-width:94vw;border-radius:10px}
.lightbox .close{position:absolute;top:18px;right:26px;color:#fff;font-size:2.6rem;cursor:pointer;line-height:1}

/* ============ CONTACT ============ */
.contact{background:var(--light)}
.contact-grid{display:grid;grid-template-columns:1fr 1.2fr;gap:40px}
.info-box{display:flex;flex-direction:column;gap:20px}
.info{display:flex;gap:18px;background:#fff;padding:22px;border-radius:var(--radius);box-shadow:0 4px 18px rgba(15,34,56,.07);align-items:flex-start}
.info-icon{flex:0 0 50px;height:50px;background:var(--navy);border-radius:12px;display:grid;place-items:center}
.info-icon svg{width:24px;height:24px;fill:none;stroke:var(--yellow);stroke-width:2;stroke-linecap:round;stroke-linejoin:round}
.info h4{font-size:1rem;margin-bottom:4px}
.info a{color:var(--navy-2);font-weight:600}
.info a:hover{color:var(--yellow-dark)}
.map{border-radius:var(--radius);overflow:hidden;box-shadow:var(--shadow);min-height:380px}
.map iframe{width:100%;height:100%;min-height:380px;border:0}

/* ============ FOOTER ============ */
footer{background:var(--navy);color:#b7c4d3;text-align:center;padding:28px 0;font-size:.9rem}
footer strong{color:#fff}

/* ============ TOMBOL WA MELAYANG ============ */
.wa-float{position:fixed;right:22px;bottom:22px;z-index:2000;display:flex;align-items:center;gap:10px;background:var(--wa);color:#fff;padding:14px 22px;border-radius:50px;font-weight:700;font-family:'Montserrat',sans-serif;font-size:.9rem;box-shadow:0 8px 25px rgba(37,211,102,.5);animation:pulse 2.2s infinite}
.wa-float svg{width:28px;height:28px;fill:#fff}
@keyframes pulse{0%{box-shadow:0 0 0 0 rgba(37,211,102,.6)}70%{box-shadow:0 0 0 18px rgba(37,211,102,0)}100%{box-shadow:0 0 0 0 rgba(37,211,102,0)}}

/* ============ ANIMASI SCROLL ============ */
.reveal{opacity:0;transform:translateY(35px);transition:.8s}
.reveal.visible{opacity:1;transform:none}

/* ============ RESPONSIVE ============ */
@media(max-width:900px){
  section{padding:70px 0}
  .about-grid,.contact-grid{grid-template-columns:1fr}
  .about-img::before{display:none}
  .gallery{grid-template-columns:repeat(2,1fr)}
  .burger{display:block}
  .menu{position:fixed;top:76px;right:-100%;width:75%;max-width:320px;height:calc(100vh - 76px);background:var(--navy);flex-direction:column;padding:35px;gap:24px;transition:.4s}
  .menu.open{right:0}
  header{background:rgba(15,34,56,.97)}
}
@media(max-width:560px){
  .gallery{grid-template-columns:1fr}
  .g-item:nth-child(1),.g-item:nth-child(6){grid-column:auto;aspect-ratio:4/3}
  .grid-services{grid-template-columns:1fr}
  .wa-float span{display:none}
  .wa-float{padding:14px}
  .btn{width:100%;justify-content:center}
}
</style>
</head>

<body>

<!-- ================= NAVBAR ================= -->
<header id="header">
  <div class="container nav">
    <a href="#home" class="logo">
      <!-- Ganti blok .logo-mark dengan: <img src="logo.png" alt="Logo" height="40"> jika sudah punya logo -->
      <span class="logo-mark">BMT</span>
      <span>PT Bangun Manunggal Trisno</span>
    </a>
    <button class="burger" id="burger" aria-label="Menu"><span></span><span></span><span></span></button>
    <ul class="menu" id="menu">
      <li><a href="#home" class="active">Beranda</a></li>
      <li><a href="#about">Tentang Kami</a></li>
      <li><a href="#services">Layanan</a></li>
      <li><a href="#why">Keunggulan</a></li>
      <li><a href="#portfolio">Portofolio</a></li>
      <li><a href="#contact">Kontak</a></li>
    </ul>
  </div>
</header>

<!-- ================= HERO ================= -->
<section class="hero" id="home">
  <!-- Masukkan file foto hero banner di sini (ganti "hero-banner.jpg" dengan nama file foto Anda) -->
  <img class="hero-bg" src="hero-banner.jpg" alt="Proyek konstruksi PT Bangun Manunggal Trisno" onerror="this.style.display='none'">
  <div class="container hero-content">
    <span class="hero-badge">Jasa Konstruksi &amp; Perdagangan Umum</span>
    <h1>PT Bangun Manunggal <span>Trisno</span></h1>
    <p>Mitra Terpercaya Solusi Konstruksi dan perdagangan umum</p>
    <a class="btn btn-wa" href="https://wa.me/6281284186229?text=Halo%20PT%20Bangun%20Manunggal%20Trisno%2C%20saya%20ingin%20konsultasi%20proyek." target="_blank" rel="noopener">
      <svg viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38a9.9 9.9 0 0 0 4.74 1.21c5.46 0 9.91-4.45 9.91-9.91S17.5 2 12.04 2zm5.8 14.12c-.25.69-1.43 1.32-1.97 1.37-.5.05-1.13.07-1.82-.11-.42-.13-.96-.31-1.65-.61-2.9-1.25-4.8-4.18-4.95-4.38-.14-.19-1.18-1.57-1.18-3s.75-2.13 1.01-2.42c.27-.29.58-.36.78-.36h.56c.18 0 .42-.07.65.5.25.6.84 2.06.91 2.21.07.15.12.32.02.51-.1.2-.15.32-.29.49l-.44.51c-.15.14-.3.3-.13.59.17.29.76 1.25 1.63 2.03 1.12 1 2.06 1.31 2.35 1.46.29.14.46.12.63-.07.17-.2.73-.85.93-1.14.19-.29.39-.24.65-.14.27.1 1.7.8 1.99.95.29.14.48.22.55.34.07.12.07.7-.18 1.39z"/></svg>
      Konsultasi Proyek (WhatsApp)
    </a>
  </div>
</section>

<!-- ================= TENTANG KAMI ================= -->
<section class="about" id="about">
  <div class="container about-grid">
    <div class="about-img reveal">
      <div class="frame">
        <div class="ph">Foto profil / kantor perusahaan<br>(tentang-kami.jpg)</div>
        <!-- Masukkan foto profil / kantor perusahaan di sini (ganti "tentang-kami.jpg") -->
        <img src="tentang-kami.jpg" alt="Kantor PT Bangun Manunggal Trisno" onerror="this.style.display='none'">
      </div>
    </div>
    <div class="about-text reveal">
      <span class="tag">Tentang Kami</span>
      <h2>Membangun dengan Komitmen dan Kualitas</h2>
      <p>PT Bangun Manunggal Trisno adalah perusahaan yang bergerak di bidang jasa konstruksi terintegrasi. Kami berkomitmen memberikan hasil pembangunan yang kokoh, aman, tepat waktu, dan berstandar mutu tinggi. Dengan didukung oleh tenaga ahli profesional dan berpengalaman, kami siap melayani berbagai kebutuhan proyek konstruksi skala kecil, menengah, hingga besar.</p>
    </div>
  </div>
</section>

<!-- ================= LAYANAN ================= -->
<section class="services" id="services">
  <div class="container">
    <div class="section-head reveal">
      <span class="tag">Layanan Kami</span>
      <h2>Solusi Konstruksi yang Lengkap</h2>
      <div class="bar"></div>
    </div>
    <div class="grid-services">

      <div class="card reveal">
        <div class="card-img">
          <!-- Foto layanan (opsional): ganti src dengan file Anda. Jika kosong, ikon akan tampil. -->
          <img src="layanan-konstruksi.jpg" alt="Konstruksi Bangunan dan Gedung" onerror="this.style.display='none'">
          <svg class="icon" viewBox="0 0 24 24"><path d="M3 21h18M5 21V7l7-4 7 4v14M9 21v-6h6v6M9 10h.01M15 10h.01"/></svg>
        </div>
        <div class="card-body">
          <h3>Konstruksi Bangunan &amp; Gedung</h3>
          <p>Pembangunan rumah tinggal, ruko, gedung perkantoran, dan fasilitas umum dari perencanaan hingga selesai.</p>
        </div>
      </div>

      <div class="card reveal">
        <div class="card-img">
          <img src="layanan-renovasi.jpg" alt="Renovasi dan Restorasi" onerror="this.style.display='none'">
          <svg class="icon" viewBox="0 0 24 24"><path d="M14.7 6.3a4 4 0 0 0-5.4 5.4L3 18v3h3l6.3-6.3a4 4 0 0 0 5.4-5.4l-2.5 2.5-2.2-.5-.5-2.2z"/></svg>
        </div>
        <div class="card-body">
          <h3>Renovasi &amp; Restorasi</h3>
          <p>Perbaikan, perluasan, dan pembaruan struktur maupun interior bangunan.</p>
        </div>
      </div>

      <div class="card reveal">
        <div class="card-img">
          <img src="layanan-infrastruktur.jpg" alt="Pekerjaan Infrastruktur dan Sipil" onerror="this.style.display='none'">
          <svg class="icon" viewBox="0 0 24 24"><path d="M4 21 9 3M20 21 15 3M12 4v3M12 11v3M12 18v3"/></svg>
        </div>
        <div class="card-body">
          <h3>Pekerjaan Infrastruktur &amp; Sipil</h3>
          <p>Pengerjaan jalan, saluran air, dan pekerjaan tanah (earthwork).</p>
        </div>
      </div>

      <div class="card reveal">
        <div class="card-img">
          <img src="layanan-manajemen.jpg" alt="Manajemen dan Konsultasi Proyek" onerror="this.style.display='none'">
          <svg class="icon" viewBox="0 0 24 24"><path d="M9 3h6a1 1 0 0 1 1 1v2H8V4a1 1 0 0 1 1-1zM8 5H6a1 1 0 0 0-1 1v14a1 1 0 0 0 1 1h12a1 1 0 0 0 1-1V6a1 1 0 0 0-1-1h-2M9 12l2 2 4-4M9 17h6"/></svg>
        </div>
        <div class="card-body">
          <h3>Manajemen &amp; Konsultasi Proyek</h3>
          <p>Pengawasan, perencanaan anggaran (RAB), dan pengelolaan tata kelola proyek secara efektif.</p>
        </div>
      </div>

      <div class="card reveal">
        <div class="card-img">
          <img src="layanan-pematangan-lahan.jpg" alt="Pematangan Lahan" onerror="this.style.display='none'">
          <svg class="icon" viewBox="0 0 24 24"><path d="M2 20h20M4 20l5-9 4 6 3-4 4 7M7 8h.01M3 14h4"/></svg>
        </div>
        <div class="card-body">
          <h3>Pematangan Lahan</h3>
          <p>Land clearing, cut and fill, compaction, dan drainase.</p>
        </div>
      </div>

    </div>
  </div>
</section>

<!-- ================= KEUNGGULAN ================= -->
<section class="why" id="why">
  <div class="container">
    <div class="section-head reveal">
      <span class="tag">Keunggulan Kami</span>
      <h2>Mengapa Memilih Kami?</h2>
      <div class="bar"></div>
    </div>
    <div class="grid-why">

      <div class="why-item reveal">
        <div class="why-icon"><svg viewBox="0 0 24 24"><circle cx="9" cy="8" r="3.5"/><path d="M2.5 20c0-3.6 2.9-6 6.5-6s6.5 2.4 6.5 6M16 4.5a3.5 3.5 0 0 1 0 7M18 14.3c2 .7 3.5 2.6 3.5 5.7"/></svg></div>
        <h3>Tenaga Ahli Berpengalaman</h3>
        <p>Dikerjakan oleh tim profesional yang berpengalaman di bidangnya.</p>
      </div>

      <div class="why-item reveal">
        <div class="why-icon"><svg viewBox="0 0 24 24"><path d="M12 2 4 5v6c0 5 3.4 9.2 8 11 4.6-1.8 8-6 8-11V5z"/><path d="m8.5 12 2.5 2.5 4.5-5"/></svg></div>
        <h3>Mutu &amp; Kualitas Terjamin</h3>
        <p>Menggunakan material berkualitas sesuai standar keamanan bangunan.</p>
      </div>

      <div class="why-item reveal">
        <div class="why-icon"><svg viewBox="0 0 24 24"><circle cx="12" cy="12" r="9"/><path d="M12 7v5l3.5 2"/></svg></div>
        <h3>Tepat Waktu &amp; Anggaran Transparan</h3>
        <p>Perencanaan pengerjaan yang terstruktur dan estimasi biaya yang jelas.</p>
      </div>

      <div class="why-item reveal">
        <div class="why-icon"><svg viewBox="0 0 24 24"><path d="M14 2H6a2 2 0 0 0-2 2v16a2 2 0 0 0 2 2h12a2 2 0 0 0 2-2V8z"/><path d="M14 2v6h6M9 14l2 2 4-4"/></svg></div>
        <h3>Legalitas Lengkap</h3>
        <p>Perusahaan resmi berbadan hukum (PT).</p>
      </div>

    </div>
  </div>
</section>

<!-- ================= PORTOFOLIO ================= -->
<section class="portfolio" id="portfolio">
  <div class="container">
    <div class="section-head reveal">
      <span class="tag">Portofolio Proyek</span>
      <h2>Hasil Karya Kami</h2>
      <div class="bar"></div>
    </div>
    <!-- Ganti nama file di src dengan foto proyek Anda. Tambah/kurangi blok .g-item sesuai kebutuhan. -->
    <div class="gallery reveal">
      <div class="g-item"><div class="ph">proyek-1.jpg</div><img src="[proyek-1.jpg](https://ibb.co/wFRzvtmh)" alt="Proyek 1" onerror="this.style.display='none'"><div class="overlay">Proyek 1</div></div>
      <div class="g-item"><div class="ph">proyek-2.jpg</div><img src="proyek-2.jpg" alt="Proyek 2" onerror="this.style.display='none'"><div class="overlay">Proyek 2</div></div>
      <div class="g-item"><div class="ph">proyek-3.jpg</div><img src="proyek-3.jpg" alt="Proyek 3" onerror="this.style.display='none'"><div class="overlay">Proyek 3</div></div>
      <div class="g-item"><div class="ph">proyek-4.jpg</div><img src="proyek-4.jpg" alt="Proyek 4" onerror="this.style.display='none'"><div class="overlay">Proyek 4</div></div>
      <div class="g-item"><div class="ph">proyek-5.jpg</div><img src="proyek-5.jpg" alt="Proyek 5" onerror="this.style.display='none'"><div class="overlay">Proyek 5</div></div>
      <div class="g-item"><div class="ph">proyek-6.jpg</div><img src="proyek-6.jpg" alt="Proyek 6" onerror="this.style.display='none'"><div class="overlay">Proyek 6</div></div>
    </div>
  </div>
</section>

<!-- Lightbox untuk memperbesar foto -->
<div class="lightbox" id="lightbox"><span class="close" id="lbClose">&times;</span><img src="" alt="Foto proyek"></div>

<!-- ================= KONTAK ================= -->
<section class="contact" id="contact">
  <div class="container">
    <div class="section-head reveal">
      <span class="tag">Kontak &amp; Lokasi</span>
      <h2>Hubungi Kami</h2>
      <div class="bar"></div>
    </div>
    <div class="contact-grid">
      <div class="info-box reveal">

        <div class="info">
          <div class="info-icon"><svg viewBox="0 0 24 24"><path d="M12 22s7-6.2 7-12a7 7 0 0 0-14 0c0 5.8 7 12 7 12z"/><circle cx="12" cy="10" r="2.5"/></svg></div>
          <div>
            <h4>Alamat Kantor</h4>
            <p>Jl. Green Lake City Boulevard Jl. West Europe VIII No.69, RT.001/RW.001, Ketapang, Kec. Cipondoh, Kota Tangerang, Banten 15147</p>
          </div>
        </div>

        <div class="info">
          <div class="info-icon"><svg viewBox="0 0 24 24"><path d="M22 16.9v3a2 2 0 0 1-2.2 2 19.8 19.8 0 0 1-8.6-3.1 19.5 19.5 0 0 1-6-6A19.8 19.8 0 0 1 2.1 4.2 2 2 0 0 1 4.1 2h3a2 2 0 0 1 2 1.7c.1 1 .4 1.9.7 2.8a2 2 0 0 1-.5 2.1L8.1 9.9a16 16 0 0 0 6 6l1.3-1.3a2 2 0 0 1 2.1-.4c.9.3 1.8.6 2.8.7a2 2 0 0 1 1.7 2z"/></svg></div>
          <div>
            <h4>Telepon</h4>
            <a href="tel:02123096007">021-2309-6007</a>
          </div>
        </div>

        <div class="info">
          <div class="info-icon"><svg viewBox="0 0 24 24"><path d="M21 11.5a8.4 8.4 0 0 1-12.3 7.4L3 21l2.1-5.5A8.4 8.4 0 1 1 21 11.5z"/></svg></div>
          <div>
            <h4>WhatsApp</h4>
            <a href="https://wa.me/6281284186229" target="_blank" rel="noopener">0812-8418-6229</a>
          </div>
        </div>

        <a class="btn btn-wa" href="https://wa.me/6281284186229?text=Halo%20PT%20Bangun%20Manunggal%20Trisno%2C%20saya%20ingin%20konsultasi%20proyek." target="_blank" rel="noopener">Chat via WhatsApp Sekarang</a>
      </div>

      <div class="map reveal">
        <iframe loading="lazy" title="Lokasi PT Bangun Manunggal Trisno"
          src="https://www.google.com/maps?q=Jl.+West+Europe+VIII+No.69,+Green+Lake+City,+Cipondoh,+Tangerang&output=embed"></iframe>
      </div>
    </div>
  </div>
</section>

<footer>
  <div class="container">
    <p>&copy; <span id="year"></span> <strong>PT Bangun Manunggal Trisno</strong>. Seluruh hak cipta dilindungi.</p>
  </div>
</footer>

<!-- ================= TOMBOL WHATSAPP MELAYANG ================= -->
<a class="wa-float" href="https://wa.me/6281284186229?text=Halo%20PT%20Bangun%20Manunggal%20Trisno%2C%20saya%20ingin%20konsultasi%20proyek." target="_blank" rel="noopener" aria-label="Chat WhatsApp">
  <svg viewBox="0 0 24 24"><path d="M12.04 2C6.58 2 2.13 6.45 2.13 11.91c0 1.75.46 3.45 1.32 4.95L2.05 22l5.25-1.38a9.9 9.9 0 0 0 4.74 1.21c5.46 0 9.91-4.45 9.91-9.91S17.5 2 12.04 2zm5.8 14.12c-.25.69-1.43 1.32-1.97 1.37-.5.05-1.13.07-1.82-.11-.42-.13-.96-.31-1.65-.61-2.9-1.25-4.8-4.18-4.95-4.38-.14-.19-1.18-1.57-1.18-3s.75-2.13 1.01-2.42c.27-.29.58-.36.78-.36h.56c.18 0 .42-.07.65.5.25.6.84 2.06.91 2.21.07.15.12.32.02.51-.1.2-.15.32-.29.49l-.44.51c-.15.14-.3.3-.13.59.17.29.76 1.25 1.63 2.03 1.12 1 2.06 1.31 2.35 1.46.29.14.46.12.63-.07.17-.2.73-.85.93-1.14.19-.29.39-.24.65-.14.27.1 1.7.8 1.99.95.29.14.48.22.55.34.07.12.07.7-.18 1.39z"/></svg>
  <span>Chat WhatsApp</span>
</a>

<script>
// Navbar: ubah gaya saat scroll
const header = document.getElementById('header');
window.addEventListener('scroll', () => header.classList.toggle('scrolled', window.scrollY > 50));

// Menu mobile
const burger = document.getElementById('burger');
const menu = document.getElementById('menu');
burger.addEventListener('click', () => { burger.classList.toggle('open'); menu.classList.toggle('open'); });
menu.querySelectorAll('a').forEach(a => a.addEventListener('click', () => { burger.classList.remove('open'); menu.classList.remove('open'); }));

// Animasi muncul saat scroll
const io = new IntersectionObserver(entries => {
  entries.forEach(e => { if (e.isIntersecting) { e.target.classList.add('visible'); io.unobserve(e.target); } });
}, { threshold: 0.12 });
document.querySelectorAll('.reveal').forEach(el => io.observe(el));

// Menu aktif sesuai bagian yang dilihat
const links = document.querySelectorAll('.menu a');
const secs = [...links].map(l => document.querySelector(l.getAttribute('href')));
window.addEventListener('scroll', () => {
  const y = window.scrollY + 120;
  secs.forEach((s, i) => { if (s && s.offsetTop <= y && s.offsetTop + s.offsetHeight > y) { links.forEach(l => l.classList.remove('active')); links[i].classList.add('active'); } });
});

// Lightbox galeri (hanya untuk foto yang berhasil dimuat)
const lb = document.getElementById('lightbox');
const lbImg = lb.querySelector('img');
document.querySelectorAll('.g-item').forEach(item => {
  item.addEventListener('click', () => {
    const img = item.querySelector('img');
    if (img && img.complete && img.naturalWidth > 0 && img.style.display !== 'none') { lbImg.src = img.src; lb.classList.add('show'); }
  });
});
lb.addEventListener('click', e => { if (e.target !== lbImg) lb.classList.remove('show'); });
document.addEventListener('keydown', e => { if (e.key === 'Escape') lb.classList.remove('show'); });

// Tahun otomatis di footer
document.getElementById('year').textContent = new Date().getFullYear();
</script>
</body>
</html>
