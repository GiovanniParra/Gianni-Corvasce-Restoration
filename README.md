<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<meta name="description" content="Furniture repair and restoration in Berkeley, CA — three generations of Italian craftsmanship. Real 4.9-star reviews, request a quote online.">
<title>Gianni Corvasce Restoration</title>
<link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Fraunces:ital,opsz,wght@0,9..144,340;0,9..144,440;0,9..144,560;0,9..144,650;1,9..144,500&family=Archivo:wght@400;500;600;700&display=swap">
<style>
  /* ============ TOKENS ============ */
  /* Deliberately single-theme (light) — a restoration studio's site is a
     business/trust document, not a mode-switching app, and a dark mode here
     previously rendered as a muddy brown page. Bright, clean, low-brown. */
  :root{
    --cream:      #FCFCF9;
    --cream-deep: #F0F5EE;
    --paper:      #FFFFFF;
    --ink:        #20241E;
    --ink-soft:   rgba(32,36,30,0.64);
    --ink-faint:  rgba(32,36,30,0.42);
    --forest:     #1E7A4C;
    --forest-deep:#155C39;
    --forest-tint: rgba(30,122,76,0.09);
    --walnut:     #A9835A;
    --walnut-tint: rgba(169,131,90,0.08);
    --brass:      #C69A2E;
    --brass-soft: rgba(198,154,46,0.32);
    --line:       rgba(32,36,30,0.10);
    --shadow:     0 18px 40px -20px rgba(32,36,30,0.22);
    --shadow-sm:  0 6px 18px -10px rgba(32,36,30,0.20);
    --radius:     7px;
    --radius-lg:  10px;
    --maxw: 1160px;
  }

  *{box-sizing:border-box}
  html{scroll-behavior:smooth}
  @media (prefers-reduced-motion: reduce){ html{scroll-behavior:auto} *{animation-duration:0.01ms !important; transition-duration:0.01ms !important;} }

  body{
    margin:0;
    background:var(--cream);
    color:var(--ink);
    font-family:'Archivo', system-ui, -apple-system, sans-serif;
    font-size:16px;
    line-height:1.6;
    -webkit-font-smoothing:antialiased;
  }
  h1,h2,h3{
    font-family:'Fraunces', Georgia, 'Times New Roman', serif;
    color:var(--ink);
    margin:0 0 0.5em;
    text-wrap:balance;
    font-weight:560;
    letter-spacing:-0.01em;
  }
  p{margin:0 0 1em; max-width:62ch}
  a{color:inherit}
  img{max-width:100%;display:block}
  .wrap{max-width:var(--maxw); margin:0 auto; padding:0 clamp(1.25rem,4vw,2.5rem)}
  .eyebrow{
    font-family:'Archivo',sans-serif; font-weight:600; font-size:0.72rem;
    letter-spacing:0.16em; text-transform:uppercase; color:var(--walnut);
    display:flex; align-items:center; gap:0.6em; margin-bottom:1em;
  }
  .eyebrow::before{content:"";width:22px;height:1px;background:var(--brass)}
  section{padding:clamp(3.5rem,7vw,6.5rem) 0}
  .section-head{max-width:640px; margin-bottom:clamp(2rem,4vw,3rem)}
  .section-head h2{font-size:clamp(1.7rem,3vw,2.4rem)}
  .section-head p{color:var(--ink-soft); font-size:1.05rem}

  /* reveal */
  .reveal{opacity:0; transform:translateY(18px); transition:opacity .6s ease, transform .6s ease}
  .reveal.in-view{opacity:1; transform:none}

  /* buttons */
  .btn{
    display:inline-flex; align-items:center; gap:0.55em;
    padding:0.85rem 1.65rem; border-radius:var(--radius);
    font-family:'Archivo',sans-serif; font-weight:600; font-size:0.95rem;
    text-decoration:none; border:1px solid transparent; cursor:pointer;
    transition:transform .18s ease, box-shadow .18s ease, background .18s ease, opacity .18s ease;
    white-space:nowrap;
  }
  .btn-primary{background:var(--forest); color:var(--cream)}
  .btn-primary:hover{background:var(--forest-deep); transform:translateY(-2px); box-shadow:var(--shadow-sm)}
  .btn-ghost{background:transparent; color:var(--ink); border-color:var(--line)}
  .btn-ghost:hover{border-color:var(--walnut); color:var(--walnut)}
  .btn-sm{padding:0.6rem 1.1rem; font-size:0.85rem}

  /* ============ NAV ============ */
  .site-nav{
    position:sticky; top:0; z-index:80;
    background:color-mix(in srgb, var(--cream) 92%, transparent);
    backdrop-filter:blur(10px);
    border-bottom:1px solid var(--line);
  }
  .site-nav .wrap{display:flex; align-items:center; justify-content:space-between; gap:1.5rem; padding-top:0.9rem; padding-bottom:0.9rem}
  .brand{font-family:'Fraunces',serif; font-weight:560; font-size:1.18rem; text-decoration:none; color:var(--ink); letter-spacing:-0.01em}
  .brand em{font-style:italic; color:var(--walnut)}
  .nav-links{display:flex; gap:2rem; list-style:none; margin:0; padding:0}
  .nav-links a{font-size:0.92rem; text-decoration:none; color:var(--ink-soft); transition:color .15s}
  .nav-links a:hover{color:var(--forest)}
  .nav-right{display:flex; align-items:center; gap:1.3rem}
  .nav-tel{display:flex; align-items:center; gap:0.4em; text-decoration:none; color:var(--ink); font-weight:600; font-size:0.92rem}
  .nav-tel svg{flex:none}
  .hamburger{display:none; flex-direction:column; gap:5px; background:none; border:0; cursor:pointer; padding:0.4rem}
  .hamburger span{width:22px; height:2px; background:var(--ink); border-radius:2px}
  @media (max-width:900px){
    .nav-links{position:fixed; inset:64px 0 auto 0; flex-direction:column; background:var(--cream);
      padding:1.25rem clamp(1.25rem,4vw,2.5rem) 1.75rem; border-bottom:1px solid var(--line);
      transform:translateY(-130%); transition:transform .25s ease; gap:1rem; box-shadow:var(--shadow-sm)}
    .nav-links.open{transform:translateY(0)}
    .nav-right .btn-primary{display:none}
    .hamburger{display:flex}
  }
  @media (max-width:480px){
    .brand{font-size:1rem}
    .tel-text{display:none}
    .nav-tel{padding:0.3rem}
  }

  /* ============ TEXTURE PLACEHOLDERS (no stock photos used) ============ */
  .grain{
    position:relative; overflow:hidden; background:
      repeating-linear-gradient(100deg, var(--forest-tint) 0px, var(--forest-tint) 1px, transparent 1px, transparent 9px),
      linear-gradient(150deg, var(--cream-deep), var(--paper) 65%);
  }
  .grain::after{
    content:""; position:absolute; inset:0;
    background:radial-gradient(120% 90% at 15% 10%, rgba(198,154,46,0.10), transparent 60%);
  }
  .placeholder-tag{
    position:absolute; left:0.9rem; bottom:0.9rem; z-index:2;
    background:color-mix(in srgb, var(--paper) 88%, transparent);
    border:1px solid var(--line); color:var(--ink-soft);
    font-size:0.72rem; padding:0.35rem 0.65rem; border-radius:100px;
    font-family:'Archivo',sans-serif; letter-spacing:0.02em;
  }
  .ph-icon{position:relative; z-index:1; display:flex; align-items:center; justify-content:center; height:100%; color:var(--forest); opacity:0.45}

  /* ============ HERO ============ */
  .hero{padding-top:clamp(3rem,7vw,5.5rem)}
  .hero .wrap{display:grid; grid-template-columns:1.05fr 0.95fr; gap:clamp(2rem,5vw,4rem); align-items:center}
  .hero h1{font-size:clamp(2.3rem,4.4vw,3.5rem); line-height:1.08}
  .hero-lede{font-size:1.15rem; color:var(--ink-soft); max-width:46ch}
  .hero-actions{display:flex; align-items:center; gap:1.4rem; flex-wrap:wrap; margin-top:1.6rem}
  .hero-call{display:flex; align-items:center; gap:0.5em; text-decoration:none; color:var(--ink); font-weight:600; font-size:0.95rem}
  .hero-media{position:relative}
  .hero-media .grain{aspect-ratio:4/5; border-radius:var(--radius-lg); box-shadow:var(--shadow)}
  .rating-float{
    position:absolute; left:-1.3rem; bottom:1.6rem; z-index:3;
    background:var(--paper); border:1px solid var(--line); box-shadow:var(--shadow);
    border-radius:var(--radius-lg); padding:0.9rem 1.15rem; display:flex; gap:0.75rem; align-items:center;
    max-width:210px;
  }
  .rating-float .stars{color:var(--brass); font-size:0.95rem; letter-spacing:0.05em}
  .rating-float strong{display:block; font-size:0.95rem}
  .rating-float span{display:block; font-size:0.76rem; color:var(--ink-soft)}
  @media (max-width:900px){
    .hero .wrap{grid-template-columns:1fr}
    .hero-media{order:-1}
    .rating-float{left:1rem}
  }

  /* trust strip */
  .trust-strip{background:var(--cream-deep); border-top:1px solid var(--line); border-bottom:1px solid var(--line)}
  .trust-strip .wrap{display:grid; grid-template-columns:repeat(3,1fr); gap:2rem; padding:2.1rem clamp(1.25rem,4vw,2.5rem)}
  .trust-item{text-align:center}
  .trust-item strong{display:block; font-family:'Fraunces',serif; font-size:1.5rem; color:var(--forest); font-weight:560}
  .trust-item span{font-size:0.85rem; color:var(--ink-soft)}
  @media (max-width:720px){.trust-strip .wrap{grid-template-columns:1fr; gap:1.4rem}}

  /* ============ ABOUT ============ */
  .about .wrap{display:grid; grid-template-columns:0.78fr 1.22fr; gap:clamp(2rem,5vw,4rem); align-items:start}
  .about-media .grain{aspect-ratio:3/4; border-radius:var(--radius-lg); box-shadow:var(--shadow-sm)}
  .about-quote{
    border-top:1px solid var(--line); border-bottom:1px solid var(--line);
    padding:1.6rem 0; margin:1.6rem 0; position:relative;
  }
  .about-quote .mark{font-family:'Fraunces',serif; font-style:italic; color:var(--brass); font-size:2.2rem; line-height:0; position:relative; top:0.6rem}
  .about-quote p{font-family:'Fraunces',serif; font-size:1.2rem; font-style:italic; color:var(--ink); line-height:1.55; font-weight:440}
  .about-quote cite{display:block; margin-top:0.9rem; font-style:normal; font-family:'Archivo',sans-serif; font-size:0.82rem; color:var(--ink-soft)}
  @media (max-width:860px){.about .wrap{grid-template-columns:1fr}}

  /* ============ SERVICES ============ */
  .services-grid{display:grid; grid-template-columns:repeat(3,1fr); gap:1.5rem}
  .service-card{
    background:var(--paper); border:1px solid var(--line); border-radius:var(--radius-lg);
    padding:2rem 1.75rem; transition:transform .2s ease, box-shadow .2s ease;
  }
  .service-card:hover{transform:translateY(-5px); box-shadow:var(--shadow-sm)}
  .service-num{font-family:'Fraunces',serif; font-style:italic; color:var(--brass-soft); font-size:1rem; display:block; margin-bottom:0.9rem}
  .service-card h3{font-size:1.2rem; margin-bottom:0.55em}
  .service-card p{color:var(--ink-soft); font-size:0.96rem; margin-bottom:0}
  @media (max-width:860px){.services-grid{grid-template-columns:1fr}}

  /* ============ GALLERY ============ */
  .gallery-grid{display:grid; grid-template-columns:repeat(3,1fr); gap:1.25rem}
  .gallery-item{position:relative}
  .gallery-item .grain{aspect-ratio:1/1; border-radius:var(--radius)}
  .gallery-cap{margin-top:0.7rem}
  .gallery-cap strong{display:block; font-size:0.95rem; font-weight:600}
  .gallery-cap span{font-size:0.8rem; color:var(--ink-faint)}
  .gallery-item:nth-child(2){grid-row:span 1}
  @media (max-width:860px){.gallery-grid{grid-template-columns:repeat(2,1fr)}}
  @media (max-width:560px){.gallery-grid{grid-template-columns:1fr}}

  /* ============ REVIEWS ============ */
  .reviews-top{display:flex; align-items:baseline; gap:1.5rem; flex-wrap:wrap; margin-bottom:2.5rem}
  .review-score{display:flex; align-items:center; gap:0.9rem}
  .review-score .num{font-family:'Fraunces',serif; font-size:2.6rem; font-weight:560; line-height:1}
  .review-score .stars{color:var(--brass); letter-spacing:0.06em}
  .review-score-sub{font-size:0.85rem; color:var(--ink-soft)}
  .review-divider{width:1px; height:36px; background:var(--line)}
  .reviews-grid{display:grid; grid-template-columns:repeat(3,1fr); gap:1.5rem}
  .review-card{
    background:var(--paper); border:1px solid var(--line); border-radius:var(--radius-lg);
    padding:1.75rem; position:relative;
  }
  .review-card .mark{font-family:'Fraunces',serif; font-style:italic; color:var(--brass); font-size:1.8rem; line-height:0; display:block; margin-bottom:0.9rem}
  .review-card p{font-size:0.95rem; color:var(--ink); margin-bottom:1.1rem}
  .review-card cite{font-style:normal; display:flex; flex-direction:column; gap:0.15rem; font-size:0.82rem; color:var(--ink-soft); border-top:1px solid var(--line); padding-top:0.85rem}
  .review-card cite b{color:var(--ink); font-weight:600}
  @media (max-width:860px){.reviews-grid{grid-template-columns:1fr}}

  /* ============ HOURS / LOCATION ============ */
  .hours-loc{background:var(--cream-deep)}
  .hours-loc .wrap{display:grid; grid-template-columns:1fr 1fr; gap:clamp(2rem,5vw,4rem)}
  .hours-table{width:100%; border-collapse:collapse; margin:1.3rem 0 1.5rem}
  .hours-table td{padding:0.55rem 0; border-bottom:1px solid var(--line); font-size:0.95rem}
  .hours-table td:last-child{text-align:right; color:var(--ink-soft)}
  .hours-note{font-size:0.88rem; color:var(--ink-soft); border-left:2px solid var(--brass); padding-left:0.9rem}
  .map-card{
    background:var(--paper); border:1px solid var(--line); border-radius:var(--radius-lg);
    padding:1.75rem; box-shadow:var(--shadow-sm);
  }
  .pin{width:38px; height:38px; border-radius:50%; background:var(--forest-tint); display:flex; align-items:center; justify-content:center; color:var(--forest); margin-bottom:1rem}
  .map-card address{font-style:normal; line-height:1.6; margin-bottom:1.1rem}
  .contact-row{display:flex; flex-direction:column; gap:0.65rem; margin-bottom:1.3rem}
  .contact-row a{display:flex; align-items:center; gap:0.6em; text-decoration:none; font-size:0.95rem; color:var(--ink)}
  .contact-row a:hover{color:var(--forest)}
  @media (max-width:860px){.hours-loc .wrap{grid-template-columns:1fr}}

  /* ============ CONTACT FORM ============ */
  .contact-form{background:var(--paper); border:1px solid var(--line); border-radius:var(--radius-lg); padding:clamp(1.75rem,4vw,2.75rem); box-shadow:var(--shadow-sm)}
  .form-grid{display:grid; grid-template-columns:1fr 1fr; gap:1.1rem}
  .form-grid .full{grid-column:1/-1}
  label{display:flex; flex-direction:column; gap:0.4rem; font-size:0.85rem; font-weight:600; color:var(--ink)}
  input,textarea,select{
    font-family:'Archivo',sans-serif; font-size:0.95rem; padding:0.75rem 0.85rem;
    border:1px solid var(--line); border-radius:6px; background:var(--cream); color:var(--ink);
  }
  input:focus,textarea:focus,select:focus{outline:2px solid var(--forest); outline-offset:1px}
  textarea{resize:vertical; min-height:110px}
  .form-foot{display:flex; align-items:center; justify-content:space-between; flex-wrap:wrap; gap:1rem; margin-top:1.4rem}
  .or-call{font-size:0.86rem; color:var(--ink-soft)}
  .or-call a{color:var(--forest); font-weight:600; text-decoration:none}
  .contact-head{display:grid; grid-template-columns:1fr 1fr; gap:clamp(2rem,5vw,4rem); align-items:start; margin-bottom:2.5rem}
  @media (max-width:860px){.contact-head{grid-template-columns:1fr} .form-grid{grid-template-columns:1fr}}

  /* ============ FOOTER ============ */
  footer{background:var(--ink); color:var(--cream); padding:3rem 0 2rem}
  footer .wrap{display:flex; flex-wrap:wrap; justify-content:space-between; gap:2rem}
  footer .f-brand{font-family:'Fraunces',serif; font-size:1.3rem; margin-bottom:0.6rem; font-weight:560}
  footer .f-col p, footer .f-col a{color:rgba(248,243,233,0.7); font-size:0.9rem; text-decoration:none; margin-bottom:0.4rem; display:block}
  footer .f-col a:hover{color:var(--brass)}
  footer .f-bottom{border-top:1px solid rgba(248,243,233,0.15); margin-top:2.5rem; padding-top:1.5rem; text-align:center; font-size:0.8rem; color:rgba(248,243,233,0.5)}
