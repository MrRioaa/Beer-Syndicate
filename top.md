<style>
.menu-nav {
  display: flex; 
  justify-content: center; 
  gap: 18px; 
  background: #f7f7f7; 
  padding: 18px 0 16px 0; 
  border-radius: 0 0 14px 14px; 
  box-shadow: 0 2px 8px #0001;
  margin-bottom: 40px;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
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
.top-wrap {
  max-width: 600px;
  margin: 0 auto 48px auto;
  background: #fcfcfd;
  border-radius: 18px;
  box-shadow: 0 2px 12px #0001;
  padding: 32px 28px 28px 28px;
  font-size: 1.13em;
}
.top-title {
  font-size: 1.5em;
  font-weight: 700;
  color: #145ba0;
  margin-bottom: 8px;
  text-align: center;
}
.top-update {
  color: #888;
  font-size: 0.97em;
  margin-bottom: 18px;
  text-align: left;
}
.top-table {
  width: 100%;
  border-collapse: collapse;
  margin-bottom: 18px;
}
.top-table th {
  background: #eaf4ff;
  color: #2979ff;
  font-weight: 700;
  font-size: 1em;
  padding: 8px 0;
  border-radius: 6px 6px 0 0;
}
.top-table th,
.top-table td {
  text-align: center;
  border: 1px solid #e4e8ee;
  padding: 8px 12px;
}
.top-table tr:nth-child(2) td {
  background: #fff9e2;
  color: #bd890b;
  font-weight: 700;
}
.top-table tr:not(:nth-child(2)) td {
  background: #f8fafc;
}
.top-table td {
  font-size: 1.05em;
}
.top-winners {
  margin-top: 14px;
  font-size: 1.02em;
  color: #7a7a7a;
}
@media (max-width: 800px) {
  .menu-nav,
  .top-wrap {
    max-width: 97vw;
  }
  .top-title { font-size: 1.13em; }
}
.footer-main {
  width: 100%;
  margin-top: 36px;
  background: #f7f7f7;
  border-radius: 18px 18px 0 0;
  box-shadow: 0 -1px 6px #0001;
  padding: 18px 0 14px 0;
  font-size: 1.04em;
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

<!-- Меню -->
<div class="menu-nav">
  <a href="/Beer-Syndicate/" class="menu-btn">Главная</a>
  <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
  <a href="/Beer-Syndicate/members" class="menu-btn">Состав</a>
  <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
  <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
</div>

<!-- Блок топа -->
<div class="top-wrap">
  <div class="top-title">Топ-5 по вкладу за неделю</div>
  <div class="top-update">Последнее обновление: 17.06.25 6:00</div>
  <table class="top-table">
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
      <td>Ksioniks</td>
      <td>50</td>
    </tr>
    <tr>
      <td>3</td>
      <td>Thxfordrugs</td>
      <td>80</td>
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
  <div class="top-winners">
    Победители прошлой недели: ----------
  </div>
</div>

<!-- Футер -->
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

<!-- Скрипт таймера -->
<script>
  function updateTimer() {
    const now = new Date();
    const updateDate = document.querySelector('.top-update');
    
    // Автоматическое обновление даты
    const formattedDate = now.toLocaleString('ru-RU', {
      day: '2-digit',
      month: '2-digit',
      year: '2-digit',
      hour: '2-digit',
      minute: '2-digit'
    }).replace(/,/, '');
    
    updateDate.textContent = `Последнее обновление: ${formattedDate}`;

    // Вычисляем время до следующей субботы 23:59
    const nextSaturday = new Date();
    const daysUntilSaturday = (6 - now.getDay() + 7) % 7; // 6 = суббота
    nextSaturday.setDate(now.getDate() + daysUntilSaturday);
    nextSaturday.setHours(23, 59, 0, 0);

    // Если сегодня суббота и время ещё не 23:59
    if (now.getDay() === 6 && now.getHours() < 23) {
      nextSaturday.setDate(now.getDate());
    }

    const diff = nextSaturday - now;
    const days = Math.floor(diff / (1000 * 60 * 60 * 24));
    const hours = Math.floor((diff % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
    const minutes = Math.floor((diff % (1000 * 60 * 60)) / (1000 * 60));

    // Обновляем таймер
    const timerElement = document.querySelector('.top-winners');
    if (diff > 0) {
      timerElement.innerHTML = `До сброса топа: <b>${days}д ${hours}ч ${minutes}м</b> | Победители прошлой недели: ----------`;
    } else {
      timerElement.innerHTML = `Топ сброшен! Обновите данные. | Победители прошлой недели: ----------`;
    }
  }

  // Запускаем таймер сразу и обновляем каждую минуту
  updateTimer();
  setInterval(updateTimer, 60000);
</script>
