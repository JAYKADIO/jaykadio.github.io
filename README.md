<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Jay — Portfolio</title>
  <meta name="description" content="Jay — Poster & Branding Designer | I fix what your eyes complain about.">
  <style>
    :root{
      --bg:#0b0f14; --card:#0f1418; --muted:#94a3b8; --accent:#7c5cff; --glass:rgba(255,255,255,0.04);
      --maxw:1100px; --radius:14px; --gap:22px; --fs:16px;
    }
    *{box-sizing:border-box}
    html,body{height:100%;margin:0;font-family:Inter,ui-sans-serif,system-ui,Arial; background:linear-gradient(180deg,#05060a 0%,#081018 100%);color:#e6eef8;font-size:var(--fs)}
    a{color:inherit;text-decoration:none}

    .wrap{max-width:var(--maxw);margin:40px auto;padding:28px}

    /* Header */
    header{display:flex;align-items:center;justify-content:space-between;gap:12px;margin-bottom:28px}
    .brand{display:flex;align-items:center;gap:12px}
    .logo{width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),#3ad6ff);display:flex;align-items:center;justify-content:center;font-weight:700;color:#081018}
    .title h1{margin:0;font-size:20px;letter-spacing:0.6px}
    .title p{margin:0;font-size:13px;color:var(--muted)}
    nav{display:flex;gap:14px}
    .btn{padding:8px 12px;border-radius:10px;background:transparent;border:1px solid rgba(255,255,255,0.06);cursor:pointer}

    /* Hero */
    .hero{display:grid;grid-template-columns:1fr 420px;gap:28px;align-items:center;margin-bottom:30px}
    .hero-card{background:linear-gradient(180deg,rgba(255,255,255,0.02),transparent);padding:28px;border-radius:var(--radius);backdrop-filter:blur(6px);border:1px solid rgba(255,255,255,0.03)}
    .hero h2{margin:0 0 12px 0;font-size:28px}
    .hero p{margin:0;color:var(--muted);line-height:1.6}
    .slogan{display:inline-block;margin-top:14px;padding:8px 12px;border-radius:999px;background:linear-gradient(90deg,rgba(124,92,255,0.16),rgba(58,214,255,0.08));border:1px solid rgba(124,92,255,0.12);font-weight:600}

    /* Gallery */
    .section-title{margin:18px 0 12px;color:var(--muted);font-size:13px}
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:var(--gap)}
    .card{background:var(--card);border-radius:12px;overflow:hidden;border:1px solid rgba(255,255,255,0.03);cursor:pointer}
    .card img{width:100%;height:230px;object-fit:cover;display:block}
    .card .meta{padding:12px}
    .meta h4{margin:0 0 6px 0;font-size:15px}
    .meta p{margin:0;color:var(--muted);font-size:13px}

    /* Branding set */
    .branding{display:grid;grid-template-columns:1fr 320px;gap:18px;align-items:start}
    .mockups{display:flex;flex-direction:column;gap:12px}
    .mock{background:var(--glass);padding:12px;border-radius:10px;border:1px solid rgba(255,255,255,0.03)}

    /* Modal */
    .modal{position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:linear-gradient(0deg,rgba(2,6,11,0.6),rgba(2,6,11,0.6));z-index:100}
    .modal.show{display:flex}
    .modal .panel{width:min(1100px,95%);max-height:90%;overflow:auto;background:#071018;padding:18px;border-radius:12px;border:1px solid rgba(255,255,255,0.04)}
    .modal img{width:100%;height:auto;display:block;border-radius:8px}
    .modal .close{margin-top:12px;display:flex;justify-content:flex-end}

    /* Footer */
    footer{margin-top:30px;color:var(--muted);font-size:14px;text-align:center;padding:18px}

    /* Responsive */
    @media (max-width:1000px){.hero{grid-template-columns:1fr} .grid{grid-template-columns:repeat(2,1fr)} }
    @media (max-width:640px){.grid{grid-template-columns:1fr} .logo{width:48px;height:48px} .hero{gap:16px} .hero h2{font-size:22px}}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">J</div>
        <div class="title"><h1>Jay — Poster & Branding</h1><p>Creative Communication Design • Bangkok University</p></div>
      </div>
      <nav>
        <a class="btn" href="#portfolio">Portfolio</a>
        <a class="btn" href="#branding">Branding</a>
        <a class="btn" href="#contact">Contact</a>
      </nav>
    </header>

    <section class="hero">
      <div class="hero-card">
        <h2>Creative layout • Dark mode</h2>
        <p>Hi — I’m Jay, 22. I design posters, branding, and visual identities for esports and creative projects. I work mostly with Photoshop & Illustrator and bring concepts to life with strong composition and bold color.</p>
        <div class="slogan">I fix what your eyes complain about.</div>
      </div>

      <div>
        <div class="hero-card">
          <h3 style="margin-top:0">Quick facts</h3>
          <p style="margin:6px 0">• 6 months full-time at an esports org (Myanmar)<br>• Freelance poster & branding projects<br>• Photoshop · Illustrator · Figma</p>
        </div>
        <div style="height:18px"></div>
        <div class="hero-card">
          <h3 style="margin-top:0">Contact</h3>
          <p style="margin:6px 0">Email: <a href="mailto:your-email@example.com">your-email@example.com</a><br>Instagram / TikTok / YouTube: @yourhandle</p>
        </div>
      </div>
    </section>

    <h3 class="section-title">Featured Posters</h3>
    <div id="portfolio" class="grid">
      <!-- Replace the src paths below with your uploaded images inside repo (images/poster1.jpg etc.) -->
      <div class="card" data-full="/images/poster1.jpg"><img src="/images/poster1.jpg" alt="Poster 1"><div class="meta"><h4>Poster 1 — Lumina Typography</h4><p>Poster / Typography</p></div></div>
      <div class="card" data-full="/images/poster2.jpg"><img src="/images/poster2.jpg" alt="Poster 2"><div class="meta"><h4>Poster 2 — Hope</h4><p>Concept Poster</p></div></div>
      <div class="card" data-full="/images/poster3.jpg"><img src="/images/poster3.jpg" alt="Poster 3"><div class="meta"><h4>Poster 3 — Esport Night</h4><p>Event Poster</p></div></div>
      <div class="card" data-full="/images/poster4.jpg"><img src="/images/poster4.jpg" alt="Poster 4"><div class="meta"><h4>Poster 4 — Butterfly Light</h4><p>Personal Project</p></div></div>
      <div class="card" data-full="/images/poster5.jpg"><img src="/images/poster5.jpg" alt="Poster 5"><div class="meta"><h4>Poster 5 — Midnight</h4><p>Music Poster</p></div></div>
      <div class="card" data-full="/images/poster6.jpg"><img src="/images/poster6.jpg" alt="Poster 6"><div class="meta"><h4>Poster 6 — Campaign</h4><p>Social Poster</p></div></div>
      <div class="card" data-full="/images/poster7.jpg"><img src="/images/poster7.jpg" alt="Poster 7"><div class="meta"><h4>Poster 7 — Neon</h4><p>Esport Concept</p></div></div>
      <div class="card" data-full="/images/poster8.jpg"><img src="/images/poster8.jpg" alt="Poster 8"><div class="meta"><h4>Poster 8 — Experiment</h4><p>Visual Study</p></div></div>
    </div>

    <h3 class="section-title">Branding — Full Set</h3>
    <section id="branding" class="branding">
      <div class="hero-card">
        <h4 style="margin-top:0">Brand: Blue Void (example)</h4>
        <p style="color:var(--muted)">A full brand set including logo, color palette, type lockups, and application examples.</p>

        <div style="display:flex;gap:10px;margin-top:12px;flex-wrap:wrap">
          <div class="mock"><strong>Logo</strong><div style="height:8px"></div><img src="/images/brand-logo.jpg" alt="Logo" style="width:140px;height:80px;object-fit:contain;border-radius:6px"></div>
          <div class="mock"><strong>Palette</strong><div style="height:8px"></div><img src="/images/brand-palette.jpg" alt="Palette" style="width:140px;height:80px;object-fit:cover;border-radius:6px"></div>
          <div class="mock"><strong>Typography</strong><div style="height:8px"></div><img src="/images/brand-type.jpg" alt="Type" style="width:140px;height:80px;object-fit:cover;border-radius:6px"></div>
        </div>

        <div style="margin-top:14px;color:var(--muted)">
          <p><strong>Deliverables</strong>: Logo, Color System, Type, Brand Guidelines PDF, Social Mockups</p>
        </div>
      </div>

      <div>
        <div class="mockups">
          <div class="mock"><img src="/images/mockup1.jpg" alt="Mockup 1" style="width:100%;height:180px;object-fit:cover;border-radius:8px"></div>
          <div class="mock"><img src="/images/mockup2.jpg" alt="Mockup 2" style="width:100%;height:180px;object-fit:cover;border-radius:8px"></div>
        </div>
      </div>
    </section>

    <h3 class="section-title">About & Contact</h3>
    <div class="hero-card">
      <h4 style="margin-top:0">About Jay</h4>
      <p style="color:var(--muted)">22-year-old Creative Communication Design student at Bangkok University. 6 months experience at an esports organization and various freelance projects. I focus on poster design and branding — delivering bold, readable visuals.</p>
      <div id="contact" style="margin-top:12px">
        <p style="color:var(--muted)"><strong>Email:</strong> your-email@example.com • <strong>Instagram:</strong> @yourhandle</p>
      </div>
    </div>

    <footer>© Jay • Designed & coded by Jay — I fix what your eyes complain about.</footer>
  </div>

  <!-- Modal / Lightbox -->
  <div id="modal" class="modal" role="dialog" aria-hidden="true">
    <div class="panel">
      <div id="modal-content"></div>
      <div class="close"><button id="closeBtn" class="btn">Close</button></div>
    </div>
  </div>

  <script>
    // Open image in modal
    document.querySelectorAll('.card').forEach(c=>c.addEventListener('click',()=>{
      const src = c.getAttribute('data-full') || c.querySelector('img').src;
      const panel = document.getElementById('modal');
      const content = document.getElementById('modal-content');
      content.innerHTML = '<img src="'+src+'" alt="Full image">';
      panel.classList.add('show'); panel.setAttribute('aria-hidden','false');
    }));
    document.getElementById('closeBtn').addEventListener('click',()=>{document.getElementById('modal').classList.remove('show');document.getElementById('modal').setAttribute('aria-hidden','true')});
    document.getElementById('modal').addEventListener('click',(e)=>{if(e.target.id==='modal') {document.getElementById('modal').classList.remove('show');document.getElementById('modal').setAttribute('aria-hidden','true')}})

    // Keyboard: close on ESC
    document.addEventListener('keydown',e=>{if(e.key==='Escape'){document.getElementById('modal').classList.remove('show');document.getElementById('modal').setAttribute('aria-hidden','true')}})
  </script>
</body>
</html>
