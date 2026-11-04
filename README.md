<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>MAYTECH Solutions — TV & Console Repair Services | Lagos</title>
<meta name="description" content="MAYTECH Solutions offers fast, reliable and affordable Smart TV, LED, OLED & QLED TV repair and PlayStation / Xbox console repair in Oshodi, Lagos. WhatsApp 0903 008 7669.">
<style>
  :root{
    --bg:#040b1e;
    --bg2:#071633;
    --panel:#0a1f45;
    --blue:#1e90ff;
    --cyan:#00e5ff;
    --yellow:#ffd400;
    --white:#f4f8ff;
    --muted:#9db4d8;
    --grad:linear-gradient(135deg,#00e5ff 0%,#1e90ff 100%);
  }
  *{margin:0;padding:0;box-sizing:border-box;}
  html{scroll-behavior:smooth;}
  body{
    font-family:'Segoe UI',Arial,sans-serif;
    background:var(--bg);
    color:var(--white);
    line-height:1.6;
    overflow-x:hidden;
  }

  /* ---------- Header ---------- */
  header{
    position:fixed;top:0;left:0;right:0;z-index:100;
    display:flex;align-items:center;justify-content:space-between;
    padding:14px 5%;
    background:rgba(4,11,30,.85);
    backdrop-filter:blur(12px);
    border-bottom:1px solid rgba(0,229,255,.25);
  }
  .logo{display:flex;align-items:center;gap:10px;text-decoration:none;}
  .logo-mark{
    width:44px;height:44px;border-radius:50%;
    background:var(--grad);
    display:flex;align-items:center;justify-content:center;
    font-weight:900;font-size:22px;color:#02101f;
    box-shadow:0 0 18px rgba(0,229,255,.6);
  }
  .logo-text{font-weight:800;letter-spacing:2px;font-size:1.05rem;color:var(--white);}
  .logo-text span{display:block;font-size:.6rem;letter-spacing:6px;color:var(--cyan);font-weight:600;}
  nav a{
    color:var(--muted);text-decoration:none;margin-left:24px;font-size:.95rem;
    transition:color .2s;
  }
  nav a:hover{color:var(--cyan);}
  .nav-cta{
    background:var(--grad);color:#02101f!important;font-weight:700;
    padding:8px 18px;border-radius:30px;
  }
  @media(max-width:960px){nav a:not(.nav-cta){display:none;}}

  /* ---------- Hero ---------- */
  .hero{
    min-height:100vh;
    display:flex;align-items:center;
    padding:130px 5% 70px;
    position:relative;
    background:
      radial-gradient(circle at 80% 20%,rgba(30,144,255,.25),transparent 45%),
      radial-gradient(circle at 15% 85%,rgba(0,229,255,.18),transparent 40%),
      linear-gradient(180deg,var(--bg) 0%,var(--bg2) 100%);
  }
  .hero::before{
    content:"";position:absolute;inset:0;pointer-events:none;
    background-image:
      linear-gradient(rgba(0,229,255,.05) 1px,transparent 1px),
      linear-gradient(90deg,rgba(0,229,255,.05) 1px,transparent 1px);
    background-size:48px 48px;
    mask-image:radial-gradient(circle at 50% 40%,black,transparent 75%);
  }
  .hero-inner{
    display:grid;grid-template-columns:1.15fr .85fr;gap:50px;align-items:center;
    max-width:1200px;margin:0 auto;position:relative;z-index:1;width:100%;
  }
  .tagline{
    display:inline-block;border:1px solid rgba(0,229,255,.5);color:var(--cyan);
    padding:6px 16px;border-radius:30px;font-size:.8rem;letter-spacing:3px;
    text-transform:uppercase;margin-bottom:22px;
    background:rgba(0,229,255,.07);
  }
  h1{
    font-size:clamp(2.2rem,5vw,3.8rem);
    line-height:1.1;font-weight:900;text-transform:uppercase;
  }
  h1 .yellow{
    background:linear-gradient(180deg,#ffe95e,var(--yellow));
    -webkit-background-clip:text;background-clip:text;color:transparent;
    text-shadow:0 0 30px rgba(255,212,0,.25);
  }
  .hero-sub{
    color:var(--white);font-weight:700;letter-spacing:1px;margin:14px 0 8px;font-size:1.15rem;
  }
  .hero-desc{color:var(--muted);max-width:520px;margin-bottom:30px;}
  .btn-row{display:flex;gap:16px;flex-wrap:wrap;}
  .btn{
    display:inline-flex;align-items:center;gap:10px;
    padding:14px 28px;border-radius:40px;font-weight:700;text-decoration:none;
    transition:transform .2s,box-shadow .2s;font-size:1rem;border:none;cursor:pointer;
  }
  .btn:hover{transform:translateY(-3px);}
  .btn-wa{background:#25D366;color:#04160b;box-shadow:0 8px 25px rgba(37,211,102,.35);}
  .btn-wa:hover{box-shadow:0 12px 32px rgba(37,211,102,.5);}
  .btn-ghost{border:1px solid rgba(0,229,255,.5);color:var(--cyan);}
  .btn-ghost:hover{background:rgba(0,229,255,.1);}

  .hero-card{
    background:rgba(10,31,69,.6);
    border:1px solid rgba(0,229,255,.3);
    border-radius:22px;padding:30px;
    box-shadow:0 0 50px rgba(30,144,255,.25),inset 0 0 40px rgba(0,229,255,.04);
    backdrop-filter:blur(8px);
  }
  .hero-card h3{color:var(--cyan);letter-spacing:2px;font-size:.85rem;text-transform:uppercase;margin-bottom:16px;}
  .hero-card ul{list-style:none;}
  .hero-card li{
    display:flex;align-items:center;gap:12px;padding:9px 0;
    border-bottom:1px dashed rgba(157,180,216,.15);font-size:.98rem;
  }
  .hero-card li:last-child{border-bottom:none;}
  .check{
    flex:0 0 24px;width:24px;height:24px;border-radius:50%;
    background:var(--grad);display:flex;align-items:center;justify-content:center;
    font-size:.75rem;color:#02101f;font-weight:900;
  }
  .hero-card li.hl{color:var(--yellow);font-weight:700;}
  @media(max-width:900px){
    .hero-inner{grid-template-columns:1fr;}
  }

  /* ---------- Marquee brands ---------- */
  .brands{
    padding:34px 0;border-top:1px solid rgba(0,229,255,.15);
    border-bottom:1px solid rgba(0,229,255,.15);
    background:rgba(7,22,51,.6);overflow:hidden;white-space:nowrap;
  }
  .marquee{display:inline-block;animation:scroll 22s linear infinite;}
  .marquee span{
    font-size:1.6rem;font-weight:900;letter-spacing:2px;margin:0 42px;
    color:var(--muted);text-transform:uppercase;
  }
  .marquee span:nth-child(odd){color:var(--white);}
  @keyframes scroll{from{transform:translateX(0);}to{transform:translateX(-50%);}}

  /* ---------- Sections ---------- */
  section{padding:90px 5%;}
  .wrap{max-width:1150px;margin:0 auto;}
  .sec-head{text-align:center;margin-bottom:55px;}
  .sec-head .kicker{color:var(--cyan);letter-spacing:4px;text-transform:uppercase;font-size:.8rem;font-weight:700;}
  .sec-head h2{font-size:clamp(1.8rem,4vw,2.6rem);text-transform:uppercase;font-weight:900;margin-top:8px;}
  .sec-head h2 em{font-style:normal;color:var(--yellow);}
  .sec-head p{color:var(--muted);max-width:600px;margin:12px auto 0;}

  /* services grid */
  .grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(255px,1fr));gap:22px;}
  .card{
    background:var(--panel);border:1px solid rgba(0,229,255,.15);
    border-radius:18px;padding:28px;transition:transform .25s,border-color .25s,box-shadow .25s;
  }
  .card:hover{
    transform:translateY(-6px);border-color:var(--cyan);
    box-shadow:0 15px 40px rgba(30,144,255,.25);
  }
  .icon{
    width:54px;height:54px;border-radius:14px;
    background:rgba(0,229,255,.1);border:1px solid rgba(0,229,255,.35);
    display:flex;align-items:center;justify-content:center;font-size:1.5rem;margin-bottom:18px;
  }
  .card h3{font-size:1.1rem;margin-bottom:8px;}
  .card p{color:var(--muted);font-size:.92rem;}

  /* ---------- Gallery ---------- */
  .gallery-grid{
    display:grid;grid-template-columns:repeat(auto-fit,minmax(240px,1fr));gap:20px;
  }
  .g-item{
    border-radius:18px;overflow:hidden;border:1px solid rgba(0,229,255,.2);
    aspect-ratio:4/3;position:relative;background:var(--panel);
    transition:transform .25s,border-color .25s;
  }
  .g-item:hover{transform:translateY(-5px);border-color:var(--cyan);}
  .g-item img{width:100%;height:100%;object-fit:cover;display:block;}
  .g-item .ph{
    width:100%;height:100%;display:flex;flex-direction:column;align-items:center;justify-content:center;
    gap:8px;color:var(--muted);text-align:center;padding:16px;font-size:.9rem;
    background:linear-gradient(135deg,rgba(10,31,69,.9),rgba(7,22,51,.9));
  }
  .g-item .ph .ph-icon{font-size:2rem;}
  .g-item .ph b{color:var(--cyan);}
  .g-cap{
    position:absolute;left:0;right:0;bottom:0;padding:10px 14px;
    background:linear-gradient(180deg,transparent,rgba(4,11,30,.92));
    font-size:.85rem;font-weight:600;
  }

  /* ---------- Testimonials ---------- */
  .reviews{background:linear-gradient(180deg,var(--bg2),var(--bg));}
  .review-card{display:flex;flex-direction:column;}
  .stars{color:var(--yellow);font-size:1.1rem;letter-spacing:3px;margin-bottom:12px;}
  .review-card p{color:var(--muted);font-size:.95rem;font-style:italic;flex:1;}
  .reviewer{display:flex;align-items:center;gap:12px;margin-top:18px;}
  .avatar{
    width:44px;height:44px;border-radius:50%;background:var(--grad);
    display:flex;align-items:center;justify-content:center;font-weight:900;color:#02101f;
  }
  .reviewer .rname{font-weight:700;font-size:.95rem;}
  .reviewer .rjob{color:var(--muted);font-size:.8rem;}
  .sample-note{
    text-align:center;color:var(--muted);font-size:.8rem;margin-top:26px;
    border:1px dashed rgba(157,180,216,.3);border-radius:12px;padding:10px 18px;
    display:inline-block;
  }

  /* ---------- Why us ---------- */
  .why .grid{grid-template-columns:repeat(auto-fit,minmax(220px,1fr));}
  .why .card{text-align:center;}
  .why .icon{margin:0 auto 16px;}

  /* ---------- Steps ---------- */
  .steps{counter-reset:step;}
  .step{display:flex;gap:20px;align-items:flex-start;padding:20px 0;border-bottom:1px solid rgba(157,180,216,.12);}
  .step:last-child{border-bottom:none;}
  .step-num{
    counter-increment:step;flex:0 0 52px;height:52px;border-radius:50%;
    background:var(--grad);color:#02101f;font-weight:900;font-size:1.3rem;
    display:flex;align-items:center;justify-content:center;
  }
  .step-num::before{content:counter(step);}
  .step h3{font-size:1.05rem;}
  .step p{color:var(--muted);font-size:.92rem;}

  /* ---------- Booking form ---------- */
  .booking{
    background:
      radial-gradient(circle at 15% 25%,rgba(37,211,102,.1),transparent 45%),
      radial-gradient(circle at 85% 80%,rgba(30,144,255,.2),transparent 45%),
      var(--bg2);
  }
  .form-card{
    max-width:680px;margin:0 auto;background:rgba(10,31,69,.75);
    border:1px solid rgba(0,229,255,.25);border-radius:22px;padding:36px;
    backdrop-filter:blur(8px);box-shadow:0 0 50px rgba(30,144,255,.15);
  }
  .form-row{display:grid;grid-template-columns:1fr 1fr;gap:18px;}
  @media(max-width:640px){.form-row{grid-template-columns:1fr;}}
  .field{margin-bottom:18px;}
  .field label{display:block;font-size:.85rem;font-weight:700;letter-spacing:1px;color:var(--cyan);margin-bottom:6px;text-transform:uppercase;}
  .field input,.field select,.field textarea{
    width:100%;padding:13px 15px;border-radius:12px;
    background:rgba(4,11,30,.7);border:1px solid rgba(157,180,216,.3);
    color:var(--white);font-size:.95rem;font-family:inherit;transition:border-color .2s;
  }
  .field input:focus,.field select:focus,.field textarea:focus{
    outline:none;border-color:var(--cyan);box-shadow:0 0 0 3px rgba(0,229,255,.12);
  }
  .field textarea{resize:vertical;min-height:110px;}
  .field select option{background:var(--panel);}
  .form-note{color:var(--muted);font-size:.82rem;text-align:center;margin-top:14px;}

  /* ---------- Contact ---------- */
  .contact{text-align:center;}
  .phone-big{
    font-size:clamp(2rem,6vw,3.4rem);font-weight:900;color:var(--yellow);
    text-decoration:none;letter-spacing:2px;display:block;margin:18px 0;
    text-shadow:0 0 35px rgba(255,212,0,.3);
  }
  .addr{color:var(--muted);font-size:1.05rem;max-width:560px;margin:0 auto 34px;}
  .addr b{color:var(--white);}
  .hours{color:var(--cyan);font-weight:700;letter-spacing:2px;text-transform:uppercase;font-size:.85rem;}
  .flyer-box{
    max-width:420px;margin:50px auto 0;border-radius:20px;overflow:hidden;
    border:1px solid rgba(0,229,255,.35);box-shadow:0 0 45px rgba(30,144,255,.3);
  }
  .flyer-box img{width:100%;display:block;}

  footer{
    padding:36px 5%;text-align:center;color:var(--muted);font-size:.9rem;
    border-top:1px solid rgba(0,229,255,.15);
  }
  footer .slogan{color:var(--white);letter-spacing:6px;font-weight:700;margin-bottom:8px;text-transform:uppercase;}

  .wa-float{
    position:fixed;right:22px;bottom:22px;z-index:99;
    width:60px;height:60px;border-radius:50%;background:#25D366;
    display:flex;align-items:center;justify-content:center;
    box-shadow:0 8px 25px rgba(37,211,102,.5);
    transition:transform .2s;text-decoration:none;
  }
  .wa-float:hover{transform:scale(1.1);}
  .wa-float svg{width:32px;height:32px;fill:#fff;}
</style>
</head>
<body>

<header>
  <a class="logo" href="#top">
    <div class="logo-mark">M</div>
    <div class="logo-text">MAYTECH<span>SOLUTIONS</span></div>
  </a>
  <nav>
    <a href="#services">Services</a>
    <a href="#gallery">Gallery</a>
    <a href="#reviews">Reviews</a>
    <a href="#booking">Book Repair</a>
    <a href="#contact">Contact</a>
    <a class="nav-cta" href="https://wa.me/2349030087669" target="_blank" rel="noopener">WhatsApp Us</a>
  </nav>
</header>

<!-- HERO -->
<section class="hero" id="top">
  <div class="hero-inner">
    <div>
      <span class="tagline">Your Tech, Our Priority</span>
      <h1>TV &amp; Console<br><span class="yellow">Repair Services</span></h1>
      <p class="hero-sub">Fast. Reliable. Affordable.</p>
      <p class="hero-desc">
        Expert repair for Smart TVs, LED, OLED &amp; QLED screens and all major game
        consoles — PlayStation, Xbox and more. Serving Bolade, Oshodi, Lagos and beyond.
      </p>
      <div class="btn-row">
        <a class="btn btn-wa" href="https://wa.me/2349030087669" target="_blank" rel="noopener">💬 WhatsApp 0903 008 7669</a>
        <a class="btn btn-ghost" href="#booking">Book a Repair →</a>
      </div>
    </div>
    <div class="hero-card">
      <h3>What We Fix</h3>
      <ul>
        <li><span class="check">✓</span> Smart TV Repair</li>
        <li><span class="check">✓</span> LED TV Repair</li>
        <li><span class="check">✓</span> OLED &amp; QLED TV Repair</li>
        <li><span class="check">✓</span> PlayStation (PS4 / PS5)</li>
        <li><span class="check">✓</span> Xbox (Series X/S, One)</li>
        <li><span class="check">✓</span> Game Console Repair</li>
        <li class="hl"><span class="check">★</span> Screen Repair &amp; Replacement</li>
        <li><span class="check">✓</span> Power &amp; Display Issues</li>
        <li><span class="check">✓</span> And More…</li>
      </ul>
    </div>
  </div>
</section>

<!-- BRANDS -->
<div class="brands">
  <div class="marquee">
    <span>Samsung</span><span>LG</span><span>Sony</span><span>Hisense</span><span>TCL</span><span>Skyworth</span>
    <span>Samsung</span><span>LG</span><span>Sony</span><span>Hisense</span><span>TCL</span><span>Skyworth</span>
  </div>
</div>

<!-- SERVICES -->
<section id="services">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">Our Services</div>
      <h2>Repairs Done <em>Right</em></h2>
      <p>From cracked screens to dead power boards — if it plugs in and turns on, we can fix it.</p>
    </div>
    <div class="grid">
      <div class="card"><div class="icon">📺</div><h3>Smart TV Repair</h3><p>Software issues, app failures, board-level faults and network problems on all Smart TV platforms.</p></div>
      <div class="card"><div class="icon">💡</div><h3>LED TV Repair</h3><p>Backlight replacement, dim or flickering screens, distorted images and sound problems.</p></div>
      <div class="card"><div class="icon">🌈</div><h3>OLED &amp; QLED Repair</h3><p>Specialist care for premium panels — burn-in, banding, panel replacement and more.</p></div>
      <div class="card"><div class="icon">🎮</div><h3>PlayStation Repair</h3><p>PS4 &amp; PS5 HDMI port replacement, overheating, disc drive faults, power and blue-light issues.</p></div>
      <div class="card"><div class="icon">🕹️</div><h3>Xbox Repair</h3><p>Series X/S and Xbox One — no-display, overheating, power supply and controller repairs.</p></div>
      <div class="card"><div class="icon">🔧</div><h3>Screen Repair &amp; Replacement</h3><p>Cracked or broken screens replaced with quality panels for TVs of all sizes.</p></div>
      <div class="card"><div class="icon">⚡</div><h3>Power Issues</h3><p>Dead devices, no-power faults, blown boards and power supply replacements.</p></div>
      <div class="card"><div class="icon">🖥️</div><h3>Display Issues</h3><p>No picture, lines on screen, colour distortion and other display faults diagnosed and fixed.</p></div>
    </div>
  </div>
</section>

<!-- GALLERY -->
<section id="gallery" style="background:rgba(7,22,51,.4);">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">Our Work</div>
      <h2>Repair <em>Gallery</em></h2>
      <p>A look at the devices we bring back to life. Real customer job photos coming soon!</p>
    </div>
    <div class="gallery-grid">
      <div class="g-item">
        <img src="maytech-flyer.jpg" alt="MAYTECH Solutions flyer — TV and console repair services">
        <div class="g-cap">📄 Our Official Flyer</div>
      </div>
      <div class="g-item"><div class="ph"><span class="ph-icon">📸</span><b>Your photo here</b>Finished TV repair</div></div>
      <div class="g-item"><div class="ph"><span class="ph-icon">📸</span><b>Your photo here</b>Console motherboard fix</div></div>
      <div class="g-item"><div class="ph"><span class="ph-icon">📸</span><b>Your photo here</b>Screen replacement</div></div>
      <div class="g-item"><div class="ph"><span class="ph-icon">📸</span><b>Your photo here</b>Before &amp; after repair</div></div>
      <div class="g-item"><div class="ph"><span class="ph-icon">📸</span><b>Your photo here</b>Our workshop</div></div>
    </div>
  </div>
</section>

<!-- TESTIMONIALS -->
<section class="reviews" id="reviews">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">Testimonials</div>
      <h2>What Customers <em>Say</em></h2>
    </div>
    <div class="grid">
      <div class="card review-card">
        <div class="stars">★★★★★</div>
        <p>"My 55" Samsung TV had no picture and I thought it was finished. MAYTECH fixed the backlight the same day and it looks brand new. Great price too!"</p>
        <div class="reviewer"><div class="avatar">A</div><div><div class="rname">Adewale K.</div><div class="rjob">Oshodi, Lagos</div></div></div>
      </div>
      <div class="card review-card">
        <div class="stars">★★★★★</div>
        <p>"My PS5 HDMI port was damaged and they replaced it perfectly. It's been months and everything still works flawlessly. Very professional service."</p>
        <div class="reviewer"><div class="avatar">C</div><div><div class="rname">Chidinma O.</div><div class="rjob">Ikeja, Lagos</div></div></div>
      </div>
      <div class="card review-card">
        <div class="stars">★★★★★</div>
        <p>"Fast, honest and affordable. They told me exactly what was wrong with my Hisense TV and didn't charge me for parts I didn't need. I highly recommend them."</p>
        <div class="reviewer"><div class="avatar">I</div><div><div class="rname">Ibrahim M.</div><div class="rjob">Mushin, Lagos</div></div></div>
      </div>
    </div>
    <div style="text-align:center;">
      <span class="sample-note">ℹ️ These are sample testimonials — replace them with real customer reviews.</span>
    </div>
  </div>
</section>

<!-- WHY US -->
<section class="why" id="why">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">Why MAYTECH</div>
      <h2>Built on <em>Trust</em></h2>
    </div>
    <div class="grid">
      <div class="card"><div class="icon">⚡</div><h3>Quick Turnaround</h3><p>Most repairs completed fast — we know you can't wait to get back to your screen.</p></div>
      <div class="card"><div class="icon">🛡️</div><h3>Professional Service</h3><p>Skilled technicians, quality parts and careful handling of your device every time.</p></div>
      <div class="card"><div class="icon">🤝</div><h3>Affordable Prices</h3><p>Honest, transparent pricing with no hidden charges — repair, don't replace.</p></div>
      <div class="card"><div class="icon">🎧</div><h3>24/7 Support</h3><p>Reach us anytime on WhatsApp for enquiries, updates and after-service support.</p></div>
    </div>
  </div>
</section>

<!-- PROCESS -->
<section id="process">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">How It Works</div>
      <h2>Simple <em>3-Step</em> Process</h2>
    </div>
    <div class="steps">
      <div class="step"><div class="step-num"></div><div><h3>Book or Message Us</h3><p>Fill the booking form below or WhatsApp us — describe the fault, share photos or video of the issue, and get a quick assessment.</p></div></div>
      <div class="step"><div class="step-num"></div><div><h3>Diagnosis &amp; Fair Quote</h3><p>Bring your device to our shop or arrange drop-off. We diagnose it and give you a clear, affordable quote.</p></div></div>
      <div class="step"><div class="step-num"></div><div><h3>Repair &amp; Pickup</h3><p>We fix it fast, test it thoroughly, and hand it back — working like new. Warranty on repairs available.</p></div></div>
    </div>
  </div>
</section>

<!-- BOOKING FORM -->
<section class="booking" id="booking">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">Book a Repair</div>
      <h2>Request a <em>Repair</em></h2>
      <p>Fill in the details below — it opens WhatsApp with your request ready to send. We reply fast!</p>
    </div>
    <form class="form-card" id="bookingForm">
      <div class="form-row">
        <div class="field">
          <label for="bname">Your Name *</label>
          <input type="text" id="bname" required placeholder="e.g. Adewale K.">
        </div>
        <div class="field">
          <label for="bphone">Phone Number *</label>
          <input type="tel" id="bphone" required placeholder="e.g. 0803 000 0000">
        </div>
      </div>
      <div class="form-row">
        <div class="field">
          <label for="bdevice">Device Type *</label>
          <select id="bdevice" required>
            <option value="">Select a device…</option>
            <option>Smart TV</option>
            <option>LED TV</option>
            <option>OLED / QLED TV</option>
            <option>PlayStation (PS4/PS5)</option>
            <option>Xbox (Series X/S, One)</option>
            <option>Other Game Console</option>
            <option>Other Device</option>
          </select>
        </div>
        <div class="field">
          <label for="bbrand">Brand</label>
          <select id="bbrand">
            <option value="">Select a brand…</option>
            <option>Samsung</option>
            <option>LG</option>
            <option>Sony</option>
            <option>Hisense</option>
            <option>TCL</option>
            <option>Skyworth</option>
            <option>Other</option>
          </select>
        </div>
      </div>
      <div class="field">
        <label for="bmodel">Model / Size</label>
        <input type="text" id="bmodel" placeholder="e.g. Samsung 55" TU8000 or PS5">
      </div>
      <div class="field">
        <label for="bissue">Describe the Problem *</label>
        <textarea id="bissue" required placeholder="e.g. TV turns on but no picture, or PS5 HDMI port bent…"></textarea>
      </div>
      <button type="submit" class="btn btn-wa" style="width:100%;justify-content:center;">💬 Send Request via WhatsApp</button>
      <p class="form-note">Submitting opens WhatsApp with your details pre-filled — just press send. No account needed.</p>
    </form>
  </div>
</section>

<!-- CONTACT -->
<section class="contact" id="contact">
  <div class="wrap">
    <div class="sec-head">
      <div class="kicker">Get In Touch</div>
      <h2>WhatsApp Us <em>Today!</em></h2>
    </div>
    <a class="phone-big" href="https://wa.me/2349030087669" target="_blank" rel="noopener">0903 008 7669</a>
    <p class="addr">
      📍 <b>Army Arena Shopping Complex, Bolade, Oshodi, Lagos</b><br>
      Shop EU 14/03
    </p>
    <p class="hours">⚡ 24/7 Support — We reply fast</p>
    <div class="btn-row" style="justify-content:center;margin-top:30px;">
      <a class="btn btn-wa" href="https://wa.me/2349030087669" target="_blank" rel="noopener">💬 Chat on WhatsApp</a>
    </div>
    <div class="flyer-box">
      <img src="maytech-flyer.jpg" alt="MAYTECH Solutions official flyer">
    </div>
  </div>
</section>

<footer>
  <div class="slogan">Your Tech, Our Priority</div>
  <p>© 2026 MAYTECH Solutions — TV &amp; Console Repair Services, Lagos, Nigeria</p>
</footer>

<a class="wa-float" href="https://wa.me/2349030087669" target="_blank" rel="noopener" aria-label="WhatsApp">
  <svg viewBox="0 0 32 32"><path d="M16 3C9.4 3 4 8.4 4 15c0 2.4.7 4.6 2 6.5L4 29l7.7-2c1.9 1 3.9 1.5 6 1.5h.3c6.6 0 12-5.4 12-12S22.6 3 16 3zm0 22c-1.9 0-3.7-.5-5.3-1.5l-.4-.2-4.6 1.2 1.2-4.4-.3-.4C5.6 18.2 5 16.6 5 15 5 9 9.9 4.9 16 4.9S27 9 27 15s-4.9 10-11 10zm6-7.5c-.3-.2-1.9-.9-2.2-1-.3-.1-.5-.2-.7.2-.2.3-.8 1-.9 1.2-.2.2-.4.2-.7.1-.3-.2-1.4-.5-2.6-1.6-1-.9-1.6-1.9-1.8-2.3-.2-.3 0-.5.1-.7l.5-.6c.2-.2.2-.3.3-.6.1-.2.1-.4 0-.6-.1-.2-.7-1.8-1-2.4-.3-.6-.5-.5-.7-.6h-.6c-.2 0-.6.1-.9.4-.3.3-1.1 1.1-1.1 2.7s1.2 3.1 1.3 3.4c.2.2 2.3 3.5 5.6 4.9.8.3 1.4.5 1.9.7.8.2 1.5.2 2.1.1.6-.1 1.9-.8 2.2-1.5.3-.8.3-1.4.2-1.5-.1-.2-.3-.3-.6-.4z"/></svg>
</a>

<script>
document.getElementById('bookingForm').addEventListener('submit', function(e){
  e.preventDefault();
  var name   = document.getElementById('bname').value.trim();
  var phone  = document.getElementById('bphone').value.trim();
  var device = document.getElementById('bdevice').value;
  var brand  = document.getElementById('bbrand').value || 'Not specified';
  var model  = document.getElementById('bmodel').value.trim() || 'Not specified';
  var issue  = document.getElementById('bissue').value.trim();

  var msg =
    'Hello MAYTECH Solutions! I would like to book a repair.\n\n' +
    '👤 Name: ' + name + '\n' +
    '📞 Phone: ' + phone + '\n' +
    '📺 Device: ' + device + '\n' +
    '🏷️ Brand: ' + brand + '\n' +
    '🔢 Model: ' + model + '\n' +
    '⚠️ Problem: ' + issue + '\n\n' +
    '(Sent from the MAYTECH website)';

  window.open('https://wa.me/2349030087669?text=' + encodeURIComponent(msg), '_blank');
});
</script>

</body>
</html>
