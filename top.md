<style>
/* Общие стили */
body {
  font-family: Arial, sans-serif;
  max-width: 800px;
  margin: 0 auto;
  padding: 20px;
  color: #333;
}

/* Навигационное меню */
.nav-table {
  width: 100%;
  border-collapse: collapse;
  margin-bottom: 30px;
}
.nav-table td {
  text-align: center;
  padding: 12px 5px;
  border-bottom: 2px solid #f0f0f0;
}
.nav-link {
  color: #2d2d2d;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.2s;
}
.nav-link:hover {
  color: #e3b108;
}

/* Блок топа */
.top-section {
  background: #fcfcfd;
  border-radius: 12px;
  padding: 25px;
  margin-bottom: 30px;
  box-shadow: 0 2px 10px rgba(0,0,0,0.05);
}
.section-title {
  font-size: 1.5em;
  text-align: center;
  margin-bottom: 15px;
  color: #145ba0;
}
.update-time {
  text-align: center;
  color: #888;
  margin-bottom: 20px;
  font-size: 0.95em;
}

/* Таблица топа */
.leaderboard-table {
  width: 100%;
  max-width: 500px; /* Фиксированная ширина для выравнивания */
  margin: 0 auto; /* Центрирование */
  border-collapse: collapse;
}
.leaderboard-table th {
  background: #eaf4ff;
  color: #2979ff;
  padding: 10px 15px;
  text-align: center;
  font-weight: 700;
}
.leaderboard-table td {
  padding: 10px 15px;
  text-align: center;
  border-bottom: 1px solid #e4e8ee;
}
.leaderboard-table tr:nth-child(2) td {
  background: #fff9e2;
  color: #bd890b;
  font-weight: 700;
}
.leaderboard-table tr:not(:nth-child(2)) td {
  background: #f8fafc;
}

/* Таймер и победители */
.timer {
  text-align: center;
  margin: 20px 0 10px;
  font-size: 1.05em;
}
.winners {
  text-align: center;
  color: #7a7a7a;
  margin-bottom: 15px;
}

/* Футер */
.footer {
  text-align: center;
  margin-top: 30px;
  padding-top: 15px;
  border-top: 1px solid #eee;
  color: #789;
}
.footer-links {
  margin-top: 8px;
}
.footer-links a {
  color: #145ba0;
  text-decoration: none;
  margin: 0 8px;
}
.footer-links a:hover {
  text-decoration: underline;
}

/* Адаптивность */
@media (max-width: 600px) {
  .nav-table td {
    padding: 8px 3px;
    font-size: 0.9em;
  }
  .leaderboard-table {
    max-width: 95%;
  }
}
</style>

<!-- Навигация -->
<table class="nav-table">
  <tr>
    <td><a href="/Beer-Syndicate/" class="nav-link">Главная</a></td>
    <td><a href="/Beer-Syndicate/about" class="nav-link">О гильдии</a></td>
    <td><a href="/Beer-Syndicate/members" class="nav-link">Состав</a></td>
    <td><a href="/Beer-Syndicate/recruit" class="nav-link">Как вступить</a></td>
    <td><a href="/Beer-Syndicate/contacts" class="nav-link">Контакты</a></td>
  </tr>
</table>

<!-- Блок топа -->
<div class="top-section">
  <h2 class="section-title">Топ-5 по вкладу за неделю</h2>
  <div class="update-time">Последнее обновление: 17.06.25 12:14</div>
  
  <table class="leaderboard-table">
    <tr>
      <th>Место</th>
      <th>Имя</th>
      <th>Вклад (неделя)</th>
    </tr>
    <tr>
      <td>1</td>
      <td>СаняДробовик</td>
      <td>160</td>
    </tr>
    <tr>
      <td>2</td>
      <td>Thxfordrugs</td>
      <td>80</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Ksioniks</td>
      <td>50</td>
    </tr>
    <tr>
      <td>4</td>
      <td>Солевичек</td>
      <td>30</td>
    </tr>
    <tr>
      <td>5</td>
      <td>Лолечка</td>
      <td>30</td>
    </tr>
  </table>
  
  <div class="timer">
    До сброса топа: <strong>4д 11ч 23м 32с</strong>
  </div>
  <div class="winners">
    Победители прошлой недели: ---
  </div>
</div>

<!-- Футер -->
<div class="footer">
  <div>© 2025 Beer-Syndicate</div>
  <div class="footer-links">
    <a href="/Beer-Syndicate/contacts">Контакты</a>
    <a href="https://t.me/BeerSyndicate_aa" target="_blank">Telegram-канал</a>
    <a href="https://discord.gg/wnCxVG2m" target="_blank">Discord</a>
  </div>
</div>

<!-- Скрипт таймера -->
<script>
  function updateTimer() {
    const now = new Date();
    const nextSaturday = new Date();
    const daysUntilSaturday = (6 - now.getDay() + 7) % 7;
    nextSaturday.setDate(now.getDate() + daysUntilSaturday);
    nextSaturday.setHours(23, 59, 0, 0);

    if (now.getDay() === 6 && now.getHours() < 23) {
      nextSaturday.setDate(now.getDate());
    }

    const diff = nextSaturday - now;
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
    const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));
    const seconds = Math.floor((diff % (1000 * 60)) / 1000);

    document.querySelector('.timer strong').textContent = 
      `${days}д ${hours}ч ${minutes}м ${seconds}с`;
  }
  updateTimer();
  setInterval(updateTimer, 1000);
</script>
