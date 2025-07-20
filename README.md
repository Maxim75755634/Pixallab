<!DOCTYPE html>
<html lang="fa" data-theme="light">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>سایت شخصی من</title>

  <!-- فونت فارسی Vazir -->
  <link href="https://cdn.fontcdn.ir/Font/Persian/Vazir/Vazir.css" rel="stylesheet" />

  <!-- آیکون‌ها -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.10.5/font/bootstrap-icons.css" />

  <style>
    :root {
      --bg: #f5f5f5;
      --text: #333;
      --header-bg: #0a192f;
      --hero-bg: linear-gradient(to right, #0f2027, #203a43, #2c5364);
      --section-title: #0077cc;
      --link: #0088cc;
      --footer-bg: #0a192f;
      --card-bg: white;
      --card-shadow: rgba(0,0,0,0.1);
    }

    [data-theme='dark'] {
      --bg: #121212;
      --text: #f0f0f0;
      --header-bg: #1e1e1e;
      --hero-bg: linear-gradient(to right, #111, #222, #333);
      --section-title: #64ffda;
      --link: #26a69a;
      --footer-bg: #1e1e1e;
      --card-bg: #1f1f1f;
      --card-shadow: rgba(0,0,0,0.7);
    }

    body {
      margin: 0;
      font-family: 'Vazir', sans-serif;
      background-color: var(--bg);
      color: var(--text);
      direction: rtl;
      transition: all 0.3s ease;
    }

    header {
      background-color: var(--header-bg);
      color: white;
      padding: 20px 0;
      text-align: center;
      position: relative;
    }

    nav a {
      color: white;
      margin: 0 15px;
      text-decoration: none;
      font-weight: bold;
    }

    nav a:hover {
      color: var(--link);
    }

    .theme-toggle {
      position: absolute;
      left: 15px;
      top: 15px;
      background: transparent;
      border: none;
      color: white;
      font-size: 1.3em;
      cursor: pointer;
    }

    .hero {
      padding: 80px 20px;
      text-align: center;
      background: var(--hero-bg);
      color: white;
    }

    .hero h1 {
      margin-bottom: 10px;
      font-size: 2.5em;
    }

    .hero p {
      font-size: 1.2em;
      color: #cccccc;
    }

    .section {
      padding: 60px 20px;
      text-align: center;
    }

    .section h2 {
      color: var(--section-title);
      margin-bottom: 20px;
    }

    /* استایل کارت‌ها */
    .portfolio-cards {
      display: grid;
      grid-template-columns: repeat(auto-fit,minmax(250px,1fr));
      gap: 20px;
      max-width: 1000px;
      margin: 0 auto;
    }

    .card {
      background-color: var(--card-bg);
      box-shadow: 0 4px 8px var(--card-shadow);
      border-radius: 10px;
      overflow: hidden;
      text-align: right;
      transition: transform 0.3s ease;
      cursor: pointer;
    }

    .card:hover {
      transform: translateY(-10px);
      box-shadow: 0 8px 16px var(--card-shadow);
    }

    .card img {
      width: 100%;
      height: 160px;
      object-fit: cover;
      display: block;
    }

    .card-body {
      padding: 15px;
    }

    .card-title {
      font-size: 1.2em;
      margin: 0 0 10px 0;
      color: var(--section-title);
    }

    .card-desc {
      font-size: 0.95em;
      color: var(--text);
      min-height: 50px;
      margin-bottom: 15px;
    }

    .card-link {
      text-decoration: none;
      color: var(--link);
      font-weight: bold;
      display: inline-flex;
      align-items: center;
    }

    .card-link i {
      margin-left: 5px;
      font-size: 1.1em;
    }

    .telegram-link {
      display: inline-block;
      margin-top: 15px;
      font-size: 1.2em;
      color: var(--link);
      text-decoration: none;
    }

    .telegram-link i {
      font-size: 1.5em;
      vertical-align: middle;
      margin-left: 5px;
    }

    footer {
      background-color: var(--footer-bg);
      color: white;
      text-align: center;
      padding: 20px 0;
      font-size: 0.9em;
    }

    @media (max-width: 600px) {
      .hero h1 {
        font-size: 2em;
      }
    }
  </style>
</head>
<body>

  <header>
    <button class="theme-toggle" onclick="toggleTheme()" title="تغییر حالت روز/شب">
      <i class="bi bi-moon-stars"></i>
    </button>
    <nav>
      <a href="#about">درباره من</a>
      <a href="#portfolio">نمونه‌کارها</a>
      <a href="#contact">ارتباط با من</a>
    </nav>
  </header>

  <section class="hero">
    <h1>سلام، من مجید هستم</h1>
    <p>طراح و توسعه‌دهنده وب، عاشق سادگی و سرعت</p>
  </section>

  <section class="section" id="about">
    <h2>درباره من</h2>
    <p>من یک برنامه‌نویس فرانت‌اند هستم که با HTML, CSS, JS سایت‌های سریع و مدرن طراحی می‌کنم.</p>
  </section>

  <section class="section" id="portfolio">
    <h2>نمونه‌کارها</h2>

    <div class="portfolio-cards">

      <div class="card">
        <img src="https://via.placeholder.com/400x250?text=پروژه+۱" alt="پروژه ۱" />
        <div class="card-body">
          <h3 class="card-title">پروژه اول</h3>
          <p class="card-desc">یک سایت شرکتی ساده و واکنش‌گرا با طراحی مدرن.</p>
          <a href="#" class="card-link" target="_blank">مشاهده پروژه <i class="bi bi-arrow-left"></i></a>
        </div>
      </div>

      <div class="card">
        <img src="https://via.placeholder.com/400x250?text=پروژه+۲" alt="پروژه ۲" />
        <div class="card-body">
          <h3 class="card-title">پروژه دوم</h3>
          <p class="card-desc">یک فروشگاه آنلاین با امکانات کامل و طراحی ساده.</p>
          <a href="#" class="card-link" target="_blank">مشاهده پروژه <i class="bi bi-arrow-left"></i></a>
        </div>
      </div>

      <div class="card">
        <img src="https://via.placeholder.com/400x250?text=پروژه+۳" alt="پروژه ۳" />
        <div class="card-body">
          <h3 class="card-title">پروژه سوم</h3>
          <p class="card-desc">وب‌اپلیکیشنی برای مدیریت کارهای روزانه.</p>
          <a href="#" class="card-link" target="_blank">مشاهده پروژه <i class="bi bi-arrow-left"></i></a>
        </div>
      </div>

    </div>

  </section>

  <section class="section" id="contact">
    <h2>ارتباط با من</h2>
    <p>برای ارتباط سریع از طریق تلگرام کلیک کنید:</p>
    <a href="https://t.me/YourTelegramUsername" class="telegram-link" target="_blank">
      <i class="bi bi-telegram"></i> پیام در تلگرام
    </a>
  </section>

  <footer>
    © 2025 - طراحی شده با ❤️ توسط مجید
  </footer>

  <script>
    function toggleTheme() {
      const html = document.documentElement;
      const currentTheme = html.getAttribute('data-theme');
      html.setAttribute('data-theme', currentTheme === 'dark' ? 'light' : 'dark');
    }
  </script>
</body>
</html>
