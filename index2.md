<!doctype html>
<html lang="ru">
<head>
  <meta charset="utf-8">
  <title>Пивной Синдикат | ArcheAge Guild</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <meta name="description" content="Официальный сайт гильдии Пивной Синдикат в ArcheAge. Новости, правила, топ-5 вкладчиков, контакты.">
  <link rel="icon" href="https://archeage.ru/static/aa.mail.ru/img/main/favicon.ico" type="image/x-icon">
  <style>
    body {
      margin: 0;
      background: linear-gradient(130deg, #e3f1ff 0%, #f4f6fa 80%, #fff8e2 100%);
      font-family: 'Segoe UI', 'Arial', sans-serif;
      color: #203040;
      min-height: 100vh;
    }
    /* Меню */
    .menu-nav {
      display: flex;
      justify-content: center;
      gap: 18px;
      background: #f7f7f7;
      padding: 18px 0 16px 0;
      border-radius: 0 0 14px 14px;
      box-shadow: 0 2px 8px #0001;
      margin-bottom: 40px;
      max-width: 760px;
      margin-left: auto;
      margin-right: auto;
      z-index: 10;
      position: relative;
    }
    .menu-btn {
      background: #fff;
      color: #2d2d2d;
      font-weight: 600;
      border-radius: 8px;
      padding: 10px 26px;
      text-decoration: none;
      transition: background 0.18s, box-shadow 0.18s, color 0.18s;
      box-shadow: 0 2px 6px #0002;
      border: 1px solid #ececec;
      display: inline-block;
    }
    .menu-btn:hover, .menu-btn:focus {
      background: #ffda73;
      border-color: #f3c143;
      color: #222;
      outline: none;
    }
    .menu-btn.active {
      background: #e3f1ff;
      border-color: #7dbdff;
      color: #145ba0;
    }

    /* Основной контент */
    .main-content {
      display: flex;
      justify-content: center;
      align-items: flex-start;
      gap: 36px;
      max-width: 1120px;
      margin: 0 auto 0 auto;
      padding: 0 10px;
    }
    .news-list {
      display: flex;
      flex-direction: column;
      gap: 24px;
      margin-top: 24px;
      max-width: 720px;
      min-width: 340px;
      flex: 2 2 0;
    }
    .news-card {
      background: #fff;
      border-left: 6px solid #ffda73;
      border-radius: 12px;
      box-shadow: 0 4px 16px #d0e7ff45;
      padding: 18px 22px;
      font-size: 1.09em;
    }
    .news-card.blue {
      border-left: 6px solid #7dbdff;
    }
    .news-title {
      font-weight: 700;
      font-size: 1.18em;
      color: #145ba0;
      margin-bottom: 7px;
    }

    /* Баннер */
    .side-banner {
      flex: 1 1 260px;
      max-width: 295px;
      min-width: 222px;
      background: linear-gradient(150deg, #e3f1ff 80%, #fff0c0 100%);
      border-radius: 18px;
      box-shadow: 0 4px 16px #7dbdff22;
      padding: 28px 20px 20px 20px;
      margin-top: 44px;
      text-align: center;
      font-weight: 600;
      color: #15598c;
      font-size: 1.07em;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 16px;
    }
    .side-banner a {
      background: #ffda73;
      color: #145ba0;
      font-weight: 700;
      border-radius: 8px;
      padding: 8px 20px;
      box-shadow: 0 2px 7px #ffe08a45;
      text-decoration: none;
      font-size: 1.08em;
      transition: background 0.13s, color 0.13s;
      margin-top: 7px;
    }
    .side-banner a:hover {
      background: #ffe99a;
      color: #bd890b;
    }
    @media (max-width: 1050px) {
      .main-content { flex-direction: column; align-items: stretch; gap: 18px; }
      .side-banner { margin-top: 0; max-width: 99vw; min-width: 0; }
    }
    @media (max-width: 800px) {
      .menu-nav, .news-list { max-width: 97vw; }
      .news-list { min-width: 0; }
    }

    /* H1 и подпись */
    h1 {
      text-align: center;
      font-weight: bold;
      white-space:nowrap;
      margin: 36px 0 10px 0;
      color: #125ca8;
      text-shadow: 0 2px 12px #e3f1ff;
      font-size: 2.1em;
    }
    .subtitle-main {
      text-align: center;
      margin-bottom: 18px;
      color: #4e708a;
      font-size: 1.14em;
    }

    /* Подвал */
    .footer-main {
      width: 100%;
      margin-top: 42px;
      background: #f7f7f7;
      border-radius: 18px 18px 0 0;
      box-shadow: 0 -1px 6px #0001;
      padding: 18px 0 14px 0;
      font-size: 1.07em;
      color: #789;
      display: flex;
      justify-content: center;
    }
    .footer-content {
      max-width: 800px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      width: 96%;
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
    @media (max-width: 700px) {
      .footer-content { flex-direction: column; gap: 8px; }
    }
  </style>
</head>
<body>
  <!-- Меню -->
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

  <!-- Две колонки: новости + баннер -->
  <div class="main-content">
    <!-- Новости -->
    <section class="news-list">
      <!-- Новость 1 -->
      <article class="news-card">
        <div class="news-title">17 июня 2025 — Открытие сайта гильдии!</div>
        <div style="margin-top: 4px;">
          Запущен официальный сайт нашей гильдии. Здесь будут публиковаться все актуальные новости, анонсы и события.
        </div>
      </article>

      <!-- Новость 2 -->
      <article class="news-card blue">
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
          <!-- Кнопка для перехода к топу -->
          <div style="margin-top:18px;">
            <a href="top" style="
              display: inline-flex; align-items: center; gap: 8px;
              background: linear-gradient(90deg,#ffe99a 60%,#ffda73 100%);
              border-radius: 8px;
              box-shadow: 0 2px 8px #ffe08a60;
              color: #bd890b;
              font-weight: 700;
              padding: 8px 18px;
              font-size: 1.07em;
              text-decoration: none;
              transition: box-shadow 0.15s, background 0.15s;">
              🏆 Смотреть текущий топ-5 недели
            </a>
          </div>
        </div>
      </article>
    </section>
    <!-- Баннер справа -->
    <aside class="side-banner">
      <span style="font-size:1.23em;">🏅 <b>Топ-5 недели</b></span>
      <div style="font-size:0.98em; color:#267cff;">
        <b>Кто лучший вкладчик?</b><br>
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
