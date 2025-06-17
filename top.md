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
  margin: 40px auto 0 auto;
  background: #fcfcfd;
  border-radius: 18px;
  box-shadow: 0 2px 12px #0001;
  padding: 32px 28px 28px 28px;
  font-size: 1.13em;
  position: relative;
}
.top-title {
  font-size: 1.5em;
  font-weight: 700;
  color: #145ba0;
  margin-bottom: 12px;
  text-align: center;
}
.top-update {
  color: #888;
  font-size: 0.97em;
  margin-bottom: 8px;
  text-align: left;
  margin-left: 2px;
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
  color: #222;
  font-weight: 400;
}
.top-table td {
  font-size: 1.05em;
}
.top-winners {
  margin-top: 14px;
  font-size: 1.02em;
  color: #7a7a7a;
  text-align: left;
  margin-left: 2px;
}
@media (max-width: 800px) {
  .menu-nav,
  .top-wrap {
    max-width: 97vw;
  }
  .top-title { font-size: 1.13em; }
}
</style>

<!-- Меню -->
<div class="menu-nav">
  <a href="/Beer-Syndicate/" class="menu-btn">Главная</a>
  <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
  <a href="/Beer-Syndicate/members" class="menu-btn">Состав</a>
  <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
  <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
  <a href="/Beer-Syndicate/top" class="menu-btn active">Топ-5 недели</a>
</div>

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
      <td>Санядробовик</td>
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
    Победители 1 недели: ----------
  </div>
</div>