</style>
</head>
<body>


<header class="site-nav">
  <div class="wrap">
    <a href="#top" class="brand">Gianni Corvasce <em>Restoration</em></a>
    <nav>
      <ul class="nav-links" id="navLinks">
        <li><a href="#about">About</a></li>
        <li><a href="#services">Services</a></li>
        <li><a href="#gallery">Gallery</a></li>
        <li><a href="#reviews">Reviews</a></li>
        <li><a href="#visit">Visit</a></li>
      </ul>
    </nav>
    <div class="nav-right">
      <a class="nav-tel" href="tel:+15103254552" aria-label="Call (510) 325-4552">
        <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
        <span class="tel-text">(510) 325-4552</span>
      </a>
      <a class="btn btn-primary btn-sm" href="#contact">Request a Quote</a>
    </div>
    <button class="hamburger" id="hamburger" aria-label="Menu" aria-expanded="false">
      <span></span><span></span><span></span>
    </button>
  </div>
</header>

<main id="top">

  <!-- ============ HERO ============ -->
  <section class="hero">
    <div class="wrap">
      <div class="hero-copy">
        <p class="eyebrow">Berkeley, CA &middot; ActivSpace Workshop</p>
        <h1>Furniture restoration worth passing down.</h1>
        <p class="hero-lede">Gianni Corvasce repairs and refinishes fine furniture, cabinetry, and doors from a family trade rooted in three generations of Italian craftsmanship. It's the kind of work that turns a cracked heirloom back into the piece your family gathers around.</p>
        <div class="hero-actions">
          <a class="btn btn-primary" href="#contact">Request a Quote</a>
          <a class="hero-call" href="tel:+15103254552">
            <svg width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
            or call (510) 325-4552
          </a>
        </div>
      </div>
      <div class="hero-media">
        <div class="grain">
          <div class="ph-icon">
            <svg width="52" height="52" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M4 14h16M6 14V6a2 2 0 0 1 2-2h8a2 2 0 0 1 2 2v8M6 14l-1.5 6M18 14l1.5 6M4.5 20h15"/></svg>
          </div>
          <span class="placeholder-tag">Add a finished-piece photo here</span>
        </div>
        <div class="rating-float">
          <span class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span>
          <div><strong>4.9 / 5.0</strong><span>44 Yelp reviews &middot; 5.0 on Google</span></div>
        </div>
      </div>
    </div>
  </section>

  <div class="trust-strip">
    <div class="wrap">
      <div class="trust-item"><strong>3</strong><span>Generations of Italian craftsmanship</span></div>
      <div class="trust-item"><strong>4.9&#9733;</strong><span>Average rating across 44 Yelp reviews</span></div>
      <div class="trust-item"><strong>100%</strong><span>Real reviews, no fabricated testimonials</span></div>
    </div>
  </div>

  <!-- ============ ABOUT ============ -->
  <section class="about reveal" id="about">
    <div class="wrap">
      <div class="about-media">
        <div class="grain">
          <div class="ph-icon">
            <svg width="46" height="46" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><circle cx="12" cy="8" r="4"/><path d="M4 21c0-4.4 3.6-8 8-8s8 3.6 8 8"/></svg>
          </div>
          <span class="placeholder-tag">Add a headshot of Gianni</span>
        </div>
      </div>
      <div class="about-copy">
        <p class="eyebrow">The Craftsman</p>
        <h2>A family trade, still done by hand.</h2>
        <p>Gianni Corvasce learned restoration the way it's been done in his family for three generations. He strips, stains, and lacquers by hand, one piece at a time, out of his workshop at ActivSpace on Seventh Street. He works on everything from dining chairs to cabinetry, exterior doors, and flooring finishes, and takes on custom furniture painting as well.</p>
        <div class="about-quote">
          <span class="mark">&#8220;</span>
          <p>Each piece of furniture has its own unique needs. At certain times of the year I'm unable to take on smaller work and I'm often away from the shop, but I try to be accommodating.</p>
          <cite>&mdash; Gianni Corvasce, in his own words (Yelp)</cite>
        </div>
        <p>It's a philosophy his customers notice: reviewers repeatedly mention that he'll tell you honestly when a piece isn't worth restoring, rather than take the work anyway.</p>
      </div>
    </div>
  </section>

  <!-- ============ SERVICES ============ -->
  <section class="reveal" id="services">
    <div class="wrap">
      <div class="section-head">
        <p class="eyebrow">What He Restores</p>
        <h2>Three ways to bring a piece back</h2>
        <p>Every restoration starts with an honest look at the piece and what it actually needs.</p>
      </div>
      <div class="services-grid">
        <article class="service-card">
          <span class="service-num">01</span>
          <h3>Furniture Repair &amp; Refinishing</h3>
          <p>Touch-ups to full refinishing: stripping, sanding, staining, painting, and lacquering for chairs, tables, and case pieces of any age.</p>
        </article>
        <article class="service-card">
          <span class="service-num">02</span>
          <h3>Heirloom &amp; Antique Restoration</h3>
          <p>Dressers, mission-style coffee tables, dining sets, and family pieces passed down for generations, including a 100-year-old dining chair and a 60-year-old family highchair, restored intact.</p>
        </article>
        <article class="service-card">
          <span class="service-num">03</span>
          <h3>Cabinetry, Doors &amp; Built-ins</h3>
          <p>Interior cabinets, exterior doors, and flooring finishes, plus custom furniture painting for pieces that need a new look rather than an old one back.</p>
        </article>
      </div>
    </div>
  </section>

  <!-- ============ GALLERY ============ -->
  <section class="reveal" id="gallery" style="background:var(--cream-deep)">
    <div class="wrap">
      <div class="section-head">
        <p class="eyebrow">Recent Work</p>
        <h2>A few pieces, before they were finished</h2>
        <p>Placeholders below. Swap each one for a real before/after photo once Gianni sends them over.</p>
      </div>
      <div class="gallery-grid">
        <div class="gallery-item">
          <div class="grain"><div class="ph-icon"><svg width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M6 3v18M18 3v18M6 8h12M6 16h12"/></svg></div></div>
          <div class="gallery-cap"><strong>Dining Chair Repair</strong><span>Frame regluing &amp; reupholstery</span></div>
        </div>
        <div class="gallery-item">
          <div class="grain"><div class="ph-icon"><svg width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><rect x="4" y="9" width="16" height="8" rx="1"/><path d="M4 9V6a2 2 0 0 1 2-2h12a2 2 0 0 1 2 2v3M8 17v2M16 17v2"/></svg></div></div>
          <div class="gallery-cap"><strong>Mission Coffee Table</strong><span>Water-ring &amp; finish restoration</span></div>
        </div>
        <div class="gallery-item">
          <div class="grain"><div class="ph-icon"><svg width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><rect x="5" y="3" width="14" height="18" rx="1"/><path d="M5 9h14M5 15h14"/></svg></div></div>
          <div class="gallery-cap"><strong>Mid-Century Dresser</strong><span>Scratch &amp; water-damage repair</span></div>
        </div>
        <div class="gallery-item">
          <div class="grain"><div class="ph-icon"><svg width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M7 21V9a5 5 0 0 1 10 0v12M4 21h16"/></svg></div></div>
          <div class="gallery-cap"><strong>Antique Highchair</strong><span>Guard rail rebuild, new hardware</span></div>
        </div>
        <div class="gallery-item">
          <div class="grain"><div class="ph-icon"><svg width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M3 7h18M6 7v13a1 1 0 0 0 1 1h10a1 1 0 0 0 1-1V7M9 7V4a1 1 0 0 1 1-1h4a1 1 0 0 1 1 1v3"/></svg></div></div>
          <div class="gallery-cap"><strong>Cabinet &amp; Door Refinish</strong><span>Interior cabinetry, exterior doors</span></div>
        </div>
        <div class="gallery-item">
          <div class="grain"><div class="ph-icon"><svg width="34" height="34" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.4"><path d="M12 19l7-7 3 3-7 7-3-3zM18 13l-1.5-7.5L2 2l3.5 14.5L13 18l5-5z"/></svg></div></div>
          <div class="gallery-cap"><strong>Custom Furniture Painting</strong><span>Full color &amp; finish changes</span></div>
        </div>
      </div>
    </div>
  </section>

  <!-- ============ REVIEWS ============ -->
  <section class="reveal" id="reviews">
    <div class="wrap">
      <div class="reviews-top">
        <div class="review-score">
          <span class="num">4.9</span>
          <div><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span><div class="review-score-sub">44 reviews on Yelp</div></div>
        </div>
        <div class="review-divider"></div>
        <div class="review-score">
          <span class="num">5.0</span>
          <div><span class="stars">&#9733;&#9733;&#9733;&#9733;&#9733;</span><div class="review-score-sub">Google Business reviews</div></div>
        </div>
      </div>
      <div class="reviews-grid">
        <article class="review-card">
          <span class="mark">&#8220;</span>
          <p>Gianni works miracles. One of my 100-plus-year-old dining room chairs was broken and I didn't think it was fixable. He made it look new. He does fantastic work.</p>
          <cite><b>Matt G.</b>Oakland, CA &middot; Yelp</cite>
        </article>
        <article class="review-card">
          <span class="mark">&#8220;</span>
          <p>Thank you for the outstanding job restoring and modernizing our family heirloom. You gave honest feedback about what could and couldn't be done. For anyone considering furniture restoration, Gianni is your guy.</p>
          <cite><b>Adam K.</b>San Bruno, CA &middot; Yelp</cite>
        </article>
        <article class="review-card">
          <span class="mark">&#8220;</span>
          <p>I brought in an antique English child's highchair that's been in my family for over 60 years. He took pride in finding and adding an antique crystal door knob, which I love. It adds sparkle to the chair.</p>
          <cite><b>Tori E.</b>Oakland, CA &middot; Yelp</cite>
        </article>
        <article class="review-card">
          <span class="mark">&#8220;</span>
          <p>Gianni did a fabulous job on an antique dresser I inherited from my mother. He was great to work with, very professional, and the piece turned out great.</p>
          <cite><b>Kristin M.</b>Alameda, CA &middot; Yelp</cite>
        </article>
        <article class="review-card">
          <span class="mark">&#8220;</span>
          <p>He really knows his stuff and cares so much about the details. My mid-century dresser had a lot of scratches and water damage and now looks brand new. Highly recommend.</p>
          <cite><b>Molly R.</b>Berkeley, CA &middot; Yelp</cite>
        </article>
        <article class="review-card">
          <span class="mark">&#8220;</span>
          <p>Gianni restored my old Mission-style coffee table. It was a mess: water rings, discoloration, damage from kids and cats. Now I actually enjoy looking at it.</p>
          <cite><b>Catherine P.</b>Oakland, CA &middot; Yelp</cite>
        </article>
      </div>
    </div>
  </section>

  <!-- ============ HOURS & LOCATION ============ -->
  <section class="hours-loc reveal" id="visit">
    <div class="wrap">
      <div class="hours-copy">
        <p class="eyebrow">Visit the Workshop</p>
        <h2>Hours &amp; drop-off</h2>
        <table class="hours-table">
          <tr><td>Monday &ndash; Friday</td><td>By appointment</td></tr>
          <tr><td>Saturday</td><td>By appointment</td></tr>
          <tr><td>Sunday</td><td>Closed</td></tr>
        </table>
        <p class="hours-note">Gianni works seasonally around larger projects, so hours vary. Call or email ahead to schedule a drop-off or shop visit.</p>
      </div>
      <div class="map-card">
        <div class="pin">
          <svg width="18" height="18" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M21 10c0 6-9 13-9 13s-9-7-9-13a9 9 0 0 1 18 0z"/><circle cx="12" cy="10" r="3"/></svg>
        </div>
        <address>
          2703 Seventh St, Suite 151 (ActivSpace)<br>
          Berkeley, CA 94710
        </address>
        <div class="contact-row">
          <a href="tel:+15103254552">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
            (510) 325-4552
          </a>
          <a href="mailto:giannicorvasce@yahoo.com">
            <svg width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2"><path d="M4 4h16v16H4z"/><path d="m22 6-10 7L2 6"/></svg>
            giannicorvasce@yahoo.com
          </a>
        </div>
        <a class="btn btn-ghost btn-sm" href="https://www.google.com/maps/search/?api=1&query=2703+Seventh+St+Berkeley+CA+94710" target="_blank" rel="noopener">Get Directions</a>
      </div>
    </div>
  </section>

  <!-- ============ CONTACT ============ -->
  <section class="reveal" id="contact">
    <div class="wrap">
      <div class="contact-head">
        <div>
          <p class="eyebrow">Start a Restoration</p>
          <h2>Tell him what you've got.</h2>
          <p style="color:var(--ink-soft)">A few details and a photo or two is usually enough for a first estimate. Gianni will follow up to talk through what the piece needs.</p>
        </div>
      </div>
      <form class="contact-form" onsubmit="return false;">
        <div class="form-grid">
          <label class="full">Name
            <input type="text" name="name" required>
          </label>
          <label>Phone
            <input type="tel" name="phone">
          </label>
          <label>Email
            <input type="email" name="email">
          </label>
          <label class="full">What needs restoring?
            <textarea name="message" placeholder="e.g. a dining table with water damage and two loose legs" required></textarea>
          </label>
        </div>
        <div class="form-foot">
          <button class="btn btn-primary" type="submit">Request a Quote</button>
          <p class="or-call">Prefer to talk it through? <a href="tel:+15103254552">Call (510) 325-4552</a></p>
        </div>
      </form>
    </div>
  </section>

