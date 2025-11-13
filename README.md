<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>CV KILAT — Jasa Pembuatan CV Profesional</title>
  <meta name="description" content="CV KILAT | Jasa pembuatan CV profesional, ATS-friendly, untuk pelamar kerja." />
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#ffffff; --muted:#6b7280; --accent:#0f172a; --primary:#0b69ff; --soft:#f3f6fb;
      --radius:12px; --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0; font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background:var(--bg); color:var(--accent); -webkit-font-smoothing:antialiased; -moz-osx-font-smoothing:grayscale;
      line-height:1.5;
    }
    a{color:inherit; text-decoration:none}
    .container{max-width:var(--maxw); margin:0 auto; padding:28px}

    /* Navbar */
    .nav{display:flex; align-items:center; justify-content:space-between; gap:16px; position:sticky; top:0; background:rgba(255,255,255,0.8); backdrop-filter:blur(6px); padding:12px 0; border-bottom:1px solid #eef2f7; z-index:40}
    .brand{display:flex; align-items:center; gap:12px}
    .logo{width:44px; height:44px; border-radius:10px; background:linear-gradient(135deg,var(--primary),#0b8cff); display:flex; align-items:center; justify-content:center; color:white; font-weight:700}
    .nav-links{display:flex; gap:18px; align-items:center}
    .btn{display:inline-flex; align-items:center; gap:8px; padding:10px 14px; border-radius:10px; font-weight:600}
    .btn-cta{background:var(--primary); color:white; box-shadow:0 6px 18px rgba(11,105,255,0.12)}
    .btn-ghost{background:transparent; color:var(--accent)}

    /* Hero */
    .hero{display:flex; gap:40px; align-items:center; padding:36px 0}
    .hero-left{flex:1}
    .headline{font-size:28px; font-weight:700; color:var(--accent); margin:0 0 12px}
    .sub{color:var(--muted); margin:0 0 20px}
    .features{display:flex; gap:12px; flex-wrap:wrap}
    .card{background:var(--soft); padding:14px; border-radius:10px}

    .hero-right{width:360px; max-width:40%; background:linear-gradient(180deg,#fff,#f8fafc); border-radius:16px; padding:18px; box-shadow:0 8px 30px rgba(16,24,40,0.04)}
    .sample{border:1px dashed #e6eefc; border-radius:10px; padding:12px; background:white}

    /* Sections */
    section{padding:36px 0}
    h2{margin:0 0 12px; font-size:20px; color:var(--accent)}
    p.lead{color:var(--muted); margin:0 0 18px}

    /* Services grid */
    .grid{display:grid; gap:16px}
    .grid-3{grid-template-columns:repeat(3,1fr)}
    .service-card{background:white; border-radius:12px; padding:18px; box-shadow:0 6px 18px rgba(12,18,24,0.04); border:1px solid #f1f5f9}
    .service-title{font-weight:600; margin:0 0 6px}
    .price{color:var(--primary); font-weight:700}

    /* Portfolio */
    .portfolio{display:flex; gap:12px; flex-wrap:wrap}
    .pf-item{width:calc(33.333% - 8px); border-radius:10px; overflow:hidden; background:linear-gradient(180deg,#ffffff,#fbfdff); border:1px solid #eef2f7; padding:12px}
    .pf-img{height:160px; background:linear-gradient(180deg,#eef7ff,#ffffff); border-radius:8px; display:flex; align-items:center; justify-content:center; color:var(--muted)}

    /* Testimonials */
    .testi{display:flex; gap:12px; flex-wrap:wrap}
    .testi-card{flex:1; min-width:230px; background:white; padding:14px; border-radius:10px; border:1px solid #f0f4f8}

    /* Contact */
    .contact-grid{display:grid; grid-template-columns:1fr 360px; gap:20px}
    form{background:white; border-radius:12px; padding:18px; border:1px solid #eef2f7}
    label{display:block; font-size:13px; color:var(--muted); margin-bottom:6px}
    input, textarea, select{width:100%; padding:10px 12px; border-radius:8px; border:1px solid #e6eef6; font-size:14px}
    textarea{min-height:120px}

    footer{padding:26px 0; color:var(--muted)}

    /* Responsive */
    @media (max-width:900px){
      .grid-3{grid-template-columns:repeat(2,1fr)}
      .hero{flex-direction:column}
      .hero-right{max-width:100%; width:100%}
      .contact-grid{grid-template-columns:1fr}
      .pf-item{width:48%}
      .nav-links{display:none}
      .mobile-toggle{display:inline-flex}
    }
    @media (max-width:520px){
      .grid-3{grid-template-columns:1fr}
      .pf-item{width:100%}
    }

    /* small helpers */
    .muted{color:var(--muted)}
    .kebab{opacity:0.6}

  </style>
</head>
<body>
  <header class="nav">
    <div class="container" style="display:flex;align-items:center;justify-content:space-between;gap:16px">
      <div class="brand">
        <div class="logo">CK</div>
        <div>
          <div style="font-weight:700">CV KILAT</div>
          <div style="font-size:12px;color:var(--muted);margin-top:2px">Jasa pembuatan CV profesional</div>
        </div>
      </div>

      <nav class="nav-links">
        <a href="#services">Layanan</a>
        <a href="#portfolio">Portofolio</a>
        <a href="#testimonials">Testimoni</a>
        <a href="#contact" class="btn btn-ghost">Kontak</a>
        <a href="#" id="whatsappTop" class="btn btn-cta">Pesan Sekarang</a>
      </nav>

      <button class="mobile-toggle btn btn-ghost" style="display:none" aria-label="menu" onclick="toggleMenu()">☰</button>
    </div>
  </header>

  <main class="container">
    <section class="hero">
      <div class="hero-left">
        <h1 class="headline">Buat CV Profesional — Dilirik HRD &amp; ATS-friendly</h1>
        <p class="sub">CV KILAT membantu pelamar kerja membuat Curriculum Vitae modern, ringkas, dan disesuaikan dengan posisi yang dilamar. Fokus pada desain, kata kunci, dan struktur yang disukai perekrut.</p>

        <div class="features">
          <div class="card">✅ CV ATS-friendly</div>
          <div class="card">✅ Revisi hingga 2x</div>
          <div class="card">✅ Contoh portofolio & template</div>
        </div>

        <div style="margin-top:18px;display:flex;gap:12px">
          <a id="cta1" class="btn btn-cta" href="#contact">Pesan Sekarang</a>
          <a href="#portfolio" class="btn btn-ghost">Lihat Portofolio</a>
        </div>

        <div style="margin-top:22px;color:var(--muted);font-size:14px">Paket mulai dari <span class="price">Rp75.000</span> — Pembayaran melalui transfer atau link pembayaran.</div>
      </div>

      <aside class="hero-right">
        <div style="display:flex;align-items:center;justify-content:space-between;margin-bottom:12px">
          <div style="font-weight:700">Contoh CV</div>
          <div class="muted" style="font-size:13px">ATS-friendly</div>
        </div>
        <div class="sample">
          <div style="font-size:13px;color:var(--muted);margin-bottom:8px">Nama: Ahmad Budi</div>
          <div style="font-weight:700;margin-bottom:6px">Posisi: Marketing Executive</div>
          <div style="font-size:13px;color:var(--muted)">Ringkasan profesional singkat yang menonjolkan pencapaian: Meningkatkan leads 30% dalam 6 bulan.</div>
        </div>
      </aside>
    </section>

    <section id="about">
      <h2>Tentang CV KILAT</h2>
      <p class="lead">CV KILAT berdiri untuk membantu pencari kerja menampilkan profil profesional terbaik mereka. Visi kami: mempermudah kandidat mendapatkan panggilan kerja dengan CV yang relevan, rapi, dan terstruktur.</p>
    </section>

    <section id="services">
      <h2>Layanan Kami</h2>
      <p class="lead">Pilih paket yang sesuai dengan kebutuhanmu — dari fresh graduate sampai profesional berpengalaman.</p>
      <div class="grid grid-3">
        <div class="service-card">
          <div class="service-title">CV Fresh Graduate</div>
          <div class="muted">Struktur fokus pada pendidikan, organisasi, dan magang.</div>
          <div style="margin-top:10px" class="price">Rp75.000</div>
        </div>
        <div class="service-card">
          <div class="service-title">CV Profesional</div>
          <div class="muted">Ringkasan eksekutif + pencapaian (achievement-driven).</div>
          <div style="margin-top:10px" class="price">Rp125.000</div>
        </div>
        <div class="service-card">
          <div class="service-title">CV Bahasa Inggris</div>
          <div class="muted">Terjemahan profesional & penyesuaian istilah HR internasional.</div>
          <div style="margin-top:10px" class="price">Rp150.000</div>
        </div>
        <div class="service-card">
          <div class="service-title">CV ATS-Friendly</div>
          <div class="muted">Optimasi kata kunci & format agar lolos sistem ATS.</div>
          <div style="margin-top:10px" class="price">Rp200.000</div>
        </div>
        <div class="service-card">
          <div class="service-title">Paket Lengkap (CV + Surat Lamaran)</div>
          <div class="muted">CV + cover letter yang disesuaikan per posisi.</div>
          <div style="margin-top:10px" class="price">Rp250.000</div>
        </div>
        <div class="service-card">
          <div class="service-title">LinkedIn Optimization</div>
          <div class="muted">Headline, summary, dan pengalaman yang menarik recruiter.</div>
          <div style="margin-top:10px" class="price">Rp180.000</div>
        </div>
      </div>
    </section>

    <section id="portfolio">
      <h2>Portofolio</h2>
      <p class="lead">Contoh desain CV yang pernah kami buat (teks pada contoh hanya ilustrasi).</p>
      <div class="portfolio">
        <div class="pf-item"><div class="pf-img">Contoh A</div></div>
        <div class="pf-item"><div class="pf-img">Contoh B</div></div>
        <div class="pf-item"><div class="pf-img">Contoh C</div></div>
      </div>
    </section>

    <section id="testimonials">
      <h2>Testimoni</h2>
      <div class="testi">
        <div class="testi-card"><div style="font-weight:600">Rina S.</div><div class="muted" style="font-size:13px">"CV KILAT bantu saya dapat panggilan interview dari 3 perusahaan dalam 2 minggu."</div></div>
        <div class="testi-card"><div style="font-weight:600">Dedi P.</div><div class="muted" style="font-size:13px">"Desain rapi dan bahasa profesional — proses cepat."</div></div>
        <div class="testi-card"><div style="font-weight:600">Maya L.</div><div class="muted" style="font-size:13px">"Sangat direkomendasikan untuk fresh graduate."</div></div>
      </div>
    </section>

    <section id="contact">
      <h2>Kontak & Pemesanan</h2>
      <p class="lead">Isi form di bawah atau klik tombol <strong>Pesan via WhatsApp</strong> untuk pemesanan cepat.</p>
      <div class="contact-grid">
        <form id="orderForm">
          <label for="name">Nama</label>
          <input id="name" name="name" placeholder="Nama lengkap" required />

          <label for="email">Email</label>
          <input id="email" name="email" type="email" placeholder="email@contoh.com" required />

          <label for="service">Paket yang dipilih</label>
          <select id="service" name="service">
            <option>CV Fresh Graduate</option>
            <option>CV Profesional</option>
            <option>CV Bahasa Inggris</option>
            <option>CV ATS-Friendly</option>
            <option>Paket Lengkap (CV + Surat Lamaran)</option>
            <option>LinkedIn Optimization</option>
          </select>

          <label for="message">Catatan / Posisi yang dilamar</label>
          <textarea id="message" name="message" placeholder="Deskripsikan posisi, pengalaman singkat, dan kebutuhan khusus..."></textarea>

          <label for="file">Upload CV (opsional)</label>
          <input id="file" name="file" type="file" accept=".pdf,.doc,.docx" />

          <div style="margin-top:12px;display:flex;gap:8px">
            <button type="button" class="btn btn-cta" onclick="sendWhatsApp()">Pesan via WhatsApp</button>
            <button type="button" class="btn btn-ghost" onclick="submitMailto()">Kirim via Email</button>
          </div>
        </form>

        <aside>
          <div style="background:linear-gradient(180deg,#fff,#fbfdff);border-radius:12px;padding:14px;border:1px solid #eef2f7">
            <div style="font-weight:700">Kontak Cepat</div>
            <div class="muted" style="margin-top:6px">WhatsApp: <span id="waNumber">+62812xxxxxxx</span></div>
            <div class="muted" style="margin-top:6px">Email: hello@cvkilat.id</div>
            <div style="margin-top:12px"><small class="muted">Catatan: Form tidak memiliki backend — gunakan tombol WhatsApp untuk pemesanan cepat. Ganti nomor WA pada file HTML sebelum deploy.</small></div>
          </div>
        </aside>
      </div>
    </section>

  </main>

  <footer class="container">
    <div style="display:flex;justify-content:space-between;align-items:center;gap:12px;flex-wrap:wrap">
      <div>© <span id="year"></span> CV KILAT — Semua hak cipta dilindungi.</div>
      <div class="muted">Follow: Instagram / LinkedIn (tambahkan link)</div>
    </div>
  </footer>

  <script>
    // Small helpers
    document.getElementById('year').textContent = new Date().getFullYear();

    // Replace this with your WhatsApp number (E.164 format, tanpa spasi, contoh: +6281234567890)
    const WA_NUMBER = '+62812xxxxxxx';
    document.getElementById('waNumber').textContent = WA_NUMBER;

    function sendWhatsApp(){
      const name = encodeURIComponent(document.getElementById('name').value || '');
      const email = encodeURIComponent(document.getElementById('email').value || '');
      const service = encodeURIComponent(document.getElementById('service').value || '');
      const message = encodeURIComponent(document.getElementById('message').value || '');

      let text = `Halo CV KILAT,%0ASaya ingin memesan layanan: *${service}*%0ANama: ${name}%0AEmail: ${email}%0ACatatan: ${message}%0A(Tolong bantu informasikan metode pembayaran)`;

      // Because we can't attach files via plain wa link reliably, ask user to attach file manually in WhatsApp
      const waUrl = `https://wa.me/${WA_NUMBER.replace('+','')}?text=${text}`;
      window.open(waUrl, '_blank');
    }

    function submitMailto(){
      const name = encodeURIComponent(document.getElementById('name').value || '');
      const email = encodeURIComponent(document.getElementById('email').value || '');
      const service = encodeURIComponent(document.getElementById('service').value || '');
      const message = encodeURIComponent(document.getElementById('message').value || '');

      const subject = encodeURIComponent('Pemesanan Layanan - ' + service);
      const body = encodeURIComponent(`Nama: ${name}%0AEmail: ${email}%0AService: ${service}%0A%0ACatatan:%0A${decodeURIComponent(message)}%0A%0A(Terima kasih)`);
      window.location.href = `mailto:hello@cvkilat.id?subject=${subject}&body=${body}`;
    }

    // Smooth scrolling for internal links
    document.querySelectorAll('a[href^="#"]').forEach(a=>{
      a.addEventListener('click', function(e){
        const target = document.querySelector(this.getAttribute('href'));
        if(target){ e.preventDefault(); target.scrollIntoView({behavior:'smooth', block:'start'}); }
      })
    })

    // Mobile nav toggle (basic)
    function toggleMenu(){
      const nav = document.querySelector('.nav-links');
      if(nav.style.display === 'flex') nav.style.display = 'none'; else nav.style.display = 'flex';
    }
  </script>
</body>
</html>
