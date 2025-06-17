<style>
/* Стили меню (исправленные) */
.menu-nav {
  display: flex;
  justify-content: center;
  gap: 18px;
  padding: 18px 0;
  margin-bottom: 30px;
}
.menu-btn {
  color: #2d2d2d;
  font-weight: 600;
  text-decoration: none;
  padding: 10px 20px;
}

/* Основные стили */
.top-wrap {
  max-width: 600px;
  margin: 0 auto;
  padding: 25px;
}

/* Таблица с фиксированной шириной столбцов */
.top-table {
  width: 100%;
  border-collapse: collapse;
  margin: 20px auto;
  table-layout: fixed; /* Фиксированная ширина столбцов */
}
.top-table th, .top-table td {
  padding: 10px 15px;
  text-align: center;
  border: 1px solid #e4e8ee;
}
.top-table th {
  background: #eaf4ff;
  color: #2979ff;
}
.top-table tr:nth-child(1) td {
  background: #fff9e2;
}

/* Таймер и футер */
.timer-block, .winners-block {
  text-align: center;
  margin: 15px 0;
}
.footer {
  text-align: center;
  margin-top: 30px;
}
</style>

<!-- Меню -->
<div class="menu-nav">
  <a href="/" class="menu-btn">Главная</a>
  <a href="/about" class="menu-btn">О гильдии</a>
  <a href="/members" class="menu-btn">Состав</a>
  <a href="/recruit" class="menu-btn">Как вступить</a>
  <a href="/contacts" class="menu-btn">Контакты</a>
</div>

<!-- Блок топа -->
<div class="top-wrap">
  <h2>Топ-5 по вкладу за неделю</h2>
  <div class="top-update">Последнее обновление: 17.06.25 12:14</div>
  
  <table class="top-table">
    <colgroup>
      <col style="width: 20%"> <!-- Место -->
      <col style="width: 50%"> <!-- Имя -->
      <col style="width: 30%"> <!-- Вклад -->
    </colgroup>
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
      <td>Лоленка</td>
      <td>30</td>
    </tr>
  </table>
  
  <div class="timer-block">
    До сброса топа: <strong>4д 11ч 6м 33с</strong>
  </div>
  <div class="winners-block">
    Победители прошлой недели: ---
  </div>
</div>

<!-- Футер -->
<div class="footer">
  <div>© 2025 Beer-Syndicate</div>
  <div>
    <a href="/contacts">Контакты</a> | 
    <a href="https://t.me/BeerSyndicate_aa">Telegram-канал</a> | 
    <a href="https://discord.gg/wnCxVG2m">Discord</a>
  </div>
</div>

<script>
// Таймер (как в предыдущих примерах)
</script>
