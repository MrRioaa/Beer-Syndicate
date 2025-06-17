<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8">
  <title>Beer-Syndicate | ArcheAge</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <style>
    body {
      margin: 0;
      background: linear-gradient(130deg, #e3f1ff 0%, #f4f6fa 85%, #fff8e2 100%);
      font-family: 'Segoe UI', 'Arial', sans-serif;
      color: #203040;
      min-height: 100vh;
    }
    .menu-nav {
      display: flex;
      justify-content: center;
      gap: 16px;
      background: transparent;
      padding: 0;
      margin-bottom: 38px;
      border-bottom: 2px solid #e3f1ff;
      box-shadow: none;
    }
    .menu-btn {
      background: none;
      color: #2373c4;
      font-weight: 600;
      border-radius: 6px 6px 0 0;
      padding: 11px 24px 8px 24px;
      text-decoration: none;
      border: none;
      box-shadow: none;
      font-size: 1em;
      transition: background 0.14s, color 0.13s;
    }
    .menu-btn:hover, .menu-btn.active {
      background: #e3f1ff;
      color: #145ba0;
    }
    .main-content {
      display: flex;
      justify-content: center;
      align-items: flex-start;
      gap: 32px;
      max-width: 1060px;
      margin: 0 auto 0 auto;
      padding: 0 10px;
    }
    .news-list {
      display: flex;
      flex-direction: column;
      gap: 21px;
      margin-top: 22px;
      max-width: 710px;
      min-width: 340px;
      flex: 2 2 0;
    }
    .news-card {
      background: #fff;
      border-left: 5px solid #7dbdff;
      border-radius: 11px;
      box-shadow: 0 2px 7px #d0e7ff45;
      padding: 17px 22px 16px 22px;
      font-size: 1.08em;
    }
    .news-title {
      font-weight: 700;
      font-size: 1.14em;
      color: #145ba0;
      margin-bottom: 7px;
    }
    .side-banner {
      background: linear-gradient(145deg,#eaf4ff 90%,#e6f7ff 100%);
      border-radius: 14px;
      box-shadow: 0 2px 8px #7dbdff22;
      padding: 18px 14px 14px 14px;
      max-width: 270px;
      min-width: 180px;
      color: #1974bb;
      margin-top: 0;
      display: flex;
      flex-direction: column;
      align-items: center;
      font-size: 1em;
    }
    .side-banner .banner-title {
      font-size: 1.12em;
      margin-bottom: 7px;
      color: #15598c;
      font-weight: 700;
    }
    .side-banner a {
      background: #ffedb3;
      color: #c1970c;
      padding: 7px 14px;
      font-size: 1em;
      border-radius: 7px;
      margin-top: 8px;
      font-weight: 600;
      text-decoration: none;
      box-shadow: none;
      border: 1px solid #ffe7a3;
      transition: background 0.14s, color 0.13s;
    }
    .side-banner a:hover {
      background: #ffe08a;
      color: #856400;
    }
    h1 {
      text-align: center;
      font-weight: bold;
      margin: 35px 0 8px 0;
      color: #2373c4;
      font-size: 2em;
      letter-spacing: 0.01em;
    }
    .subtitle-main {
      text-align: center;
      margin-bottom: 17px;
      color: #4e708a;
      font-size: 1.12em;
    }
    .footer-main {
      width: 100%;
      background: #f7f7fa;
      border-top: 1.5px solid #e3f1ff;
      border-radius: 0;
      box-shadow: none;
      margin-top: 46px;
      font-size: 1em;
      color: #789;
      display: flex;
      justify-content: center;
      padding: 15px 0 12px 0;
    }
    .footer-content {
      max-width: 900px;
      width: 98%;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      gap: 7px;
    }
    .footer-links a {
      color: #145ba0;
      text-decoration: none;
      margin: 0 4px;
      font-weight: 600;
      transition: color 0.13s;
    }
    .footer-links a:hover {
      color: #e3b108;
      text-decoration: underline;
    }
    .footer-links span {
      margin: 0 3px;
      color: #aaa;
    }
    @media (max-width: 1050px) {
      .main-content { flex-direction: column; align-items: stretch; gap: 15px; }
      .side-banner { margin-top: 0; max-width: 97vw; min-width: 0; }
    }
    @media (max-width: 800px) {
      .menu-nav, .news-list { max-width: 97vw; }
      .news-list { min-width: 0; }
    }
    @media (max-width: 700px) {
      .footer-content { flex-direction: column; gap: 8px; }
      .main-content { gap: 6vw; }
    }
  </style>
</head>
<body>
  <nav class="menu-nav">
    <a href="/Beer-Syndicate/" class="menu-btn active">Главная</a>
    <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
    <a href="/Beer-Syndicate/members" class="menu-btn">Состав</a>
    <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
    <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
  </nav>
  <h1>Добро пожаловать на сайт гильдии Пивной Синдикат ArcheAge!</h1>
  <div class="subtitle-main">
    Наша гильдия создана для комфортной и совместной игры!
  </div>
  <div class="main-content">
    <section class="news-list">
      <article class="news-card">
        <div class="news-title">17 июня 2025 — Открытие сайта гильдии!</div>
        <div style="margin-top: 4px;">
          Запущен официальный сайт нашей гильдии. Здесь будут публиковаться все актуальные новости, анонсы и события.
        </div>
      </article>
      <article class="news-card">
        <div class="news-title">17 июня 2025 — Еженедельные выплаты за вклад в гильдию!</div>
        <div style="margin-top: 4px; font-size: 1.07em;">
          <b>💰 Еженедельные выплаты за вклад в гильдию</b><br>
          <b>Суть:</b> 1 очко вклада = 1 голда.<br>
          Топ-5 участников с наибольшим вкладом получают выплаты, <b>но только если набрали минимум 160 очков за неделю.</b>
          <br><br>
          <b style="color:#2979ff;">◆ Пример:</b>
          <ul style="margin-left:1.1em;">
            <li>Если у тебя <b>250 очков</b> и ты в топ-5 → получишь <b>250 голды</b>.</li>
            <li>Если у тебя <b>150 очков</b> и ты в топ-5 → не попадаешь в выплаты (мало вклада).</li>
            <li>Если у тебя <b>400 очков</b>, но ты 6-й в списке → не попадаешь в топ-5.</li>
          </ul>
          <span style="color:#e53935; font-weight:600;">📅 Считаем каждую субботу, выплаты — в воскресенье.</span>
          <div style="margin-top:18px;">
            <a href="top" style="
              display: inline-flex; align-items: center; gap: 7px;
              background: #ffe99a;
              border-radius: 7px;
              color: #a0830b;
              font-weight: 600;
              padding: 7px 14px;
              font-size: 1em;
              text-decoration: none;
              border: 1px solid #ffe7a3;
              margin-top: 0;
            ">
              Смотреть текущий топ-5 недели
            </a>
          </div>
        </div>
      </article>
    </section>
    <aside class="side-banner">
      <div class="banner-title">🏅 Топ-5 недели</div>
      <div style="font-size:0.98em; color:#267cff;">
        Кто лучший вкладчик?<br>
        Переходи к&nbsp;текущему рейтингу участников<br>— получи свою награду!
      </div>
      <a href="top">Перейти к ТОПу</a>
    </aside>
  </div>
  <footer class="footer-main">
    <div class="footer-content">
      <span>© 2025 Beer-Syndicate</span>
      <span class="footer-links">
        <a href="/Beer-Syndicate/contacts">Контакты</a>
        <span>|</span>
        <a href="https://t.me/BeerSyndicate_aa" target="_blank">Telegram-канал</a>
        <span>|</span>
        <a href="https://discord.gg/wnCxVG2m" target="_blank">Discord</a>
      </span>
    </div>
  </footer>
</body>
</html>
