# andrre7849.github.io
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>Rivera's Mobile Detail — Professional Mobile Detailing</title>
  <meta name="description" content="Rivera's Mobile Detail — Mobile car detailing, ceramic coatings, interior deep clean. We come to you. Proudly serving The IE." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;600;700&display=swap" rel="stylesheet">
  <style>
    :root{
      --bg:#0f1724;
      --card:#0b1220;
      --muted:#94a3b8;
      --accent:#0ea5a4;
      --accent-2:#06b6d4;
      --glass: rgba(255,255,255,0.03);
      --radius:12px;
      --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      font-family:Inter,system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      margin:0;background:linear-gradient(180deg,#071021 0%, #071827 60%);color:#e6eef6;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      line-height:1.45;
      padding:24px;
      display:flex;
      justify-content:center;
    }
    .wrap{width:100%;max-width:var(--maxw);}

    /* header */
    header{display:flex;align-items:center;justify-content:space-between;margin-bottom:22px}
    .brand{display:flex;gap:12px;align-items:center}
    .logo{width:52px;height:52px;border-radius:10px;background:linear-gradient(135deg,var(--accent),var(--accent-2));display:flex;align-items:center;justify-content:center;font-weight:700;color:#042029}
    .brand h1{font-size:18px;margin:0}
    .cta{display:flex;gap:10px;align-items:center}
    .btn{
      background:linear-gradient(90deg,var(--accent),var(--accent-2));border:0;color:#032023;padding:10px 14px;border-radius:10px;font-weight:600;text-decoration:none;
      box-shadow:0 6px 18px rgba(6,182,212,0.12);
    }
    .btn.secondary{background:transparent;border:1px solid rgba(255,255,255,0.06);color:var(--muted);padding:8px 12px}

    /* hero */
    .hero{display:grid;grid-template-columns:1fr 380px;gap:28px;align-items:start;margin-bottom:26px}
    .hero-left h2{font-size:28px;margin:0 0 8px}
    .hero-left p{color:var(--muted);margin:0 0 18px}
    .features{display:flex;gap:12px;flex-wrap:wrap}
    .chip{background:var(--glass);padding:8px 12px;border-radius:999px;color:var(--muted);font-weight:600;font-size:13px}

    .card{background:linear-gradient(180deg, rgba(255,255,255,0.02), rgba(255,255,255,0.01));padding:18px;border-radius:var(--radius);box-shadow:0 6px 30px rgba(2,6,23,0.6);}

    /* booking */
    .booking h3{margin:0 0 8px}
    label{display:block;font-size:13px;color:var(--muted);margin-top:10px}
    input[type=text], input[type=email], input[type=tel], select, textarea{
      width:100%;padding:10px;border-radius:8px;border:1px solid rgba(255,255,255,0.04);background:transparent;color:inherit;
      margin-top:6px;font-size:14px;
    }
    textarea{min-height:90px;resize:vertical}
    .small{font-size:13px;color:var(--muted);margin-top:8px}

    /* services */
    .grid{display:grid;grid-template-columns:repeat(3,1fr);gap:14px;margin:18px 0}
    .service{padding:14px;border-radius:12px;background:linear-gradient(180deg, rgba(255,255,255,0.01), rgba(255,255,255,0.02));}
    .price{font-weight:700;color:var(--accent);font-size:18px;margin-top:8px}

    /* gallery */
    .gallery{display:grid;grid-template-columns:repeat(4,1fr);gap:8px}
    .gallery img{width:100%;height:120px;object-fit:cover;border-radius:8px;display:block;cursor:pointer;opacity:0.98}

    /* testimonials */
    .testimonials{display:flex;gap:12px;flex-wrap:wrap}
    .tcard{background:rgba(255,255,255,0.02);padding:12px;border-radius:10px;flex:1 1 240px}

    footer{margin-top:26px;padding:14px;border-radius:10px;background:transparent;color:var(--muted);display:flex;justify-content:space-between;align-items:center}

    /* responsive */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr;gap:12px}
      .grid{grid-template-columns:repeat(2,1fr)}
      .gallery{grid-template-columns:repeat(3,1fr)}
    }
    @media (max-width:620px){
      body{padding:14px}
      .grid{grid-template-columns:1fr}
      .gallery{grid-template-columns:repeat(2,1fr)}
      header{flex-direction:column;align-items:flex-start;gap:10px}
    }

    /* lightbox */
    .lightbox{
      position:fixed;inset:0;display:none;align-items:center;justify-content:center;background:rgba(2,6,23,0.75);z-index:80;
    }
    .lightbox img{max-width:92%;max-height:86%;border-radius:10px}
    .close-x{position:absolute;top:18px;right:18px;color:#fff;font-weight:700;cursor:pointer;padding:8px 10px;border-radius:8px;background:rgba(255,255,255,0.06)}
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">RD</div>
        <div>
          <h1>Rivera's Mobile Detailing</h1>
          <div style="font-size:13px;color:var(--muted)">Mobile detailing • Ceramic • Interior • We come to you</div>
        </div>
      </div>
      <div class="cta">
        <a class="btn" href="#booking">Book now</a>
        <a class="btn secondary" href="#services">Services</a>
      </div>
    </header>

    <section class="hero">
      <div class="hero-left">
        <h2>Professional mobile detailing that comes to you</h2>
        <p>Fast, reliable, and protective detailing — from express washes to full ceramic coatings. Serving Bloomington & surrounding areas. Save time, skip the line.</p>

        <div class="features">
          <div class="chip">Steaming</div>
          <div class="chip">Mobile • On-site</div>
          <div class="chip">Ceramic Coating</div>
          <div class="chip">Interior Deep Clean</div>
          <div class="chip">Fleet & Recurring</div>
        </div>

        <div style="margin-top:18px" class="card">
          <strong>Why choose us</strong>
          <ul style="color:var(--muted);margin:8px 0 0;padding-left:18px">
            <li>Fast turnaround — most cars in 60–90 minutes</li>
            <li>Eco-friendly products & water-efficient methods</li>
            <li>Experience with mobile setups and secure mounts</li>
          </ul>
        </div>
      </div>

      <aside class="card booking" id="booking">
        <h3>Quick book</h3>
        <p class="small">Fill this form or call <strong>(909) 640-0063</strong></p>

        <!-- Replace FORM_ACTION with your Formspree endpoint or server -->
        <form id="bookForm" action="https://formspree.io/f/your-form-id" method="POST">
          <label for="name">Full name</label>
          <input id="name" name="name" type="text" required placeholder="Your name" />
          <label for="phone">Phone</label>
          <input id="phone" name="phone" type="tel" required placeholder="(555) 555-5555" />
          <label for="email">Email</label>
          <input id="email" name="email" type="email" placeholder="you@example.com" />
          <label for="service">Service</label>
          <select id="service" name="service">
            <option>Express Wash — Exterior</option>
            <option>Full Detail — Interior & Exterior</option>
            <option>Ceramic Coating — Single Stage</option>
          </select>
          <label for="date">Preferred date/time</label>
          <input id="date" name="date" type="text" placeholder="June 30, 2pm" />
          <label for="notes">Address / Notes</label>
          <textarea id="notes" name="notes" placeholder="Address, car make/model, notes"></textarea>

          <div style="display:flex;gap:8px;margin-top:12px">
            <button class="btn" type="submit">Request booking</button>
            <button class="btn secondary" type="button" onclick="window.location='tel:+15555555555'">Call now</button>
          </div>

          <div id="formMsg" class="small" style="display:none;margin-top:10px"></div>
        </form>

        <div class="small" style="margin-top:12px">Pro tip: For best results, park in a shaded area and remove personal items from the vehicle.</div>
      </aside>
    </section>

    <section id="services" style="margin-top:6px">
      <h3 style="margin:0 0 8px">Services &  Estimated Pricing</h3>
      <div class="grid">
        <div class="service card">
          <h4>Express Exterior</h4>
          <div class="price">$55-$70</div>
          <p style="color:var(--muted)">Quick wash, wheel clean, tire dressing, exterior wipe-down. Great for weekly maintenance.</p>
        </div>

        <div class="service card">
          <h4>Full Detail</h4>
          <div class="price">$140 – $200</div>
          <p style="color:var(--muted)">Exterior wash, clay bar, polish, interior vacuum, shampoo, trim dress. Most popular.</p>
        </div>

        <div class="service card">
          <h4>Ceramic Coating</h4>
          <div class="price">$399+</div>
          <p style="color:var(--muted)">Long-lasting protection. Price varies by vehicle size & prep needed.</p>
        </div>

        <div class="service card">
          <h4>Interior Deep Clean</h4>
          <div class="price">$100 – $160</div>
          <p style="color:var(--muted)">Steam cleaning, stain removal, leather conditioning.</p>
        </div>

        <div class="service card">
          <h4>Headlight Restoration</h4>
          <div class="price">$60</div>
          <p style="color:var(--muted)">Restore clarity & brightness, protectant included.</p>
        </div>

        <div class="service card">
          <h4>Fleet / Subscription</h4>
          <div class="price">Contact for quote</div>
          <p style="color:var(--muted)">Volume discounts and scheduled maintenance packages available.</p>
        </div>
      </div>
    </section>


    <section style="margin-top:18px">
      <h3 style="margin-bottom:8px">What clients say</h3>
      <div class="testimonials">
        <div class="tcard card">
          <strong>Isaac T.</strong>
          <p style="color:var(--muted)">“Came to my house, great communication, my car looked brand new. Highly recommend.”</p>
        </div>
        <div class="tcard card">
          <strong>Maria L.</strong>
          <p style="color:var(--muted)">“Fast, friendly, and thorough. The ceramic coating made my paint look better than before.”</p>
        </div>
      </div>
    </section>

    <footer>
      <div>
        <strong>Rivera's Mobile Detailing</strong> • (909) 640-0063 • <a href="mailto:andrre7849r@gmail.com" style="color:inherit">andrre7849r@gmail.com</a>
      </div>
      <div style="font-size:13px;color:var(--muted)">Proudly serving the IE</div>
    </footer>
  </div>

  <!-- Lightbox -->
  <div class="lightbox" id="lightbox" role="dialog" aria-hidden="true">
    <div class="close-x" id="lbClose">✕</div>
    <img src="" alt="gallery large" id="lbImg" />
  </div>

  <script>
    // LIGHTBOX
    document.querySelectorAll('#gallery img').forEach(img=>{
      img.addEventListener('click', ()=>{
        const src = img.dataset.full || img.src;
        const lb = document.getElementById('lightbox');
        document.getElementById('lbImg').src = src;
        lb.style.display = 'flex';
        lb.setAttribute('aria-hidden','false');
      });
    });
    document.getElementById('lbClose').addEventListener('click', ()=> {
      const lb = document.getElementById('lightbox');
      lb.style.display = 'none';
      lb.setAttribute('aria-hidden','true');
    });
    document.getElementById('lightbox').addEventListener('click', (e)=>{
      if(e.target.id === 'lightbox') { e.currentTarget.style.display='none'; }
    });

    // Simple form submit UX (works with Formspree or similar)
    const form = document.getElementById('bookForm');
    const msg = document.getElementById('formMsg');
    form.addEventListener('submit', (ev)=>{
      msg.style.display = 'block';
      msg.textContent = 'Sending...';
      // If you use Formspree, the action will POST and redirect/return status.
      // We show a friendly message and let the default submit proceed.
      setTimeout(()=> {
        msg.textContent = 'If you don’t see a confirmation, call (555) 555-5555.';
      },1200);
    });

    // small accessibility: focus trap on lightbox via Escape
    window.addEventListener('keydown', (e)=> {
      if(e.key === 'Escape') {
        const lb = document.getElementById('lightbox');
        if(lb.style.display === 'flex') lb.style.display = 'none';
      }
    });
  </script>
</body>
</html>
