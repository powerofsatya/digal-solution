<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>MTSS — Security • Staffing • Facility Experts</title>
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700;900&display=swap" rel="stylesheet">
  <meta name="description" content="MTSS — Professional security, staffing and facility experts" />
  <style>
    :root{
      --bg:#f5f7fa;
      --muted:#6b7280;
      --accent:#0a84ff;
      --dark:#0f1724;
      --glass: rgba(255,255,255,0.7);
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family: 'Poppins', system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background:linear-gradient(180deg,var(--bg),#ffffff 60%);
      color:var(--dark);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
    }
    .container{max-width:1200px;margin:0 auto;padding:28px}

    /* NAV */
    header{
      position:sticky;top:0;z-index:40;background:transparent;padding:18px 0;backdrop-filter: blur(6px);
    }
    .nav-inner{display:flex;align-items:center;justify-content:space-between;gap:18px}
    .brand{display:flex;align-items:center;gap:14px}
    .brand img{height:44px;width:auto;display:block}
    .brand h1{font-size:1.05rem;margin:0;font-weight:700;letter-spacing:1px}
    nav ul{display:flex;gap:20px;list-style:none;margin:0;padding:0;align-items:center}
    nav a{color:var(--dark);text-decoration:none;font-weight:600;opacity:.95}
    nav a.small{font-weight:500;color:var(--muted);font-size:.95rem}
    .cta{padding:10px 14px;border-radius:10px;background:var(--dark);color:#fff;text-decoration:none;font-weight:700}

    /* HERO */
    .hero{padding:88px 16px 120px;text-align:center}
    .hero-grid{display:grid;grid-template-columns:1fr;gap:28px;align-items:center}
    .hero-badge{display:inline-block;padding:8px 14px;border-radius:999px;background:rgba(10,132,255,0.12);color:var(--accent);font-weight:700;font-size:.9rem}
    .hero h2{font-size: clamp(28px, 4.6vw, 56px);line-height:1.02;margin:10px 0;font-weight:800}
    .hero p{max-width:780px;margin:16px auto;font-size:1.05rem;color:var(--muted);}
    .hero-actions{display:flex;gap:14px;justify-content:center;margin-top:18px}
    .btn{padding:12px 18px;border-radius:12px;text-decoration:none;font-weight:700}
    .btn-primary{background:var(--dark);color:#fff}
    .btn-ghost{background:transparent;border:1px solid rgba(15,23,36,0.08);color:var(--dark)}

    /* Showcase card */
    .showcase{margin-top:34px;border-radius:18px;overflow:hidden;display:flex;align-items:center;justify-content:center;padding:24px;background:linear-gradient(180deg, rgba(255,255,255,0.8), rgba(250,250,250,0.6));box-shadow:0 20px 40px rgba(10,10,10,0.05)}
    .showcase .logo-wrap{display:flex;align-items:center;gap:18px}
    .showcase img{height:96px;width:auto;border-radius:12px}
    .showcase .intro{max-width:760px;text-align:left}
    .showcase h3{margin:0;font-size:1.25rem;font-weight:800}
    .showcase p{margin:6px 0;color:var(--muted)}

    /* FEATURES */
    .features{display:grid;grid-template-columns:repeat(3,1fr);gap:20px;margin:72px 0}
    .feature{background:#fff;border-radius:14px;padding:22px;box-shadow:0 8px 30px rgba(15,23,36,0.04);min-height:150px}
    .feature h4{margin:0 0 10px 0;font-size:1.05rem}
    .feature p{color:var(--muted);margin:0;font-size:.98rem}

    /* SERVICES full-width band */
    .band{background:linear-gradient(90deg, #fbfcff, #f1f9ff);padding:36px;border-radius:16px;display:flex;align-items:center;justify-content:space-between;gap:20px}
    .band .left{max-width:720px}
    .band h3{margin:0;font-weight:800}
    .band p{color:var(--muted);margin-top:8px}

    /* CONTACT */
    .contact{margin:72px 0;display:grid;grid-template-columns:1fr 420px;gap:30px;align-items:start}
    .contact-card{background:#fff;padding:28px;border-radius:12px;box-shadow:0 10px 30px rgba(15,23,36,0.04)}
    .contact form{display:flex;flex-direction:column;gap:12px}
    input,textarea{padding:12px;border-radius:10px;border:1px solid #e6e9ee;font-size:1rem}
    textarea{min-height:140px}

    footer{margin-top:72px;padding:28px 0;text-align:center;color:var(--muted);font-size:.95rem}

    /* tiny helpers */
    .muted{color:var(--muted)}

    /* Responsive */
    @media (max-width:900px){
      .features{grid-template-columns:1fr 1fr}
      .contact{grid-template-columns:1fr}
      .showcase{flex-direction:column;text-align:center}
      .showcase .intro{text-align:center}
    }
    @media (max-width:640px){
      nav ul{display:none}
      .hero{padding:48px 16px 80px}
      .brand h1{display:none}
      .features{grid-template-columns:1fr}
    }

    /* subtle animations */
    .fade-up{transform:translateY(10px);opacity:0;animation:up .7s cubic-bezier(.2,.9,.2,1) forwards}
    @keyframes up{to{transform:none;opacity:1}}
  </style>
</head>
<body>
  <header>
    <div class="container nav-inner">
      <div class="brand">
        <img src="MTSS logo.png" alt="MTSS logo" />
        <h1>MTSS</h1>
      </div>
      <nav>
        <ul>
          <li><a href="#services">Services</a></li>
          <li><a href="#about">About</a></li>
          <li><a href="#contact" class="small">Contact</a></li>
          <li><a href="#" class="cta">Get a Quote</a></li>
        </ul>
      </nav>
    </div>
  </header>

  <main>
    <section class="hero">
      <div class="container hero-grid">
        <div>
          <span class="hero-badge fade-up">Security • Staffing • Facility</span>
          <h2 class="fade-up">Professional protection and workplace services that just work.</h2>
          <p class="fade-up">MTSS delivers trusted security, reliable staffing solutions, and efficient facility management — built for organisations that expect excellence. Modern processes, trained people, and strict quality controls.</p>
          <div class="hero-actions fade-up">
            <a class="btn btn-primary" href="#contact">Request a Quote</a>
            <a class="btn btn-ghost" href="#services">Explore Services</a>
          </div>
        </div>

        <div class="showcase fade-up" aria-hidden="true">
          <div class="logo-wrap">
            <img src="MTSS logo.png" alt="MTSS logo"/>
            <div class="intro">
              <h3>Trusted by businesses across the region</h3>
              <p class="muted">Security officers, facility teams and staffing resources aligned to your needs. 24/7 support &amp; real-time reporting.</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section id="services" class="container">
      <h2 class="section-title">Our Services</h2>
      <div class="features">
        <div class="feature fade-up">
          <h4>Physical Security</h4>
          <p>Uniformed guards, mobile patrols, CCTV monitoring and incident reporting — tailored to your site risk profile.</p>
        </div>
        <div class="feature fade-up">
          <h4>Staffing Solutions</h4>
          <p>Pre-screened personnel for industrial, corporate and events. Quick scaling and long-term placements available.</p>
        </div>
        <div class="feature fade-up">
          <h4>Facility Management</h4>
          <p>Cleaning, maintenance, and asset management to keep your operations running smoothly and safely.</p>
        </div>
      </div>

      <div class="band fade-up" style="margin-top:28px">
        <div class="left">
          <h3>Enterprise-level service, local delivery</h3>
          <p>Integrated operations with dedicated account managers and regular quality audits to meet SLAs and compliance.</p>
        </div>
        <div>
          <a class="btn btn-primary" href="#contact">Talk to Sales</a>
        </div>
      </div>
    </section>

    <section id="about" class="container" style="margin-top:44px">
      <h2 class="section-title">About MTSS</h2>
      <div style="max-width:880px;margin:0 auto;color:var(--muted);text-align:center"> 
        MTSS combines experienced personnel and modern systems to deliver professional security, staffing and facility services. Our focus is operational excellence, proactive risk management and transparent reporting.</div>
    </section>

    <section id="contact" class="container">
      <h2 class="section-title">Get in touch</h2>
      <div class="contact">
        <div class="contact-card fade-up">
          <h3>Request a quote</h3>
          <p class="muted">Tell us about your requirements and we'll get back within one business day.</p>
          <form>
            <input type="text" placeholder="Full name" required />
            <input type="email" placeholder="Email address" required />
            <input type="text" placeholder="Company / Site" />
            <textarea placeholder="Brief description of your requirement"></textarea>
            <div style="display:flex;gap:10px;margin-top:8px">
              <button class="btn btn-primary" type="submit">Submit Request</button>
              <a class="btn btn-ghost" href="tel:+000000000">Call Us</a>
            </div>
          </form>
        </div>

        <div>
          <div class="contact-card fade-up">
            <h4>Office</h4>
            <p class="muted">Jharsuguda, Odisha — India</p>
            <hr style="margin:12px 0;border:none;border-top:1px solid #eef2f6">
            <p style="margin:0"><strong>Support:</strong> +91 00000 00000</p>
            <p style="margin:0"><strong>Email:</strong> info@mtss.example</p>
          </div>

          <div style="height:18px"></div>

          <div class="contact-card fade-up">
            <h4>Why clients choose us</h4>
            <p class="muted">Rigorous training • Background-checked staff • 24/7 operations • Digital reporting</p>
          </div>
        </div>
      </div>
    </section>

  </main>

  <footer>
    <div class="container">
      <small>© <span id="year"></span> MTSS — All rights reserved.</small>
    </div>
  </footer>

  <script>
    // Small interactions
    document.getElementById('year').textContent = new Date().getFullYear();
    // simple form interception (demo)
    document.querySelector('form')?.addEventListener('submit', function(e){
      e.preventDefault();
      alert('Thanks! Your request was submitted (demo).');
      this.reset();
    });
  </script>
</body>
</html>

