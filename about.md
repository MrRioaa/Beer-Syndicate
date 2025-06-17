<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>О гильдии | Пивной Синдикат</title>
  <style>
    :root {
      --beer-bg: #2b2116;
      --beer-panel: #3b2e22;
      --beer-panel-light: #53422d;
      --beer-cream: #fff8e1;
      --beer-cream2: #ffe3a3;
      --beer-yellow: #FFDE69;
      --beer-yellow2: #FFC34A;
      --beer-orange: #FFA941;
      --beer-brown: #A87536;
      --beer-brown-dark: #6e4923;
      --beer-border: #6e4923;
      --beer-shadow: #0008;
    }
    body {
      font-family: 'Segoe UI', 'Arial', sans-serif;
      background: var(--beer-bg);
      margin: 0;
      padding: 0;
      color: var(--beer-cream);
      min-height: 100vh;
    }
    .main-wrapper {
      max-width: 980px;
      margin: 38px auto 0 auto;
      background: linear-gradient(140deg, var(--beer-panel) 88%, var(--beer-panel-light) 100%);
      border-radius: 24px;
      box-shadow: 0 8px 36px #000b, 0 1.5px 6px #ffde6930;
      padding: 32px 28px 22px 28px;
      border: 1.5px solid var(--beer-border);
      position: relative;
      display: flex;
      flex-direction: row;
      gap: 36px;
      min-height: 600px;
    }
    .menu-nav {
      display: flex;
      justify-content: center;
      align-items: center;
      gap: 22px;
      background: var(--beer-panel);
      border-radius: 18px;
      box-shadow: 0 3px 16px #000a, 0 1.5px 4px #ffde6930;
      padding: 14px 0;
      margin-bottom: 32px;
      border: 2px solid var(--beer-brown);
    }
    .menu-btn {
      background: var(--beer-cream2);
      color: var(--beer-panel);
      font-weight: 700;
      border-radius: 10px;
      padding: 10px 26px;
      text-decoration: none;
      font-size: 1.08em;
      transition: background 0.18s, box-shadow 0.18s, color 0.18s, transform 0.1s;
      box-shadow: 0 1.5px 7px #ffc34a1c;
      border: 2px solid transparent;
      outline: none;
      cursor: pointer;
      position: relative;
      top: 0;
    }
    .menu-btn:hover, .menu-btn:focus {
      background: var(--beer-yellow);
      color: var(--beer-panel);
      border-color: var(--beer-orange);
      box-shadow: 0 2.5px 18px #ffde6933;
      transform: translateY(-2px) scale(1.04);
      z-index: 2;
    }
    .menu-btn.active {
      background: linear-gradient(95deg, var(--beer-yellow) 70%, var(--beer-yellow2) 100%);
      border-color: var(--beer-orange);
      color: var(--beer-panel);
      box-shadow: 0 2.5px 13px #ffde694a;
    }
    .about-content {
      width: 700px;
      background: var(--beer-panel-light);
      border-radius: 18px;
      box-shadow: 0 2px 12px #0005;
      padding: 38px 34px 36px 34px;
      font-size: 1.13em;
      color: var(--beer-cream);
      border: 2px solid var(--beer-border);
      margin: 0 auto 0 0;
      position: relative;
    }
    .about-content h2 {
      margin-top: 0.5em;
      color: var(--beer-yellow);
      font-size: 1.38em;
      text-shadow: 0 2px 6px #0008;
    }
    .about-list {
      margin: 0.5em 0 1.5em 0;
      padding-left: 1.2em;
    }
    .about-rule-title {
      font-weight: 700;
      font-size: 1.12em;
      margin: 1.7em 0 0.3em 0;
      color: var(--beer-orange);
      text-shadow: 0 2px 6px #0005;
    }
    .rule-list {
      margin: 0.6em 0 0.7em 0;
      padding-left: 1.3em;
    }
    .rule-list li {
      margin-bottom: 0.35em;
    }
    .rule-label {
      font-weight: 600;
      color: var(--beer-yellow);
    }
    .rule-num {
      font-weight: 700;
      color: var(--beer-yellow2);
      margin-right: 7px;
    }
    hr {
      border: none;
      border-top: 2px solid var(--beer-yellow2);
      background: none;
      margin: 2em 0 1.2em 0;
      opacity: 0.3;
    }
    /* Баннер справа */
    .about-banner {
      min-width: 235px;
      max-width: 270px;
      width: 245px;
      position: static;
      background: linear-gradient(90deg,#4c381c 60%,#ffde6933 100%);
      border-radius: 14px;
      box-shadow: 0 2px 12px #000a, 0 2px 12px #ffc34a33;
      color: var(--beer-yellow2);
      font-weight: 700;
      font-size: 1.09em;
      padding: 26px 20px 20px 22px;
      display: flex;
      flex-direction: column;
      align-items: center;
      gap: 14px;
      text-align: center;
      transition: box-shadow 0.15s, background 0.15s;
      border: 2px solid var(--beer-brown);
      z-index: 3;
      margin-left: 0;
      margin-top: 12px;
      height: fit-content;
      align-self: flex-start;
    }
    .about-banner a {
      color: var(--beer-yellow);
      text-decoration: none;
      font-weight: 700;
      transition: color 0.18s;
      border-bottom: 2px dashed var(--beer-orange);
      padding-bottom: 1px;
    }
    .about-banner a:hover {
      color: var(--beer-orange);
      border-bottom: 2px solid var(--beer-orange);
    }
    @media (max-width: 1200px) {
      .main-wrapper {
        flex-direction: column;
        gap: 0;
        min-height: unset;
      }
      .about-content, .about-banner {
        max-width: 98vw;
        width: 99vw;
      }
      .about-banner { margin: 22px auto 10px auto; justify-content: center; }
    }
    @media (max-width: 900px) {
      .main-wrapper { padding: 8vw 0 5vw 0; }
      .about-content { padding: 6vw 2vw; }
      .about-banner { font-size:1em; padding:12px 10px;}
    }
    @media (max-width: 700px) {
      .footer-content { flex-direction: column; gap: 8px; }
    }
    footer.footer-main {
      width: 100vw;
      margin-top: 40px;
      background: linear-gradient(90deg, #38280f 40%, #523813 100%);
      border-radius: 18px 18px 0 0;
      box-shadow: 0 -1px 13px #000a;
      padding: 22px 0 14px 0;
      font-size: 1.12em;
      color: var(--beer-yellow2);
      display: flex;
      justify-content: center;
      font-weight: 600;
      border-top: 3px solid var(--beer-yellow2);
      position: relative;
      left: 50%;
      right: 50%;
      margin-left: -50vw;
      margin-right: -50vw;
    }
    .footer-content {
      max-width: 850px;
      margin: 0 auto;
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      align-items: center;
      width: 96%;
    }
    .footer-links a {
      color: var(--beer-yellow);
      text-decoration: none;
      margin: 0 4px;
      font-weight: 600;
      transition: color 0.13s;
    }
    .footer-links a:hover {
      color: var(--beer-orange);
      text-decoration: underline;
    }
    .footer-links span {
      margin: 0 3px;
      color: var(--beer-brown-dark);
    }
  </style>
</head>
<body>
  <nav class="menu-nav">
    <a href="/Beer-Syndicate/" class="menu-btn">Главная</a>
    <a href="/Beer-Syndicate/about" class="menu-btn active">О гильдии</a>
    <a href="/Beer-Syndicate/members" class="menu-btn">Состав</a>
    <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
    <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
  </nav>
  <div class="main-wrapper">
    <div class="about-content">
      <h2>Добро пожаловать в «Пивной Синдикат»!</h2>
      <p>Наша гильдия создана для комфортной и совместной игры:</p>
      <ul class="about-list">
        <li>Свобода выбора</li>
        <li>Занимайся тем, что нравится — <b>PVP</b>, <b>PVE</b>, фарм, крафт или просто общение внутри Ги</li>
      </ul>
      <p>Единственное, что мы требуем: <b>поддерживай товарищей, участвуй в жизни гильдии и делись опытом</b>.<br>
      Заходи, комфортно устраивайся и отдыхай — <b>«Пивной Синдикат» рад каждому!</b></p>
      <hr>
      <h2>📜 Правила «Пивного Синдиката»</h2>
      <div class="about-rule-title"><span class="rule-num">1️⃣</span> Основные принципы</div>
      <ul class="rule-list">
        <li><span class="rule-label">Уважение —</span> токсичность, оскорбления, дискриминации или буллинг только в дружеском формате. Мы не ханжи, но и не быдло ебанное :3</li>
        <li><span class="rule-label">Совместная игра —</span> помогаем друг другу, делимся ресурсами (по возможности) и знаниями.</li>
        <li><span class="rule-label">Активность —</span> даже если вы заняты IRL, старайтесь иногда заходить в Discord/игру, чтобы гильдия не казалась «мертвой».</li>
      </ul>
      <div class="about-rule-title"><span class="rule-num">2️⃣</span> В игре</div>
      <ul class="rule-list">
        <li><span class="rule-label">Гильд-ивенты —</span> участие в совместных мероприятиях приветствуется, но не строго обязательно.</li>
        <li><span class="rule-label">Честность —</span> никакого скама, краж из общего склада или обмана согильдийцев.</li>
        <li><span class="rule-label">Конфликты —</span> решаем мирно через офицеров/лидера, а не переходим на личности.</li>
      </ul>
      <div class="about-rule-title"><span class="rule-num">3️⃣</span> В Discord</div>
      <p><b>Голосовые каналы:</b></p>
      <ul class="rule-list">
        <li>Гостиная — Общение с новобранцами</li>
        <li>Таверна — Общение на любые темы</li>
        <li>Голосовой 1,2 — Общение по игре</li>
        <li>КП 1,2 — Личные чаты</li>
      </ul>
      <p><b>Текстовые чаты:</b></p>
      <ul class="rule-list">
        <li>Таверна — Общение на любые темы</li>
        <li>КП 1,2 — Личные чаты</li>
        <li>Общее — Спам помойка</li>
      </ul>
      <p>
        <b style="color:#e53935;">NSFW-контент запрещён.</b>
      </p>
    </div>
    <!-- Баннер справа -->
    <aside class="about-banner">
      <span style="font-size:1.17em;">🏆 Текущий <a href="/Beer-Syndicate/top">топ-5 вкладчиков недели</a></span>
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
