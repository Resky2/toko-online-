```html
<!DOCTYPE html>
<html lang="id">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Warung Sess Mas Resky — Kreco, Janggelan &amp; Rica-Rica Bekicot</title>
<meta name="description" content="Warung Sess Mas Resky. Pesan kreco, es janggelan, dan rica-rica bekicot langsung lewat WhatsApp.">
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Bevan&family=Work+Sans:wght@400;500;600;700&display=swap" rel="stylesheet">

<style>
  :root {
    --bg-deep: #243420;
    --bg-deep-2: #1b2818;
    --cream: #efe3c3;
    --cream-2: #f6eeda;
    --ink: #221a11;
    --chili: #b5402a;
    --chili-dark: #8f301e;
    --turmeric: #c68a2e;
    --shell: #8b7355;
    --line: rgba(34, 26, 17, 0.18);
  }

  * { box-sizing: border-box; }
  html { scroll-behavior: smooth; }

  body {
    margin: 0;
    background: var(--cream);
    color: var(--ink);
    font-family: 'Work Sans', sans-serif;
    line-height: 1.5;
  }

  h1, h2, h3, .display {
    font-family: 'Bevan', serif;
    font-weight: 400;
    line-height: 1.15;
    margin: 0;
  }

  img, svg { display: block; max-width: 100%; }
  a { color: inherit; }

  .wrap {
    max-width: 1080px;
    margin: 0 auto;
    padding: 0 24px;
  }

  .hero {
    background:
      radial-gradient(ellipse at 20% -10%, #33482c 0%, transparent 55%),
      radial-gradient(ellipse at 90% 110%, #1a2717 0%, transparent 50%),
      var(--bg-deep);
    padding: 20px 0 64px;
    position: relative;
    overflow: hidden;
  }

  .topbar {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 18px 0;
    color: var(--cream-2);
  }

  .topbar .mark {
    display: flex;
    align-items: center;
    gap: 10px;
    font-family: 'Bevan', serif;
    font-size: 1.05rem;
    letter-spacing: 0.02em;
  }

  .topbar .mark svg { width: 30px; height: 30px; }

  .topbar nav a {
    text-decoration: none;
    color: var(--cream-2);
    opacity: 0.85;
    margin-left: 22px;
    font-size: 0.92rem;
    transition: opacity 0.2s ease;
  }
  .topbar nav a:hover { opacity: 1; }

  .signboard {
    margin: 56px auto 0;
    max-width: 760px;
    text-align: center;
    color: var(--cream-2);
  }

  .signboard .eyebrow-leaf {
    display: flex;
    justify-content: center;
    gap: 14px;
    margin-bottom: 18px;
    color: var(--turmeric);
  }
  .signboard .eyebrow-leaf svg { width: 26px; height: 26px; }

  .signboard h1 {
    font-size: clamp(2.4rem, 6vw, 4.1rem);
    color: var(--cream-2);
  }

  .signboard h1 span {
    display: block;
    color: var(--turmeric);
    font-size: 0.42em;
    margin-top: 10px;
    letter-spacing: 0.03em;
  }

  .signboard p {
    max-width: 480px;
    margin: 22px auto 0;
    color: #d8d2bd;
    font-size: 1.02rem;
  }

  .hero-cta {
    display: flex;
    justify-content: center;
    gap: 14px;
    margin-top: 32px;
    flex-wrap: wrap;
  }

  .btn {
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 9px;
    padding: 13px 24px;
    border-radius: 8px;
    font-family: 'Work Sans', sans-serif;
    font-weight: 600;
    font-size: 0.98rem;
    text-decoration: none;
    border: 2px solid transparent;
    cursor: pointer;
    transition: transform 0.15s ease, box-shadow 0.15s ease, background-color 0.2s ease;
  }
  .btn:hover { transform: translateY(-2px); }

  .btn-primary {
    background: var(--chili);
    color: #fff8ee;
    box-shadow: 0 6px 0 var(--chili-dark);
  }
  .btn-primary:hover { box-shadow: 0 8px 0 var(--chili-dark); }
  .btn-primary:active { transform: translateY(1px); box-shadow: 0 3px 0 var(--chili-dark); }

  .btn-ghost {
    background: transparent;
    color: var(--cream-2);
    border-color: rgba(239,227,195,0.4);
  }
  .btn-ghost:hover { border-color: var(--cream-2); }

  .wave {
    display: block;
    width: 100%;
    height: 46px;
    margin-top: -2px;
  }

  .menu {
    padding: 60px 0 40px;
  }

  .menu-head {
    text-align: center;
    max-width: 580px;
    margin: 0 auto 36px;
  }

  .menu-head h2 {
    font-size: clamp(1.8rem, 4vw, 2.5rem);
    color: var(--ink);
  }

  .menu-head p {
    margin-top: 14px;
    color: #4c4230;
    font-size: 1rem;
  }

  /* Filter Tabs */
  .filter-bar {
    display: flex;
    justify-content: center;
    gap: 12px;
    margin-bottom: 40px;
    flex-wrap: wrap;
  }

  .filter-btn {
    background: var(--cream-2);
    border: 2px solid var(--ink);
    padding: 8px 18px;
    border-radius: 30px;
    font-family: 'Work Sans', sans-serif;
    font-weight: 600;
    font-size: 0.9rem;
    color: var(--ink);
    cursor: pointer;
    transition: all 0.2s ease;
    box-shadow: 2px 2px 0 rgba(34,26,17,0.15);
  }

  .filter-btn:hover, .filter-btn.active {
    background: var(--bg-deep);
    color: var(--cream-2);
    border-color: var(--bg-deep);
    box-shadow: 3px 3px 0 var(--turmeric);
  }

  .menu-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 28px;
  }

  @media (max-width: 900px) {
    .menu-grid { grid-template-columns: 1fr; max-width: 440px; margin: 0 auto; }
  }

  .plate {
    background: var(--cream-2);
    border: 2px solid var(--ink);
    border-radius: 16px;
    overflow: hidden;
    position: relative;
    display: flex;
    flex-direction: column;
    box-shadow: 6px 6px 0 rgba(34,26,17,0.14);
    transition: transform 0.25s ease, box-shadow 0.25s ease, opacity 0.3s ease;
  }

  .plate:hover {
    transform: translateY(-4px);
    box-shadow: 8px 10px 0 rgba(34,26,17,0.18);
  }

  .plate.hide {
    display: none !important;
  }

  .plate .torn {
    position: absolute;
    top: 14px;
    left: 14px;
    background: var(--turmeric);
    color: var(--ink);
    font-family: 'Bevan', serif;
    font-size: 0.72rem;
    padding: 5px 12px;
    border-radius: 4px;
    transform: rotate(-2deg);
    box-shadow: 0 3px 0 rgba(34,26,17,0.25);
    z-index: 2;
  }

  /* Image Container & Hover Zoom */
  .media-box {
    position: relative;
    width: 100%;
    aspect-ratio: 4 / 3;
    overflow: hidden;
    background: #1b2818;
    cursor: pointer;
  }

  .media-box img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    transition: transform 0.4s ease, filter 0.3s ease;
  }

  .media-box:hover img {
    transform: scale(1.08);
    filter: brightness(0.92);
  }

  .media-overlay {
    position: absolute;
    inset: 0;
    background: rgba(34,26,17,0.35);
    display: flex;
    align-items: center;
    justify-content: center;
    opacity: 0;
    transition: opacity 0.25s ease;
  }

  .media-box:hover .media-overlay {
    opacity: 1;
  }

  .zoom-icon {
    background: var(--cream);
    color: var(--ink);
    padding: 8px 14px;
    border-radius: 20px;
    font-size: 0.82rem;
    font-weight: 700;
    display: flex;
    align-items: center;
    gap: 6px;
    box-shadow: 0 4px 10px rgba(0,0,0,0.3);
  }

  .plate-body {
    padding: 22px 22px 20px;
    display: flex;
    flex-direction: column;
    flex-grow: 1;
  }

  .plate h3 {
    font-size: 1.35rem;
    color: var(--ink);
    margin-bottom: 8px;
  }

  .plate p.desc {
    margin: 0;
    color: #4c4230;
    font-size: 0.92rem;
    line-height: 1.5;
    flex-grow: 1;
    margin-bottom: 18px;
  }

  .plate .price-row {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: auto;
    padding-top: 14px;
    border-top: 1px dashed var(--line);
  }

  .price-tag {
    font-family: 'Bevan', serif;
    font-size: 1.3rem;
    color: var(--chili);
  }
  .price-tag small {
    font-family: 'Work Sans', sans-serif;
    font-weight: 500;
    font-size: 0.65rem;
    color: #6b5f47;
    display: block;
    margin-top: 1px;
  }

  .order-btn {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    background: var(--chili);
    color: #fff8ee;
    border: none;
    padding: 10px 16px;
    border-radius: 8px;
    font-weight: 600;
    font-size: 0.88rem;
    box-shadow: 0 4px 0 var(--chili-dark);
    cursor: pointer;
    transition: transform 0.15s ease, box-shadow 0.15s ease;
  }
  .order-btn:hover { transform: translateY(-2px); box-shadow: 0 6px 0 var(--chili-dark); }
  .order-btn:active { transform: translateY(1px); box-shadow: 0 2px 0 var(--chili-dark); }
  .order-btn svg { width: 17px; height: 17px; }

  .strip {
    margin-top: 64px;
    background: var(--bg-deep-2);
    color: var(--cream-2);
    padding: 48px 0;
  }
  .strip .wrap {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 28px;
    flex-wrap: wrap;
  }
  .strip h3 {
    font-size: 1.4rem;
    max-width: 440px;
  }
  .strip p {
    color: #cfc8b1;
    max-width: 380px;
    margin: 10px 0 0;
    font-size: 0.92rem;
  }

  footer {
    padding: 40px 0 30px;
    text-align: center;
    color: #6b5f47;
    font-size: 0.85rem;
  }
  footer .fwa {
    color: var(--chili);
    font-weight: 600;
    text-decoration: none;
  }

  .float-wa {
    position: fixed;
    right: 22px;
    bottom: 22px;
    background: #25D366;
    color: #ffffff;
    width: 58px;
    height: 58px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    box-shadow: 0 8px 20px rgba(0,0,0,0.3);
    text-decoration: none;
    z-index: 90;
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }
  .float-wa:hover {
    transform: scale(1.08);
    box-shadow: 0 10px 24px rgba(0,0,0,0.35);
  }
  .float-wa svg { width: 30px; height: 30px; }

  .modal-backdrop {
    position: fixed;
    inset: 0;
    background: rgba(18, 26, 16, 0.82);
    backdrop-filter: blur(4px);
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 20px;
    z-index: 100;
    opacity: 0;
    pointer-events: none;
    transition: opacity 0.25s ease;
  }

  .modal-backdrop.active {
    opacity: 1;
    pointer-events: auto;
  }

  .modal-card {
    background: var(--cream-2);
    border: 2px solid var(--ink);
    border-radius: 16px;
    max-width: 520px;
    width: 100%;
    overflow: hidden;
    box-shadow: 0 16px 32px rgba(0,0,0,0.3);
    position: relative;
    transform: translateY(20px);
    transition: transform 0.25s ease;
  }

  .modal-backdrop.active .modal-card {
    transform: translateY(0);
  }

  .modal-close {
    position: absolute;
    top: 14px;
    right: 14px;
    width: 32px;
    height: 32px;
    background: rgba(34,26,17,0.75);
    color: var(--cream-2);
    border: none;
    border-radius: 50%;
    font-size: 1.2rem;
    line-height: 1;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
    z-index: 5;
    transition: background 0.2s;
  }
  .modal-close:hover { background: var(--chili); }

  /* Lightbox specific */
  .lightbox-card {
    max-width: 720px;
    background: var(--bg-deep-2);
    color: var(--cream-2);
    border: 2px solid var(--turmeric);
  }

  .lightbox-img-wrap {
    max-height: 420px;
    background: #000;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }

  .lightbox-img-wrap img {
    width: 100%;
    max-height: 420px;
    object-fit: contain;
  }

  .lightbox-info {
    padding: 20px 24px 24px;
  }

  .lightbox-info h3 {
    font-size: 1.5rem;
    color: var(--turmeric);
    margin-bottom: 6px;
  }

  .lightbox-info p {
    color: #cfc8b1;
    margin-bottom: 16px;
    font-size: 0.95rem;
  }

  /* Order Modal Specific */
  .order-modal-head {
    display: flex;
    gap: 16px;
    padding: 20px;
    background: var(--cream);
    border-bottom: 1px dashed var(--line);
  }

  .order-modal-thumb {
    width: 80px;
    height: 80px;
    border-radius: 8px;
    object-fit: cover;
    border: 1px solid var(--ink);
  }

  .order-modal-title h3 {
    font-size: 1.25rem;
    color: var(--ink);
  }

  .order-modal-title .modal-price {
    font-family: 'Bevan', serif;
    color: var(--chili);
    font-size: 1.1rem;
    margin-top: 4px;
  }

  .order-modal-body {
    padding: 20px;
  }

  .form-group {
    margin-bottom: 18px;
  }

  .form-group label {
    display: block;
    font-weight: 600;
    font-size: 0.9rem;
    margin-bottom: 8px;
    color: var(--ink);
  }

  .qty-picker {
    display: flex;
    align-items: center;
    gap: 12px;
  }

  .qty-btn {
    width: 38px;
    height: 38px;
    background: var(--cream);
    border: 2px solid var(--ink);
    border-radius: 8px;
    font-size: 1.2rem;
    font-weight: bold;
    cursor: pointer;
    display: flex;
    align-items: center;
    justify-content: center;
  }
  .qty-btn:hover { background: var(--turmeric); color: #fff; }

  .qty-input {
    width: 50px;
    text-align: center;
    font-family: 'Bevan', serif;
    font-size: 1.1rem;
    border: none;
    background: transparent;
  }

  .note-textarea {
    width: 100%;
    padding: 10px 12px;
    border: 2px solid var(--ink);
    border-radius: 8px;
    background: var(--cream-2);
    font-family: inherit;
    font-size: 0.9rem;
    resize: vertical;
    min-height: 70px;
  }
  .note-textarea:focus {
    outline: none;
    border-color: var(--chili);
  }

  .order-modal-foot {
    padding: 16px 20px 20px;
    background: var(--cream);
    border-top: 1px dashed var(--line);
    display: flex;
    align-items: center;
    justify-content: space-between;
  }

  .total-price-val {
    font-family: 'Bevan', serif;
    font-size: 1.35rem;
    color: var(--chili);
  }
</style>
</head>
<body>

<header class="hero">
  <div class="wrap">
    <div class="topbar">
      <div class="mark">
        <svg viewBox="0 0 40 40" fill="none" xmlns="http://www.w3.org/2000/svg">
          <path d="M20 4C11 4 4 11 4 20c0 9 7 16 16 16 9 0 16-7 16-16C36 11 29 4 20 4z" fill="#c68a2e"/>
          <path d="M13 22c0-5 3-9 7-9s7 4 7 9-3 7-7 7-7-2-7-7z" fill="#efe3c3"/>
          <circle cx="17" cy="20" r="1.6" fill="#221a11"/>
        </svg>
        Warung Sess Mas Resky
      </div>
      <nav>
        <a href="#menu">Menu Utama</a>
        <a href="#cara-pesan">Cara Pesan</a>
      </nav>
    </div>

    <div class="signboard">
      <div class="eyebrow-leaf">
        <svg viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C7 2 3 6 3 11c0 6 5 9 9 11 4-2 9-5 9-11 0-5-4-9-9-9zm0 4c2.8 0 5 2.2 5 5 0 3.5-2.6 5.7-5 7-2.4-1.3-5-3.5-5-7 0-2.8 2.2-5 5-5z"/></svg>
      </div>
      <h1>Kreco, Janggelan &amp; Rica-Rica Bekicot<span>Racikan rumahan, pedas dan segarnya pas</span></h1>
      <p>Camilan kreco gurih, es janggelan yang bikin adem, sampai rica-rica bekicot pedas nampol — diolah khas Warung Sess Mas Resky. Klik fotonya untuk perbesar atau pesan langsung via WhatsApp!</p>
      <div class="hero-cta">
        <a class="btn btn-primary" href="#menu">
          <svg viewBox="0 0 24 24" width="18" height="18" fill="currentColor"><path d="M7 4h-2l-1 2v2h1l3 10a2 2 0 0 0 2 1h8a2 2 0 0 0 2-1l3-9H6.4M9 20a1 1 0 1 0 0 2 1 1 0 0 0 0-2zm8 0a1 1 0 1 0 0 2 1 1 0 0 0 0-2z"/></svg>
          Lihat Menu &amp; Foto
        </a>
        <a class="btn btn-ghost" href="#cara-pesan">Cara Pesan</a>
      </div>
    </div>
  </div>

  <svg class="wave" viewBox="0 0 1200 46" preserveAspectRatio="none" xmlns="http://www.w3.org/2000/svg">
    <path d="M0 20 Q 50 46 100 20 T 200 20 T 300 20 T 400 20 T 500 20 T 600 20 T 700 20 T 800 20 T 900 20 T 1000 20 T 1100 20 T 1200 20 V46 H0 Z" fill="#efe3c3"/>
  </svg>
</header>

<main>
  <section class="menu" id="menu">
    <div class="wrap">
      <div class="menu-head">
        <h2>Menu Warung</h2>
        <p>Tiga andalan Warung Sess Mas Resky. Klik foto untuk pratinjau detail atau tekan "Pesan" untuk mengatur jumlah porsi.</p>
      </div>

      <!-- Filter Buttons -->
      <div class="filter-bar">
        <button class="filter-btn active" data-filter="all">Semua Menu</button>
        <button class="filter-btn" data-filter="makanan">Makanan &amp; Camilan</button>
        <button class="filter-btn" data-filter="minuman">Minuman Segar</button>
      </div>

      <div class="menu-grid">

        <!-- KRECO -->
        <article class="plate" data-category="makanan">
          <span class="torn">Camilan Favorit</span>
          <div class="media-box" onclick="openLightbox('Kreco Gurih Sawah', 'https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=1000&q=80', 'Keripik & keong sawah gurih renyah dengan bumbu khas warung. Cocok untuk teman ngobrol sore.', '10.000')">
            <img src="https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=800&q=80" 
                 alt="Kreco Olahan Keong Sawah Gurih"
                 onerror="this.src='https://placehold.co/800x600/243420/efe3c3?text=Kreco+Gurih'">
            <div class="media-overlay">
              <span class="zoom-icon">
                <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>
                Perbesar Foto
              </span>
            </div>
          </div>
          <div class="plate-body">
            <h3>Kreco</h3>
            <p class="desc">Olahan keong sawah gurih renyah, dimasak dengan bumbu rempah khas warung yang meresap sempurna. Cocok jadi teman ngobrol sore.</p>
            <div class="price-row">
              <span class="price-tag">Rp10.000<small>per porsi</small></span>
              <button class="order-btn" onclick="openOrderModal('Kreco', 10000, 'https://images.unsplash.com/photo-1541544741938-0af808871cc0?auto=format&fit=crop&w=300&q=80')">
                <svg viewBox="0 0 24 24" fill="currentColor"><path d="M20.5 3.5A11 11 0 0 0 3.6 17.3L2 22l4.8-1.6A11 11 0 1 0 20.5 3.5zm-8.4 17a9 9 0 0 1-4.6-1.3l-.3-.2-3 1 1-2.9-.2-.3A9 9 0 1 1 12.1 20.5zm5-6.7c-.3-.1-1.6-.8-1.8-.9-.2-.1-.4-.1-.6.1-.2.3-.7.9-.8 1-.2.2-.3.2-.5.1-.3-.1-1.2-.4-2.2-1.4-.8-.7-1.4-1.6-1.6-1.9-.2-.3 0-.4.1-.6l.4-.5c.1-.2.2-.3.3-.5.1-.2 0-.4 0-.5 0-.1-.6-1.5-.8-2-.2-.5-.4-.4-.6-.4h-.5c-.2 0-.5.1-.7.3-.2.3-1 1-1 2.3 0 1.4 1 2.7 1.1 2.9.1.2 2 3.1 4.9 4.3.7.3 1.2.5 1.6.6.7.2 1.3.2 1.8.1.5-.1 1.6-.7 1.9-1.3.2-.6.2-1.1.2-1.3-.1-.1-.3-.2-.6-.3z"/></svg>
                Pesan
              </button>
            </div>
          </div>
        </article>

        <!-- JANGGELAN -->
        <article class="plate" data-category="minuman">
          <span class="torn">Penyegar Dahaga</span>
          <div class="media-box" onclick="openLightbox('Es Janggelan Segar', 'https://images.unsplash.com/photo-1556881286-fc6915169721?auto=format&fit=crop&w=1000&q=80', 'Es cincau hitam asli disiram sirup gula aren leleh dan santan gurih segar.', '5.000')">
            <img src="https://images.unsplash.com/photo-1556881286-fc6915169721?auto=format&fit=crop&w=800&q=80" 
                 alt="Es Janggelan Cincau Hitam Gula Aren"
                 onerror="this.src='https://placehold.co/800x600/243420/efe3c3?text=Es+Janggelan'">
            <div class="media-overlay">
              <span class="zoom-icon">
                <svg width="16" height="16" fill="currentColor" viewBox="0 0 24 24"><path d="M15.5 14h-.79l-.28-.27C15.41 12.59 16 11.11 16 9.5 16 5.91 13.09 3 9.5 3S3 5.91 3 9.5 5.91 16 9.5 16c1.61 0 3.09-.59 4.23-1.57l.27.28v.79l5 4.99L20.49 19l-4.99-5zm-6 0C7.01 14 5 11.99 5 9.5S7.01 5 9.5 5 14 7.01 14 9.5 11.99 14 9.5 14z"/></svg>
                Perbesar Foto
              </span>
            </div>
          </div>
          <div class="plate-body">
            <h3>Janggelan</h3>
            <p class="desc">Es cincau hitam alami, disiram lelehan gula aren cair dan santan gurih segar. Manisnya pas, adem dan nyelekit segar di tenggorokan.</p>
            <div class="price-row">
              <span class="price-tag">Rp5.000<small>per gelas</small></span>
        
