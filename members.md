with open("/mnt/data/members_darkbeer_v3.html", "w", encoding="utf-8") as f:
    f.write("""<!DOCTYPE html>
<html lang="ru">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width,initial-scale=1">
  <title>Состав | Пивной Синдикат</title>
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
      --beer-rank-header-bg: #433117;
      --beer-rank-header-text: #d9c08a;
    }
    body {
      font-family: 'Segoe UI', 'Arial', sans-serif;
      background: var(--beer-bg);
      margin: 0;
      padding: 0;
      color: var(--beer-cream);
      min-height: 100vh;
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
      max-width: 980px;
      margin-left: auto;
      margin-right: auto;
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
    .members-main {
      display: flex;
      align-items: flex-start;
      gap: 36px;
      max-width: 980px;
      margin: 0 auto 36px auto;
      min-height: 540px;
    }
    .members-wrap {
      max-width: 700px;
      flex: 1 1 0px;
      background: var(--beer-panel-light);
      border-radius: 18px;
      box-shadow: 0 2px 12px #0005;
      padding: 38px 34px 32px 34px;
      font-size: 1.15em;
      color: var(--beer-cream);
      border: 2px solid var(--beer-border);
    }
    .members-title {
      font-size: 1.3em;
      font-weight: 700;
      color: var(--beer-yellow);
      margin-bottom: 18px;
      text-shadow: 0 2px 6px #0008;
    }
    .members-table {
      width: 100%;
      border-collapse: separate;
      border-spacing: 0 8px;
    }
    .rank-header {
      background: var(--beer-rank-header-bg);
      color: var(--beer-rank-header-text);
      font-weight: 700;
      font-size: 1.07em;
      border-radius: 10px 10px 0 0;
      padding: 10px 0 10px 14px;
      border-left: 5px solid var(--beer-brown-dark);
      margin-top: 20px;
      box-shadow: 0 1.5px 5px #0002;
      letter-spacing: 0.04em;
      text-shadow: 0 1px 8px #000a;
    }
    .member-row {
      background: var(--beer-cream2);
      border-radius: 7px;
      box-shadow: 0 1px 4px #0001;
    }
    .member-cell {
      padding: 10px 18px;
      border: none;
      font-size: 1.07em;
      color: var(--beer-panel);
      font-weight: 600;
    }
    .leader-badge {
      background: var(--beer-yellow);
      color: #b48b0a;
      border-radius: 7px;
      font-weight: 700;
      padding: 2px 8px;
      margin-left: 8px;
      font-size: 0.93em;
    }
    .banner-side {
      min-width: 225px;
      max-width: 260px;
      margin-top: 12px;
      background: linear-gradient(120deg,#4c381c 60%,#ffde6933 100%);
      border-radius: 15px;
      box-shadow: 0 2px 12px #000a, 0 2px 12px #ffc34a33;
      padding: 32px 18px 22px 18px;
      display: flex;
      flex-direction: column;
      align-items: center;
      border: 2px solid var(--beer-brown);
      color: var(--beer-yellow2);
      font-size: 1.1em;
      font-weight: 700;
      height: fit-content;
    }
    .banner-title {
      color: var(--beer-yellow);
      font-weight: 700;
      font-size: 1.14em;
      margin-bottom: 6px;
    }
    .banner-txt {
      font-size: 1em;
      color: var(--beer-cream2);
      margin-bottom: 18px;
      text-align: center;
    }
    .banner-btn {
      display: inline-flex; align-items: center; gap: 7px;
      background: linear-gradient(90deg,var(--beer-yellow) 60%,var(--beer-yellow2) 100%);
      border-radius: 8px;
      box-shadow: 0 2px 8px #ffc34a60;
      color: var(--beer-panel);
      font-weight: 700;
      padding: 10px 22px;
      font-size: 1.06em;
      text-decoration: none;
      border: 2px solid var(--beer-yellow);
      transition: box-shadow 0.15s, background 0.15s, color 0.13s, border 0.13s;
    }
    .banner-btn:hover {
      background: var(--beer-yellow2);
      color: var(--beer-orange);
      border-color: var(--beer-orange);
      box-shadow: 0 4px 14px #ffc34a80;
    }
    @media (max-width: 1000px) {
      .members-main { flex-direction: column; gap: 24px; }
      .banner-side { max-width: 99vw; min-width: unset; width: 98vw; margin-left: 0; }
      .members-wrap { max-width: 99vw; }
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
    @media (max-width: 700px) {
      .footer-content { flex-direction: column; gap: 8px; }
    }
  </style>
</head>
<body>
  <nav class="menu-nav">
    <a href="/Beer-Syndicate/" class="menu-btn">Главная</a>
    <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
    <a href="/Beer-Syndicate/members" class="menu-btn active">Состав</a>
    <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
    <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
  </nav>
  <div class="members-main">
    <div class="members-wrap">
      <div class="members-title">Состав гильдии</div>
      <!-- Лидер -->
      <div class="rank-header">Пивной Барон (Лидер гильдии)</div>
      <table class="members-table">
        <tr class="member-row">
          <td class="member-cell">СаняДробовик <span class="leader-badge">Лидер</span></td>
        </tr>
      </table>
      <!-- Офицеры -->
      <div class="rank-header" style="margin-top: 18px;">Пивозавры (Офицеры)</div>
      <table class="members-table">
        <tr class="member-row"><td class="member-cell">Офицер 1</td></tr>
        <tr class="member-row"><td class="member-cell">Офицер 2</td></tr>
        <tr class="member-row"><td class="member-cell">Офицер 3</td></tr>
        <tr class="member-row"><td class="member-cell">Офицер 4</td></tr>
      </table>
      <!-- Подпивасы -->
      <div class="rank-header" style="margin-top: 18px;">Подпивасы</div>
      <table class="members-table">
        <tr class="member-row"><td class="member-cell">Подпивас 1</td></tr>
        <tr class="member-row"><td class="member-cell">Подпивас 2</td></tr>
      </table>
      <!-- Алкаши -->
      <div class="rank-header" style="margin-top: 18px;">Алкаши</div>
      <table class="members-table">
        <tr class="member-row"><td class="member-cell">Алкаш 1</td></tr>
        <tr class="member-row"><td class="member-cell">Алкаш 2</td></tr>
      </table>
      <!-- Пивусики -->
      <div class="rank-header" style="margin-top: 18px;">Пивусики</div>
      <table class="members-table">
        <tr class="member-row"><td class="member-cell">Пивусик 1</td></tr>
        <tr class="member-row"><td class="member-cell">Пивусик 2</td></tr>
      </table>
    </div>
    <div class="banner-side">
      <div class="banner-title">🏆 Текущий топ-5 по вкладу</div>
      <div class="banner-txt">
        Узнай, кто сейчас лидирует по вкладу в гильдию и кто получит награды на этой неделе!
      </div>
      <a href="/Beer-Syndicate/top" class="banner-btn">
        Перейти к топу недели →
      </a>
    </div>
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
""")
