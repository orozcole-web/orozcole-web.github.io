# orozcole-web.github.io
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>charity: water — Real People. Real Water. Real Results.</title>
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Archivo:wght@400;500;700;800&family=Roboto+Slab:wght@400;500&display=swap" rel="stylesheet">
<style>
  :root {
    --black: #0a0a0a;
    --cream: #f7f3e9;
    --yellow: #FFC907;
    --yellow-dark: #f2b705;
    --text-muted: #cfcfc9;
    --max-width: 1280px;
  }

  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }

  body {
    background-color: var(--black);
    font-family: 'Archivo', sans-serif;
    color: var(--cream);
  }

  a {
    text-decoration: none;
    color: inherit;
  }

  .container {
    max-width: var(--max-width);
    margin: 0 auto;
  }

  /* ---------- Header ---------- */

  header {
    border-bottom: 1px solid rgba(247, 243, 233, 0.15);
  }

  .header-inner {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 24px 40px;
  }

  .logo {
    display: flex;
    align-items: center;
    gap: 10px;
    font-family: 'Roboto Slab', serif;
    font-size: 1.5rem;
    letter-spacing: 0.03em;
  }

  .logo-icon {
    width: 28px;
    height: 28px;
    flex-shrink: 0;
  }

  nav {
    display: flex;
    align-items: center;
    gap: 40px;
  }

  .nav-links {
    display: flex;
    gap: 36px;
    list-style: none;
  }

  .nav-links a {
    font-size: 1rem;
    font-weight: 500;
    transition: opacity 0.2s ease;
  }

  .nav-links a:hover,
  .nav-links a:focus-visible {
    opacity: 0.7;
  }

  .btn-donate {
    border: 1.5px solid var(--yellow);
    color: var(--yellow);
    font-weight: 700;
    padding: 12px 28px;
    border-radius: 999px;
    font-size: 1rem;
    transition: background-color 0.2s ease, color 0.2s ease;
    white-space: nowrap;
  }

  .btn-donate:hover,
  .btn-donate:focus-visible {
    background-color: var(--yellow);
    color: var(--black);
  }

  /* ---------- Hero ---------- */

  .hero {
    display: grid;
    grid-template-columns: 1fr 1fr;
    align-items: stretch;
    min-height: 700px;
  }

  .hero-content {
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding: 40px 40px 60px;
    max-width: 640px;
  }

  .hero-content h1 {
    font-family: 'Archivo', sans-serif;
    font-weight: 800;
    font-size: 4.2rem;
    line-height: 1.05;
    letter-spacing: -0.01em;
    color: var(--cream);
  }

  .hero-content p {
    margin-top: 28px;
    font-size: 1.15rem;
    line-height: 1.6;
    color: var(--text-muted);
    max-width: 520px;
  }

  .btn-cta {
    display: inline-block;
    margin-top: 36px;
    background-color: var(--yellow);
    color: var(--black);
    font-weight: 700;
    font-size: 1.15rem;
    padding: 22px 36px;
    border-radius: 999px;
    width: fit-content;
    border: none;
    cursor: pointer;
    transition: transform 0.15s ease, background-color 0.2s ease;
  }

  .btn-cta:hover,
  .btn-cta:focus-visible {
    background-color: var(--yellow-dark);
    transform: translateY(-2px);
  }

  .hero-image {
    position: relative;
    overflow: hidden;
    background: radial-gradient(circle at 30% 20%, #2a5a63 0%, #123039 45%, #060b0c 100%);
  }

  .hero-image img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
  }

  /* Fallback visual treatment if no photo is supplied */
  .hero-image .placeholder-note {
    position: absolute;
    inset: 0;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    padding: 40px;
    color: rgba(247, 243, 233, 0.5);
    font-size: 0.95rem;
    line-height: 1.6;
  }

  /* ---------- Responsive ---------- */

  @media (max-width: 960px) {
    .header-inner {
      padding: 20px;
    }

    .nav-links {
      display: none;
    }

    .hero {
      grid-template-columns: 1fr;
      min-height: unset;
    }

    .hero-content {
      padding: 48px 24px;
      max-width: 100%;
    }

    .hero-content h1 {
      font-size: 2.8rem;
    }

    .hero-image {
      min-height: 420px;
    }
  }

  @media (max-width: 480px) {
    .hero-content h1 {
      font-size: 2.2rem;
    }

    .logo span {
      font-size: 1.2rem;
    }

    .btn-donate {
      padding: 10px 18px;
      font-size: 0.9rem;
    }
  }

  @media (prefers-reduced-motion: reduce) {
    * {
      transition: none !important;
    }
  }
</style>
</head>
<body>

<header>
  <div class="header-inner">
    <a href="#" class="logo">
      <svg class="logo-icon" viewBox="0 0 32 32" fill="none" xmlns="http://www.w3.org/2000/svg" aria-hidden="true">
        <rect x="2" y="4" width="28" height="24" rx="3" fill="#FFC907"/>
        <circle cx="16" cy="16" r="6" fill="#0a0a0a"/>
        <rect x="13" y="2" width="6" height="4" rx="1" fill="#FFC907"/>
      </svg>
      <span>charity: water</span>
    </a>
    <nav>
      <ul class="nav-links">
        <li><a href="#">Take Action</a></li>
        <li><a href="#">About Us</a></li>
        <li><a href="#">Why Water?</a></li>
      </ul>
      <a href="#donate" class="btn-donate">Donate</a>
    </nav>
  </div>
</header>

<main>
  <section class="hero container">
    <div class="hero-content">
      <h1>Real People.<br>Real Water.<br>Real Results.</h1>
      <p>100% of your donation funds clean water projects, complete with GPS coordinates and photos of the source you helped build, ensuring you know where your dollar's going.</p>
      <button class="btn-cta">Give Clean Water</button>
    </div>
    <div class="hero-image">
      <!-- Replace the src below with your own photo of a project beneficiary -->
      <img src="your-photo.jpg" alt="A woman smiling as clean water splashes over her face and shoulders" onerror="this.style.display='none'; this.nextElementSibling.style.display='flex';">
      <div class="placeholder-note" style="display:none;">
        Drop in your hero photo here<br>(e.g. your-photo.jpg)
      </div>
    </div>
  </section>
</main>

</body>
</html>