</main>

<footer>
  <div class="wrap">
    <div class="f-col">
      <div class="f-brand">Gianni Corvasce Restoration</div>
      <p>2703 Seventh St, Suite 151<br>Berkeley, CA 94710</p>
    </div>
    <div class="f-col">
      <a href="tel:+15103254552">(510) 325-4552</a>
      <a href="mailto:giannicorvasce@yahoo.com">giannicorvasce@yahoo.com</a>
      <a href="#contact">Request a Quote</a>
    </div>
    <div class="f-col">
      <a href="#about">About</a>
      <a href="#services">Services</a>
      <a href="#gallery">Gallery</a>
      <a href="#reviews">Reviews</a>
    </div>
  </div>
  <div class="f-bottom wrap">Mockup built by Parra Marketing Solutions &middot; not yet the live site of Gianni Corvasce Restoration</div>
</footer>

<script>
  const hb = document.getElementById('hamburger');
  const nl = document.getElementById('navLinks');
  hb.addEventListener('click', () => {
    const open = nl.classList.toggle('open');
    hb.setAttribute('aria-expanded', open);
  });
  nl.querySelectorAll('a').forEach(a => a.addEventListener('click', () => {
    nl.classList.remove('open');
    hb.setAttribute('aria-expanded', 'false');
  }));

  if (!window.matchMedia('(prefers-reduced-motion: reduce)').matches) {
    const io = new IntersectionObserver((entries) => {
      entries.forEach(e => { if (e.isIntersecting) e.target.classList.add('in-view'); });
    }, { threshold: 0.12 });
    document.querySelectorAll('.reveal').forEach(s => io.observe(s));
  } else {
    document.querySelectorAll('.reveal').forEach(s => s.classList.add('in-view'));
  }
</script>

</body>
</html>
