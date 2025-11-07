<!doctype html>
<html lang="id">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width,initial-scale=1" />
  <title>ChocoCream — Toko Es Krim</title>
  <meta name="description" content="ChocoCream — berbagai rasa coklat & es krim artisanal" />
  <link href="i.pinimg.com/736x/32/d3/f6/32d3f643d223441e6ffb7f4c4deb4e44.jpg" rel="stylesheet">
  <style>
    :root{
      --bg:#fffaf6;
      --card:#fff8f2;
      --accent:#7b4f39; /* coklat utama */
      --accent-2:#c77b49; /* salted caramel */
      --muted:#826b63;
      --soft:#f9eae0;
      --radius:14px;
      --maxw:1100px;
    }
    *{box-sizing:border-box}
    html,body{height:100%}
    body{
      margin:0;
      font-family:"Poppins",system-ui,-apple-system,Segoe UI,Roboto,"Helvetica Neue",Arial;
      background: linear-gradient(180deg,var(--bg),#fff3e8 90%);
      color:var(--accent);
      -webkit-font-smoothing:antialiased;
      -moz-osx-font-smoothing:grayscale;
      display:flex;
      justify-content:center;
      padding:32px 18px;
    }

    .wrap{width:100%;max-width:var(--maxw)}

/* Header */
    header{
      display:flex;align-items:center;gap:16px;padding:14px 18px;border-radius:12px;
      background:linear-gradient(90deg, rgba(123,79,57,0.06), rgba(199,123,73,0.03));
      box-shadow:0 8px 30px rgba(123,79,57,0.06);
      margin-bottom:20px;
    }
    .brand{
      display:flex;align-items:center;gap:12px;
    }
    .logo{
      width:56px;height:56px;border-radius:12px;background:linear-gradient(135deg,var(--accent),var(--accent-2));
      display:flex;align-items:center;justify-content:center;color:white;font-weight:700;font-size:20px;box-shadow:0 6px 14px rgba(0,0,0,0.08)
    }
    h1{margin:0;font-size:18px}
    .tag{font-size:13px;color:var(--muted)}

    nav{margin-left:auto;display:flex;gap:12px;align-items:center}
    nav a{color:var(--muted);text-decoration:none;padding:8px 10px;border-radius:10px;font-weight:600}
    nav a:hover{background:var(--soft);color:var(--accent)}

 /* Hero */
    .hero{
      display:grid;grid-template-columns:1fr 380px;gap:24px;align-items:center;margin-bottom:20px;
    }
    .hero-card{background:linear-gradient(180deg,var(--card),#fff);padding:28px;border-radius:16px;box-shadow:0 18px 40px rgba(123,79,57,0.06)}
    .hero h2{font-size:32px;margin:0 0 8px;color:var(--accent)}
    .lead{color:var(--muted);margin:0 0 16px}
    .cta{display:flex;gap:12px;margin-top:8px}
    .btn-primary{background:linear-gradient(90deg,var(--accent),var(--accent-2));color:white;padding:12px 16px;border-radius:12px;border:none;font-weight:700;cursor:pointer}
    .btn-ghost{background:transparent;border:1px solid rgba(123,79,57,0.08);padding:10px 14px;border-radius:12px;cursor:pointer;color:var(--accent)}

    .hero-illus{
      border-radius:14px;overflow:hidden;background:linear-gradient(180deg,#fff6f0,#fff2eb);height:300px;display:flex;flex-direction:column;align-items:center;justify-content:center;
      box-shadow:0 14px 34px rgba(123,79,57,0.05)
    }
    .hero-illus img{width:100%;height:100%;object-fit:cover;display:block}

/* Flavors (main) */
    main{display:grid;grid-template-columns:1fr;gap:20px}
    .section{padding:20px;background:linear-gradient(180deg,#fff,#fffaf6);border-radius:14px;box-shadow:0 12px 26px rgba(123,79,57,0.04)}
    .section h3{margin:0 0 12px;font-size:20px;color:var(--accent)}
    .filters{display:flex;gap:10px;flex-wrap:wrap;margin-bottom:12px}
    .chip{background:#fff4ef;padding:8px 12px;border-radius:999px;border:1px solid rgba(123,79,57,0.06);font-weight:600;color:var(--muted);cursor:pointer}
    .chip.active{background:linear-gradient(90deg,var(--accent),var(--accent-2));color:white}

    .grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(230px,1fr));gap:16px}

/* Flavor card */
    .card{
      background:linear-gradient(180deg,#fff7f3,#fff3ee);
      border-radius:12px;overflow:hidden;border:1px solid rgba(123,79,57,0.06);
      transition:transform .22s ease,box-shadow .22s ease;display:flex;flex-direction:column;
    }
    .card:hover{transform:translateY(-8px);box-shadow:0 18px 40px rgba(123,79,57,0.08)}
    .card .img{height:160px;overflow:hidden}
    .card .img img{width:100%;height:100%;object-fit:cover;display:block}
    .card .body{padding:12px;flex:1;display:flex;flex-direction:column}
    .card h4{margin:0 0 6px;font-size:16px;color:var(--accent)}
    .meta{color:var(--muted);font-size:13px;margin-bottom:8px}
    .price{margin-top:auto;font-weight:700;color:var(--accent-2)}
    .actions{display:flex;gap:8px;margin-top:10px}

/* footer / contact */
    footer{margin-top:18px;text-align:center;color:var(--muted);font-size:13px}

/* responsive */
    @media (max-width:980px){
      .hero{grid-template-columns:1fr}
      .hero-illus{height:260px}
    }
    @media (max-width:520px){
      header{flex-direction:column;align-items:flex-start;gap:10px}
      nav{align-self:stretch;display:flex;gap:8px;flex-wrap:wrap}
      .card .img{height:140px}
    }
  </style>
</head>
<body>
  <div class="wrap">
    <header>
      <div class="brand">
        <div class="logo">CC</div>
        <div>
          <h1>ChocoCream</h1>
          <div class="tag">Es krim coklat & varian spesial</div>
        </div>
      </div>

      <nav>
        <a href="#home">Beranda</a>
        <a href="#flavors">Rasa</a>
        <a href="#menu">Menu</a>
        <a href="#contact">Kontak</a>
      </nav>
    </header>

    <!-- HERO -->
    <div class="hero">
      <div class="hero-card">
        <h2 id="home">Selamat datang di ChocoCream 🍫</h2>
        <p class="lead">Surga buat pecinta coklat — puluhan varian coklat mulai dari klasik hingga kreasi unik. Pilih rasa favoritmu, pesan, dan nikmati momen manismu.</p>

        <div class="cta">
          <button class="btn-primary" onclick="document.getElementById('flavors').scrollIntoView({behavior:'smooth'})">Lihat Rasa Coklat</button>
          <button class="btn-ghost" onclick="alert('Hubungi kami di chat / email untuk pemesanan!')">Hubungi Kami</button>
        </div>

        <div style="height:14px"></div>
        <div style="color:var(--muted);font-size:14px">Buka setiap hari 09:00 — 21:00 • Pengiriman tersedia</div>
      </div>

      <div class="hero-illus">
        <!-- sample background; ganti src dengan foto toko/es krimmu -->
        <img src="https://i.pinimg.com/736x/ca/b9/30/cab930774d1c9e5effec3a7eb8d9f422.jpg" alt="Ilustrasi es krim">
      </div>
    </div>

    <!-- FLAVORS SECTION -->
    <main>
      <section class="section" id="flavors">
        <h3>Rasa Favorit — Banyak Coklat!</h3>
        <p class="meta">Kumpulan rasa spesial & coklat-forward — ada classic, molten, bomb, dan banyak lagi.</p>

        <div class="filters" aria-hidden="true">
          <div class="chip active" data-filter="all">Semua</div>
          <div class="chip" data-filter="milk">Milk Chocolate</div>
          <div class="chip" data-filter="dark">Dark Chocolate</div>
          <div class="chip" data-filter="brownie">Brownie & Cake</div>
          <div class="chip" data-filter="nutt">Nutties</div>
          <div class="chip" data-filter="special">Special / Fusion</div>
        </div>

        <div class="grid" id="grid">
          <!-- Banyak varian coklat: kamu bisa ganti src gambar nanti -->
          <!-- 1 -->
          <article class="card" data-type="milk">
            <div class="img"><img src="https://i.pinimg.com/736x/32/d3/f6/32d3f643d223441e6ffb7f4c4deb4e44.jpg" alt="Classic Milk Chocolate"></div>
            <div class="body">
              <h4>Classic Milk Chocolate</h4>
              <div class="meta">Krim susu + coklat lembut</div>
              <div class="price">Rp 28.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Classic Milk Chocolate')">Beli</button></div>
            </div>
          </article>

          <!-- 2 -->
          <article class="card" data-type="dark">
            <div class="img"><img src="https://i.pinimg.com/736x/e3/33/58/e33358769493e095567b5d2cbf23dd18.jpg" alt="Intense Dark Cocoa"></div>
            <div class="body">
              <h4>Intense Dark Cocoa</h4>
              <div class="meta">Dark chocolate 70% — untuk penikmat pahit manis</div>
              <div class="price">Rp 30.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Intense Dark Cocoa')">Beli</button></div>
            </div>
          </article>

          <!-- 3 -->
          <article class="card" data-type="brownie">
            <div class="img"><img src="https://i.pinimg.com/736x/5d/82/92/5d829273fceebe3c64ac00603da3b6ee.jpg" alt="Brownie Chunk"></div>
            <div class="body">
              <h4>Brownie Chunk</h4>
              <div class="meta">Potongan brownie + swirl coklat</div>
              <div class="price">Rp 33.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Brownie Chunk')">Beli</button></div>
            </div>
          </article>

          <!-- 4 -->
          <article class="card" data-type="milk">
            <div class="img"><img src="https://i.pinimg.com/736x/1a/37/c8/1a37c8bfa21f2db02ab1d0f165d4bf33.jpg" alt="Silky Caramel Chocolate"></div>
            <div class="body">
              <h4>Silky Caramel Chocolate</h4>
              <div class="meta">Caramel ribbon + milk chocolate</div>
              <div class="price">Rp 32.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Silky Caramel Chocolate')">Beli</button></div>
            </div>
          </article>

          <!-- 5 -->
          <article class="card" data-type="nutt">
            <div class="img"><img src="https://i.pinimg.com/736x/fd/be/41/fdbe416d8d71cefaef0a0bb168a7f136.jpg" alt="Hazelnut Choco Crunch"></div>
            <div class="body">
              <h4>Hazelnut Choco Crunch</h4>
              <div class="meta">Coklat + kacang hazelnut renyah</div>
              <div class="price">Rp 35.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Hazelnut Choco Crunch')">Beli</button></div>
            </div>
          </article>

          <!-- 6 -->
          <article class="card" data-type="special">
            <div class="img"><img src="https://i.pinimg.com/736x/68/d0/bc/68d0bc36d3c9c63f9018ba3900db13ee.jpg" alt="Choco Lava Bomb"></div>
            <div class="body">
              <h4>Choco Lava Bomb</h4>
              <div class="meta">Pusat molten chocolate — meleleh di mulut</div>
              <div class="price">Rp 40.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Choco Lava Bomb')">Beli</button></div>
            </div>
          </article>

          <!-- 7 -->
          <article class="card" data-type="dark">
            <div class="img"><img src="https://i.pinimg.com/1200x/fd/91/f8/fd91f8e12a722b1f9fd6432bd64bc8b9.jpg" alt="Espresso Dark Choco"></div>
            <div class="body">
              <h4>Espresso Dark Choco</h4>
              <div class="meta">Kopi + dark chocolate</div>
              <div class="price">Rp 31.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Espresso Dark Choco')">Beli</button></div>
            </div>
          </article>

          <!-- 8 -->
          <article class="card" data-type="brownie">
            <div class="img"><img src="https://i.pinimg.com/1200x/8c/24/d9/8c24d92ad4b58e8a1e10ce53d9b2051f.jpg" alt="Cake & Choco"></div>
            <div class="body">
              <h4>Cake & Choco Swirl</h4>
              <div class="meta">Cake crumb + chocolate swirl</div>
              <div class="price">Rp 34.000 / scoop</div>
              <div class="actions"><button class="btn-primary" onclick="addAlert('Cake & Choco Swirl')">Beli</button></div>
            </div>
          </article>

          <!-- Tambah lagi varian sesuai kebutuhan... -->
        </div>
      </section>

      <!-- MENU / INFO -->
      <section class="section" id="menu">
        <h3>Menu & Paket</h3>
        <p class="meta">Pilih satu scoop, dua scoop, atau paket keluarga. Tersedia topping dan saus coklat.</p>
        <div style="display:flex;gap:18px;flex-wrap:wrap;margin-top:12px">
          <div style="flex:1;min-width:220px;background:linear-gradient(180deg,#fff7f3,#fff3ee);padding:16px;border-radius:12px">
            <strong>Scoop</strong>
            <p class="meta" style="margin:8px 0 0">1 scoop — Rp 28.000</p>
            <p class="meta" style="margin:6px 0 0">2 scoop — Rp 52.000</p>
          </div>
          <div style="flex:1;min-width:220px;background:linear-gradient(180deg,#fff7f3,#fff3ee);padding:16px;border-radius:12px">
            <strong>Paket Keluarga</strong>
            <p class="meta" style="margin:8px 0 0">Box 8 scoop — Rp 220.000</p>
            <p class="meta" style="margin:6px 0 0">Box 12 scoop — Rp 320.000</p>
          </div>
          <div style="flex:1;min-width:220px;background:linear-gradient(180deg,#fff7f3,#fff3ee);padding:16px;border-radius:12px">
            <strong>Topping & Saus</strong>
            <p class="meta" style="margin:8px 0 0">Nuts, sprinkles, hot fudge</p>
          </div>
        </div>
      </section>

      <!-- CONTACT -->
      <section class="section" id="contact">
        <h3>Kontak & Pemesanan</h3>
        <p class="meta">Hubungi kami lewat email atau telepon untuk pesanan besar atau catering.</p>
        <div style="display:flex;gap:12px;align-items:center;flex-wrap:wrap;margin-top:12px">
          <a class="chip" href="mailto:order@chococream.id">✉️ order@chococream.id</a>
          <div class="chip">📞 +62 812 3456 7890</div>
          <div class="chip">🏬 Jl. Manis No.10, Kota</div>
        </div>
      </section>

    </main>

    <footer>
      © 2025 ChocoCream • Cinta untuk coklat & es krim
    </footer>
  </div>

  <script>
    // Filter chips
    document.querySelectorAll('.chip').forEach(chip => {
      chip.addEventListener('click', function(){
        const filter = this.dataset.filter;
        document.querySelectorAll('.chip').forEach(c => c.classList.remove('active'));
        this.classList.add('active');
        filterGrid(filter || 'all');
      });
    });

    function filterGrid(filter){
      const cards = document.querySelectorAll('.grid .card');
      cards.forEach(card => {
        if(filter === 'all' || !filter) {
          card.style.display = '';
        } else {
          card.style.display = card.dataset.type === filter ? '' : 'none';
        }
      });
    }

    // initial show all
    filterGrid('all');

    // Simple "add to cart" alert (placeholder)
    function addAlert(name){
      // simple toast-like feedback
      const t = document.createElement('div');
      t.textContent = name + ' ditambahkan ke pesanan!';
      t.style.position = 'fixed';
      t.style.right = '18px';
      t.style.bottom = '18px';
      t.style.background = 'linear-gradient(90deg,var(--accent),var(--accent-2))';
      t.style.color = 'white';
      t.style.padding = '12px 16px';
      t.style.borderRadius = '12px';
      t.style.boxShadow = '0 8px 20px rgba(0,0,0,0.12)';
      t.style.zIndex = 9999;
      document.body.appendChild(t);
      setTimeout(()=> t.style.opacity = '0.9', 10);
      setTimeout(()=> t.remove(), 2200);
    }
  </script>
</body>
</html>
