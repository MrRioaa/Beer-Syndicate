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
.news-list {
  display: flex;
  flex-direction: column;
  gap: 24px;
  margin-top: 24px;
  max-width: 700px;
  margin-left: auto;
  margin-right: auto;
}
.news-card {
  background: #f9f9f9;
  border-left: 5px solid #ffda73;
  border-radius: 10px;
  box-shadow: 0 2px 8px #0001;
  padding: 18px 20px;
}
.news-card.blue {
  border-left: 5px solid #7dbdff;
}
.news-title {
  font-weight: 700;
  font-size: 1.1em;
  color: #145ba0;
}
@media (max-width: 800px) {
  .menu-nav,
  .news-list {
    max-width: 97vw;
  }
}
</style>

<!-- Меню -->
<div class="menu-nav">
  <a href="/Beer-Syndicate/" class="menu-btn active">Главная</a>
  <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
  <a href="/Beer-Syndicate/members" class="menu-btn">Состав</a>
  <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
  <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
</div>

<h1 style="text-align:center; font-weight: bold; white-space:nowrap;">
Добро пожаловать на сайт гильдии Пивной Синдикат ArcheAge!
</h1>

<div style="text-align:center; margin-bottom: 18px;">
  Наша гильдия создана для комфортной и совместной игры!
</div>

---

## 📰 Новости гильдии

<div class="news-list">

  <!-- Новость 1 -->
  <div class="news-card">
    <div class="news-title">17 июня 2025 — Открытие сайта гильдии!</div>
    <div style="margin-top: 4px;">
      Запущен официальный сайт нашей гильдии. Здесь будут публиковаться все актуальные новости, анонсы и события.
    </div>
  </div>

  <!-- Новость 2 -->
  <div class="news-card blue">
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
    </div>
  </div>

</div>
