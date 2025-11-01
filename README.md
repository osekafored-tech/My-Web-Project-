<html lang="en">
<head>
  theme: jekyll-theme-minimal.
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>PureAura Perfumes — Signature Scents for Every Mood</title>
  <meta name="description" content="PureAura premium perfumes — long-lasting, unique fragrances. Order now with free delivery."/>
  <style>
    /* --------- Basic Reset & Type --------- */
    :root{
      --accent:#B76E79;
      --accent-dark:#8f4953;
      --muted:#666;
      --bg:#fbfafb;
      --card:#fff;
      --glass: rgba(255,255,255,0.8);
      --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:Inter, system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial;
      background: linear-gradient(180deg, #fff 0%, #fbf6f8 35%, #fff 100%);
      color:#222;
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      padding-bottom:120px;
    }
    a{color:var(--accent); text-decoration:none}
    img{max-width:100%; display:block}

    /* ---------- Layout ---------- */
    .wrap{max-width:var(--maxw); margin:28px auto; padding:20px;}
    header{display:flex; align-items:center; justify-content:space-between; gap:16px}
    .brand{display:flex; gap:12px; align-items:center}
    .logo{
      width:56px; height:56px; border-radius:12px;
      background:linear-gradient(135deg,var(--accent),var(--accent-dark));
      color:white; display:flex; align-items:center; justify-content:center;
      font-weight:700; font-size:18px; box-shadow:0 6px 20px rgba(183,110,121,0.15);
    }
    nav{display:flex; gap:12px; align-items:center}
    nav a.button{
      background:var(--accent); color:#fff; padding:10px 14px; border-radius:10px; font-weight:600;
      box-shadow:0 6px 18px rgba(143,73,83,0.12);
    }

    /* ---------- Hero ---------- */
    .hero{
      display:flex; gap:30px; align-items:center; padding:28px; margin-top:18px;
      background: linear-gradient(90deg, rgba(255,255,255,0.6), rgba(255,255,255,0.6));
      border-radius:18px; box-shadow:0 12px 30px rgba(0,0,0,0.05);
    }
    .hero-left{flex:1}
    .eyebrow{color:var(--muted); font-size:14px; margin-bottom:8px}
    h1{margin:0 0 12px; font-size:32px; line-height:1.05}
    p.lead{margin:0 0 18px; color:var(--muted)}
    .price{font-weight:800; font-size:22px; margin-right:8px}
    .offer-bubble{display:inline-block; background:linear-gradient(90deg,#ffecec,#fff4f6); padding:8px 12px; border-radius:12px; border:1px solid rgba(183,110,121,0.1); font-weight:700; color:var(--accent-dark)}

    .hero-cta{display:flex; gap:12px; align-items:center; margin-top:10px}
    .btn-primary{background:var(--accent); color:white; padding:12px 18px; border-radius:12px; font-weight:700; border:none; cursor:pointer}
    .btn-ghost{background:transparent; border:2px solid var(--accent); color:var(--accent-dark); padding:10px 14px; border-radius:12px; cursor:pointer}

    .hero-right{width:360px; display:flex; justify-content:center}
    .perfume-card{background:var(--card); padding:18px; border-radius:16px; width:320px; text-align:center; box-shadow:0 10px 28px rgba(0,0,0,0.06)}
    .perfume-photo{height:260px; border-radius:12px; background:linear-gradient(180deg,#fff,#fff); display:flex; align-items:center; justify-content:center; overflow:hidden;}
    .stars{margin-top:8px; color:gold}

    /* ---------- Sections ---------- */
    .grid{display:grid; grid-template-columns:repeat(3,1fr); gap:18px; margin-top:24px}
    .card{background:var(--card); padding:18px; border-radius:12px; box-shadow:0 6px 18px rgba(0,0,0,0.04)}
    .center{text-align:center}

    /* ---------- Sticky bottom bar ---------- */
    .sticky-order{
      position:fixed; left:50%; transform:translateX(-50%); bottom:18px; z-index:9999;
      width:min(980px,calc(100% - 36px));
      display:flex; align-items:center; justify-content:space-between; gap:12px; padding:12px;
      background:linear-gradient(90deg,#fff,#fff); border-radius:14px; box-shadow:0 20px 50px rgba(0,0,0,0.12);
      border:1px solid rgba(0,0,0,0.04);
    }
    .sticky-order img{height:58px; width:58px; border-radius:10px; object-fit:cover}
    .sticky-order .info{flex:1; padding-left:8px}
    .small{font-size:13px; color:var(--muted)}

    /* ---------- Modal & overlay ---------- */
    .modal-backdrop{position:fixed; inset:0; background:rgba(0,0,0,0.45); display:none; align-items:center; justify-content:center; z-index:10000}
    .modal{background:var(--card); padding:18px; border-radius:12px; width:min(720px,96%); max-height:92vh; overflow:auto}
    form.row{display:flex; gap:8px; align-items:center; flex-wrap:wrap}
    input[type="text"], input[type="email"], input[type="tel"], select{padding:10px 12px; border-radius:8px; border:1px solid #eee; width:100%}

    /* ---------- Footer ---------- */
    footer{margin-top:40px; padding:18px 8px; text-align:center; color:var(--muted); font-size:14px}

    /* ---------- Responsive ---------- */
    @media (max-width:900px){
      .hero{flex-direction:column; align-items:center}
      .grid{grid-template-columns:repeat(1,1fr)}
      .hero-right{width:100%}
      header{gap:8px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">PA</div>
        <div>
          <div style="font-weight:700">PureAura</div>
          <div style="font-size:13px; color:var(--muted)">Signature Perfumes • Free delivery</div>
        </div>
      </div>
      <nav>
        <a href="#products">Products</a>
        <a href="#reviews">Reviews</a>
        <a class="button" id="openOrderTop">Order Now</a>
      </nav>
    </header>

    <section class="hero" aria-label="hero">
      <div class="hero-left">
        <div class="eyebrow">Limited stock — first 100 orders get a free sample</div>
        <h1>Discover your signature scent — long-lasting, luxury perfumes</h1>
        <p class="lead">PureAura crafts unique blends that last all day. Choose your scent, order now and enjoy free delivery.</p>

        <div style="display:flex;align-items:center;gap:12px">
          <div class="offer-bubble">Save ₦2,500 — Intro Price</div>
          <div style="margin-left:auto; display:flex; gap:8px; align-items:center">
            <div class="price">₦6,990</div>
            <div style="text-decoration:line-through; color:var(--muted)">₦9,490</div>
          </div>
        </div>

        <div class="hero-cta">
          <button class="btn-primary" id="openOrder">Order Now</button>
          <button class="btn-ghost" id="openInfo">How it works</button>
        </div>

        <div style="margin-top:14px; color:var(--muted); font-size:14px">
          <strong>Fast delivery</strong> — 24–72 hours in major cities. Cash on delivery available.
        </div>
      </div>

      <div class="hero-right">
        <div class="perfume-card">
          <div class="perfume-photo">
            <img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="Perfume bottle">
          </div>
          <h3 style="margin:12px 0 0">PureAura — Rose Amber</h3>
          <div class="stars">★★★★★ (4.9)</div>
          <div style="margin-top:8px; color:var(--muted); font-size:14px">100ml • Long lasting • Compliment magnet</div>
        </div>
      </div>
    </section>

    <!-- Features -->
    <section id="products" style="margin-top:24px">
      <div style="display:flex; justify-content:space-between; align-items:center">
        <h2 style="margin:0">Why customers love PureAura</h2>
        <div style="color:var(--muted)">Secure checkout • Free samples • 7-day return</div>
      </div>

      <div class="grid" style="margin-top:12px">
        <div class="card center">
          <h3>Premium Ingredients</h3>
          <p class="small">Natural essences blended by expert perfumers.</p>
        </div>
        <div class="card center">
          <h3>Long-lasting</h3>
          <p class="small">Wear it in the morning, smell it at night.</p>
        </div>
        <div class="card center">
          <h3>Free delivery</h3>
          <p class="small">We ship fast across Nigeria — COD available.</p>
        </div>
      </div>
    </section>

    <!-- Reviews -->
    <section id="reviews" style="margin-top:26px">
      <h2>Real customers, real stories</h2>
      <div class="grid" style="margin-top:12px">
        <div class="card">
          <strong>Amaka, Lagos</strong>
          <p class="small">“My colleagues kept asking what I was wearing — lasted all day even after church.”</p>
        </div>
        <div class="card">
          <strong>Grace, Abuja</strong>
          <p class="small">“Nice smooth scent. Fast delivery and the free sample was a sweet surprise.”</p>
        </div>
        <div class="card">
          <strong>Uche, PH</strong>
          <p class="small">“Quality bottle, luxury feel — I bought 3 after trying one.”</p>
        </div>
      </div>
    </section>

    <!-- FAQ -->
    <section style="margin-top:26px">
      <h2>FAQ</h2>
      <div style="display:grid; gap:10px; margin-top:10px">
        <details><summary style="cursor:pointer; font-weight:700">How long is delivery?</summary>
          <div class="small" style="margin-top:8px">Usually 24–72 hours in major cities. Rural areas may take longer.</div>
        </details>
        <details><summary style="cursor:pointer; font-weight:700">Can I pay on delivery?</summary>
          <div class="small" style="margin-top:8px">Yes — cash on delivery (COD) is available for most locations.</div>
        </details>
      </div>
    </section>

    <footer>
      © <span id="year"></span> PureAura • Contact: +234 800 123 4567 • Follow us on Facebook
    </footer>
  </div>

  <!-- Sticky bottom order bar -->
  <div class="sticky-order" aria-hidden="false">
    <img src="https://images.unsplash.com/photo-1522335789203-aabd1fc54bc9?q=80&w=1200&auto=format&fit=crop&ixlib=rb-4.0.3&s=placeholder" alt="bottle">
    <div class="info">
      <div style="font-weight:700">PureAura — Rose Amber</div>
      <div class="small">₦6,990 — Limited stock</div>
    </div>
    <div style="display:flex; gap:10px;">
      <button class="btn-ghost" id="openChat">Chat</button>
      <button class="btn-primary" id="openOrderSticky">Buy now</button>
    </div>
  </div>

  <!-- Modal: Order -->
  <div class="modal-backdrop" id="modalOrder">
    <div class="modal" role="dialog" aria-modal="true" aria-labelledby="orderTitle">
      <h2 id="orderTitle">Place your order — PureAura Rose Amber</h2>
      <p class="small">Fill the details below. We will call to confirm and schedule delivery.</p>

      <form id="orderForm" style="margin-top:10px">
        <div class="row">
          <div style="flex:1">
            <label for="name">Full name</label>
            <input id="name" name="name" type="text" placeholder="e.g. Amina Olawale" required>
          </div>
          <div style="flex:1">
            <label for="phone">Phone (WhatsApp)</label>
            <input id="phone" name="phone" type="tel" placeholder="+2348012345678" required>
          </div>
        </div>

        <div style="margin-top:8px">
          <label for="address">Delivery address</label>
          <input id="address" name="address" type="text" placeholder="House, Street, City" required>
        </div>

        <div style="margin-top:8px" class="row">
          <div style="flex:1">
            <label for="qty">Quantity</label>
            <select id="qty" name="qty" required>
              <option value="1">1 bottle — ₦6,990</option>
              <option value="2">2 bottles — ₦12,980 (save ₦1,000)</option>
              <option value="3">3 bottles — ₦18,000 (save ₦2,970)</option>
            </select>
          </div>
          <div style="flex:1">
            <label for="pay">Payment</label>
            <select id="pay" name="pay" required>
              <option>Cash on Delivery</option>
              <option>Bank Transfer</option>
              <option>Mobile Pay</option>
            </select>
          </div>
        </div>

        <div style="display:flex; gap:8px; margin-top:12px; justify-content:flex-end">
          <button type="button" class="btn-ghost" id="closeModal">Cancel</button>
          <button type="submit" class="btn-primary">Confirm order</button>
        </div>
      </form>
    </div>
  </div>

  <!-- Modal: Info / How it works -->
  <div class="modal-backdrop" id="modalInfo">
    <div class="modal">
      <h2>How PureAura works</h2>
      <p class="small">Every bottle is blended in small batches. We test scent long-lasting performance and include a complimentary sample for early buyers.</p>
      <ul class="small">
        <li>100ml bottles, premium packaging</li>
        <li>Free delivery on orders above ₦10,000</li>
        <li>7-day satisfaction return policy</li>
      </ul>
      <div style="display:flex; justify-content:flex-end; margin-top:12px">
        <button class="btn-primary" id="closeInfo">Close</button>
      </div>
    </div>
  </div>

  <!-- Cookie / consent -->
  <div id="cookieBanner" style="position:fixed; left:16px; right:16px; bottom:86px; z-index:9998; display:none; margin:auto; max-width:800px;">
    <div style="background:var(--glass); padding:12px; border-radius:10px; display:flex; justify-content:space-between; align-items:center; gap:12px; box-shadow:0 10px 30px rgba(0,0,0,0.08)">
      <div>
        <div style="font-weight:700">We use cookies</div>
        <div class="small">To keep orders simple and save your preferences.</div>
      </div>
      <div style="display:flex; gap:8px">
        <button class="btn-ghost" id="declineCookies">Decline</button>
        <button class="btn-primary" id="acceptCookies">Accept</button>
      </div>
    </div>
  </div>

  <!-- Thank you overlay (shown after order submit) -->
  <div class="modal-backdrop" id="modalThanks">
    <div class="modal center">
      <h2>Thanks — order received</h2>
      <p class="small">We will call you soon to confirm details. Your order number: <strong id="orderNo">#</strong></p>
      <div style="margin-top:12px; display:flex; justify-content:center">
        <button class="btn-primary" id="closeThanks">Close</button>
      </div>
    </div>
  </div>

  <script>
    // Basic handlers & fake submit
    document.getElementById('year').textContent = new Date().getFullYear();

    const modalOrder = document.getElementById('modalOrder');
    const modalInfo = document.getElementById('modalInfo');
    const modalThanks = document.getElementById('modalThanks');

    function showModal(el){ el.style.display = 'flex'; document.body.style.overflow='hidden' }
    function hideModal(el){ el.style.display = 'none'; document.body.style.overflow='' }

    document.getElementById('openOrder').addEventListener('click', ()=> showModal(modalOrder));
    document.getElementById('openOrderTop').addEventListener('click', ()=> showModal(modalOrder));
    document.getElementById('openOrderSticky').addEventListener('click', ()=> showModal(modalOrder));
    document.getElementById('closeModal').addEventListener('click', ()=> hideModal(modalOrder));
    document.getElementById('openInfo').addEventListener('click', ()=> showModal(modalInfo));
    document.getElementById('closeInfo').addEventListener('click', ()=> hideModal(modalInfo));

    // Chat button behavior (example - open WhatsApp)
    document.getElementById('openChat').addEventListener('click', ()=>{
      const phone = '+2348001234567';
      const text = encodeURIComponent('Hi PureAura — I would like to ask about your Rose Amber perfume.');
      window.open('https://wa.me/' + phone.replace(/\D/g,'') + '?text=' + text, '_blank');
    });

    // Cookie banner show once
    if(!localStorage.getItem('pureaura_cookies')){
      document.getElementById('cookieBanner').style.display='block';
    }
    document.getElementById('acceptCookies').addEventListener('click', ()=>{
      localStorage.setItem('pureaura_cookies','accepted'); document.getElementById('cookieBanner').style.display='none';
    });
    document.getElementById('declineCookies').addEventListener('click', ()=> {
      localStorage.setItem('pureaura_cookies','declined'); document.getElementById('cookieBanner').style.display='none';
    });

    // Order form: fake submit (client-only)
    document.getElementById('orderForm').addEventListener('submit', function(e){
      e.preventDefault();
      // Simple validation
      const name = this.name.value.trim();
      const phone = this.phone.value.trim();
      if(!name || !phone){ alert('Please enter name and phone'); return; }

      // show thanks with fake order number
      hideModal(modalOrder);
      const num = 'PA' + Math.floor(100000 + Math.random()*900000);
      document.getElementById('orderNo').textContent = num;
      showModal(modalThanks);

      // Simulate sending data to server:
      // TODO: Replace with real POST / webhook that saves orders.
      console.log('ORDER (simulate):', {
        name: this.name.value, phone: this.phone.value, address: this.address.value, qty: this.qty.value, pay: this.pay.value
      });
    });

    document.getElementById('closeThanks').addEventListener('click', ()=> hideModal(modalThanks));

    // Allow backdrop click to close modals
    document.querySelectorAll('.modal-backdrop').forEach(back => {
      back.addEventListener('click', (ev)=>{
        if(ev.target === back){ hideModal(back); }
      });
    });

    // Accessibility escape key to close modals
    document.addEventListener('keydown', (ev)=>{
      if(ev.key === 'Escape'){
        document.querySelectorAll('.modal-backdrop').forEach(back => hideModal(back));
      }
    });

    // show cookie banner after short delay (if not set)
    setTimeout(()=> {
      if(!localStorage.getItem('pureaura_cookies')) document.getElementById('cookieBanner').style.display = 'block';
    }, 1000);

  </script>
</body>
</html>
 
