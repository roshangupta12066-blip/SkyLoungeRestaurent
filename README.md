<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Sky Lounge | Ghazipur</title>
  <meta name="description" content="Sky Lounge, Ghazipur - Fine dining across 5 floors with tandoori, Chinese starters, main course, desserts and beverages." />
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cinzel:wght@500;700;800&family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">

  <style>
    :root{
      --bg:#120d08;
      --bg2:#1b140d;
      --card:#20170f;
      --text:#f7efe1;
      --muted:#cdbb9a;
      --gold:#d7a84a;
      --gold-soft:#e9c97e;
      --accent:#7a4c16;
      --line:rgba(233,201,126,.25);
      --shadow:0 20px 40px rgba(0,0,0,.35);
    }
    *{box-sizing:border-box}
    html,body{margin:0;padding:0;background:radial-gradient(circle at 10% 10%, #2b1d10 0%, var(--bg) 45%, #0b0805 100%);color:var(--text);font-family:'Poppins',system-ui,-apple-system,sans-serif;scroll-behavior:smooth}
    a{color:inherit;text-decoration:none}
    .container{width:min(1150px,92%);margin-inline:auto}
    .fancy{font-family:'Cinzel',serif;letter-spacing:.6px}
    .btn{
      display:inline-block;padding:12px 20px;border-radius:999px;font-weight:600;
      border:1px solid var(--line);transition:.25s ease;cursor:pointer
    }
    .btn-primary{background:linear-gradient(135deg,var(--gold),#b9822f);color:#1a120a;box-shadow:0 10px 25px rgba(215,168,74,.35)}
    .btn-primary:hover{transform:translateY(-2px);filter:brightness(1.03)}
    .btn-outline{background:transparent;color:var(--gold-soft)}
    .btn-outline:hover{background:rgba(233,201,126,.1)}
    header{
      position:sticky;top:0;z-index:50;background:rgba(18,13,8,.7);backdrop-filter: blur(10px);
      border-bottom:1px solid var(--line)
    }
    .nav{display:flex;align-items:center;justify-content:space-between;padding:12px 0;gap:10px}
    .logo{display:flex;align-items:center;gap:10px}
    .logo-badge{
      width:42px;height:42px;border-radius:12px;background:linear-gradient(145deg,#f0d48f,#a77423);
      color:#1f150a;display:grid;place-items:center;font-weight:800;font-family:'Cinzel',serif
    }
    .logo h1{font-size:1.1rem;margin:0;line-height:1}
    .logo small{color:var(--muted)}
    .nav-links{display:flex;gap:16px;flex-wrap:wrap}
    .nav-links a{font-size:.95rem;color:var(--muted)}
    .nav-links a:hover{color:var(--gold-soft)}

    .hero{
      padding:72px 0 42px;
      background:
      linear-gradient(rgba(10,7,4,.5),rgba(10,7,4,.8)),
      url('https://images.unsplash.com/photo-1517248135467-4c7edcad34c4?q=80&w=1600&auto=format&fit=crop') center/cover no-repeat;
      border-bottom:1px solid var(--line)
    }
    .hero-grid{display:grid;grid-template-columns:1.2fr .8fr;gap:26px;align-items:end}
    .tag{display:inline-flex;padding:7px 14px;border:1px solid var(--line);border-radius:999px;color:var(--gold-soft);font-size:.84rem;background:rgba(25,18,11,.6)}
    .hero h2{font-size:clamp(2rem,4.5vw,3.5rem);margin:.7rem 0 .8rem}
    .hero p{color:var(--muted);max-width:650px}
    .hero-card{
      background:linear-gradient(180deg,rgba(34,25,16,.9),rgba(16,12,8,.95));border:1px solid var(--line);border-radius:18px;padding:18px;box-shadow:var(--shadow)
    }
    .hero-card ul{list-style:none;padding:0;margin:0;display:grid;gap:10px}
    .hero-card li{display:flex;justify-content:space-between;gap:12px;font-size:.95rem}
    .hero-card li span:first-child{color:var(--muted)}
    .hero-actions{display:flex;gap:12px;flex-wrap:wrap;margin-top:18px}

    section{padding:56px 0}
    .sec-head{display:flex;justify-content:space-between;align-items:end;gap:10px;margin-bottom:20px}
    .sec-head h3{margin:0;font-size:clamp(1.5rem,3vw,2.2rem)}
    .sec-head p{margin:0;color:var(--muted)}
    .menu-tabs{display:flex;flex-wrap:wrap;gap:10px;margin-bottom:16px}
    .tab{
      padding:9px 14px;border:1px solid var(--line);border-radius:999px;color:var(--muted);cursor:pointer;user-select:none
    }
    .tab.active{background:linear-gradient(135deg,var(--gold),#b98336);color:#1f1509;border-color:transparent;font-weight:600}
    .menu-grid{
      display:grid;grid-template-columns:repeat(2,minmax(0,1fr));gap:14px
    }
    .item{
      background:linear-gradient(180deg,rgba(34,24,15,.75),rgba(24,17,10,.9));border:1px solid var(--line);
      border-radius:14px;padding:14px 16px;display:flex;justify-content:space-between;gap:15px;align-items:flex-start
    }
    .item .name{font-weight:500}
    .price{color:var(--gold-soft);font-weight:700;white-space:nowrap}

    .about-grid,.contact-grid,.review-grid,.gallery{
      display:grid;gap:16px
    }
    .about-grid{grid-template-columns:1.1fr .9fr}
    .panel{
      background:linear-gradient(180deg,rgba(34,24,15,.75),rgba(24,17,10,.9));
      border:1px solid var(--line);border-radius:16px;padding:20px;box-shadow:var(--shadow)
    }
    .stats{display:grid;grid-template-columns:repeat(3,1fr);gap:10px}
    .stat{padding:14px;border:1px solid var(--line);border-radius:12px;text-align:center}
    .stat strong{display:block;font-size:1.2rem;color:var(--gold-soft)}
    .gallery{grid-template-columns:repeat(4,1fr)}
    .gallery img{width:100%;height:170px;object-fit:cover;border-radius:14px;border:1px solid var(--line)}
    .review-grid{grid-template-columns:repeat(3,1fr)}
    .review{padding:18px}
    .stars{color:#ffd77a;letter-spacing:2px}
    .contact-grid{grid-template-columns:1fr 1fr}
    .map{
      border:0;width:100%;height:320px;border-radius:14px;filter:sepia(22%) saturate(90%) hue-rotate(-10deg)
    }
    footer{padding:24px 0;border-top:1px solid var(--line);color:var(--muted);text-align:center}
    @media (max-width:960px){
      .hero-grid,.about-grid,.contact-grid{grid-template-columns:1fr}
      .menu-grid{grid-template-columns:1fr}
      .review-grid{grid-template-columns:1fr}
      .gallery{grid-template-columns:repeat(2,1fr)}
    }
    @media (max-width:580px){
      .nav-links{display:none}
      .gallery{grid-template-columns:1fr}
      .hero{padding-top:58px}
    }
  </style>
</head>
<body>
  <header>
    <div class="container nav">
      <div class="logo">
        <div class="logo-badge">SL</div>
        <div>
          <h1 class="fancy">Sky Lounge</h1>
          <small>Ghazipur</small>
        </div>
      </div>
      <nav class="nav-links">
        <a href="#menu">Menu</a>
        <a href="#about">About</a>
        <a href="#gallery">Gallery</a>
        <a href="#reviews">Reviews</a>
        <a href="#contact">Contact</a>
      </nav>
    </div>
  </header>

  <section class="hero">
    <div class="container hero-grid">
      <div>
        <span class="tag fancy">Taste Above the City</span>
        <h2 class="fancy">Sky Lounge</h2>
        <p>Premium family dining experience with elegant ambience across <strong>5 floors</strong>. Enjoy flavorful tandoori delights, Chinese favorites, rich main course, desserts and beverages — all crafted fresh.</p>
        <div class="hero-actions">
          <a href="tel:9284069518" class="btn btn-primary">Call / WhatsApp</a>
          <a href="#menu" class="btn btn-outline">Explore Menu</a>
        </div>
      </div>
      <div class="hero-card">
        <ul>
          <li><span>City</span><strong>Ghazipur</strong></li>
          <li><span>Open Timing</span><strong>11:00 - 23:00 (All Week)</strong></li>
          <li><span>Floors</span><strong>5 Floors</strong></li>
          <li><span>Phone</span><strong>9284069518</strong></li>
        </ul>
      </div>
    </div>
  </section>

  <section id="menu">
    <div class="container">
      <div class="sec-head">
        <h3 class="fancy">Our Menu</h3>
        <p>Fresh taste, premium quality</p>
      </div>
      <div class="menu-tabs" id="tabs"></div>
      <div class="menu-grid" id="menuGrid"></div>
    </div>
  </section>

  <section id="about">
    <div class="container about-grid">
      <div class="panel">
        <div class="sec-head" style="margin-bottom:12px">
          <h3 class="fancy">Why Sky Lounge?</h3>
        </div>
        <p style="color:var(--muted);margin-top:0">Sky Lounge is designed for cozy family dinners, friends meetups and memorable celebrations. Warm interiors, rooftop vibe, and carefully prepared food make every visit special.</p>
        <div class="stats">
          <div class="stat"><strong>5</strong><span>Floors</span></div>
          <div class="stat"><strong>40+</strong><span>Menu Items</span></div>
          <div class="stat"><strong>4.9/5</strong><span>Guest Love</span></div>
        </div>
      </div>
      <div class="panel">
        <h3 class="fancy" style="margin-top:0">Quick Info</h3>
        <p style="margin:0;color:var(--muted)"><strong style="color:var(--gold-soft)">Address:</strong><br>Plat no. 9, Dariyapur Road, Above Dulhan Marriage Point, Khairabad, Sultanpur, Uttar Pradesh 228001.</p>
        <p style="margin:.8rem 0 0;color:var(--muted)"><strong style="color:var(--gold-soft)">Timing:</strong> 11:00 - 23:00 (All Week)</p>
        <p style="margin:.4rem 0 0;color:var(--muted)"><strong style="color:var(--gold-soft)">Phone / WhatsApp:</strong> 9284069518</p>
      </div>
    </div>
  </section>

  <section id="gallery">
    <div class="container">
      <div class="sec-head">
        <h3 class="fancy">Gallery</h3>
        <p>Premium vibes, delicious moments</p>
      </div>
      <div class="gallery">
        <img src="https://images.unsplash.com/photo-1559339352-11d035aa65de?q=80&w=1200&auto=format&fit=crop" alt="Restaurant interior" />
        <img src="https://images.unsplash.com/photo-1528605248644-14dd04022da1?q=80&w=1200&auto=format&fit=crop" alt="Dining table setup" />
        <img src="https://images.unsplash.com/photo-1552566626-52f8b828add9?q=80&w=1200&auto=format&fit=crop" alt="Fine dining ambience" />
        <img src="https://images.unsplash.com/photo-1515003197210-e0cd71810b5f?q=80&w=1200&auto=format&fit=crop" alt="Food platter" />
      </div>
    </div>
  </section>

  <section id="reviews">
    <div class="container">
      <div class="sec-head">
        <h3 class="fancy">Guest Reviews</h3>
        <p>What people are saying</p>
      </div>
      <div class="review-grid">
        <div class="panel review">
          <div class="stars">★★★★★</div>
          <p>Best Restaurent in Town, great service, every thin is perfect taste, interior, seeting area, open space everything</p>
          <strong style="color:var(--gold-soft)">Nitin Pandey</strong>
          <div style="color:var(--muted);font-size:.9rem">Food:5 | Service:5 | Atmosphere:5</div>
        </div>
        <div class="panel review">
          <div class="stars">★★★★★</div>
          <p>Delicious Delicious just waiting for you to arrive. Don't miss it!</p>
          <strong style="color:var(--gold-soft)">Naman Singh</strong>
          <div style="color:var(--muted);font-size:.9rem">Food:5 | Service:5 | Atmosphere:5</div>
        </div>
        <div class="panel review">
          <div class="stars">★★★★★</div>
          <p>After a long time enjoyed fully relished food. Food was very tasy, staff and service is excellent.</p>
          <strong style="color:var(--gold-soft)">Suryansh Mishra</strong>
          <div style="color:var(--muted);font-size:.9rem">Food:5 | Service:5 | Atmosphere:5</div>
        </div>
      </div>
    </div>
  </section>

  <section id="contact">
    <div class="container contact-grid">
      <div class="panel">
        <h3 class="fancy" style="margin-top:0">Contact & Location</h3>
        <p style="color:var(--muted)"><strong style="color:var(--gold-soft)">Address:</strong><br>Plat no. 9, Dariyapur Road, Above Dulhan Marriage Point, Khairabad, Sultanpur, Uttar Pradesh 228001.</p>
        <p style="color:var(--muted)"><strong style="color:var(--gold-soft)">Phone / WhatsApp:</strong> <a href="tel:9284069518">9284069518</a></p>
        <p style="color:var(--muted)"><strong style="color:var(--gold-soft)">Timing:</strong> 11:00 - 23:00, All Week</p>
        <div class="hero-actions">
          <a class="btn btn-primary" href="https://wa.me/919284069518" target="_blank">WhatsApp Now</a>
          <a class="btn btn-outline" target="_blank" href="https://www.google.com/maps?q=26.249807,82.069075">Open in Maps</a>
        </div>
      </div>
      <div class="panel">
        <iframe class="map" loading="lazy" src="https://maps.google.com/maps?q=26.249807,82.069075&z=15&output=embed"></iframe>
      </div>
    </div>
  </section>

  <footer>
    <div class="container">© <span id="year"></span> Sky Lounge, Ghazipur • Crafted with taste & elegance</div>
  </footer>

  <script>
    const menuData = {
      "Tandoori Veg Starters": [
        ["Dahi ke Kabab", 189],
        ["Veg Hara Bhara Kabab", 179],
        ["Veg Galawati Kabab", 189],
        ["Veg Seek Kabab", 189],
        ["Paneer Galawati Kabab", 229],
        ["Paneer Lasooni Tikka", 269],
        ["Paneer Hariyali Tikka", 269],
        ["Paneer Ka Sula", 259],
        ["Paneer Malai Tikka", 289],
        ["Paneer Achari Tikka", 269]
      ],
      "Chinese Veg Starters": [
        ["Paneer Manchurian [Dry]", 269],
        ["Chilli Paneer [Dry]", 269],
        ["Mushroom Chilli [Dry]", 189],
        ["Honey Chilli Potato", 179],
        ["Chilli Potato", 169],
        ["Veg Salt And Pepper", 179],
        ["Paneer Salt And Pepper", 269],
        ["Mushroom Salt And Pepper", 269],
        ["American Corn Salt And Pepper", 269]
      ],
      "Main Course": [
        ["Chilli Paneer [Gravy]", 289],
        ["Paneer Manchurian [Gravy]", 289],
        ["Mushroom Chilli [Gravy]", 229],
        ["Baby Corn Chilli [Gravy]", 229],
        ["Veg Chowmein", 149],
        ["Veg Manchurian [Dry]", 189],
        ["Veg Manchurian [Gravy]", 229],
        ["Matar Paneer", 249],
        ["Paneer Tikka Masala", 289],
        ["Paneer Lababdar", 289]
      ],
      "Dessert": [
        ["Gulab Jamun", 30],
        ["Rasmalai", 49],
        ["Vanilla Ice Cream", 60],
        ["Strawberry Ice Cream", 60],
        ["Chocolate Ice Cream", 80],
        ["Butterscotch Ice Cream", 80]
      ],
      "Drinks (Beverages)": [
        ["Coffee", 49],
        ["Masala Chai", 39],
        ["Chai", 29]
      ]
    };

    const tabs = document.getElementById("tabs");
    const menuGrid = document.getElementById("menuGrid");

    function renderTabs() {
      Object.keys(menuData).forEach((cat, idx) => {
        const b = document.createElement("button");
        b.className = "tab" + (idx === 0 ? " active" : "");
        b.textContent = cat;
        b.onclick = () => {
          document.querySelectorAll(".tab").forEach(t => t.classList.remove("active"));
          b.classList.add("active");
          renderItems(cat);
        };
        tabs.appendChild(b);
      });
    }

    function renderItems(cat) {
      menuGrid.innerHTML = "";
      menuData[cat].forEach(([name, price]) => {
        const el = document.createElement("article");
        el.className = "item";
        el.innerHTML = `<div class="name">${name}</div><div class="price">₹${price}</div>`;
        menuGrid.appendChild(el);
      });
    }

    renderTabs();
    renderItems(Object.keys(menuData)[0]);
    document.getElementById("year").textContent = new Date().getFullYear();
  </script>
</body>
</html>
