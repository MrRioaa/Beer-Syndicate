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
.contacts-wrap {
  max-width: 700px;
  margin: 0 auto 36px auto;
  background: #fcfcfd;
  border-radius: 18px;
  box-shadow: 0 2px 12px #0001;
  padding: 32px 28px 28px 28px;
  font-size: 1.15em;
}
.contacts-title {
  font-size: 1.4em;
  font-weight: 700;
  color: #145ba0;
  margin-bottom: 20px;
  display: flex;
  align-items: center;
  gap: 10px;
}
.contacts-list {
  list-style: none;
  margin: 0 0 2em 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  gap: 14px;
}
.contacts-list li {
  background: #f7faff;
  border-left: 4px solid #7dbdff;
  border-radius: 10px;
  padding: 12px 18px;
  font-size: 1.06em;
  display: flex;
  align-items: center;
  gap: 8px;
}
.contacts-link {
  color: #145ba0;
  text-decoration: none;
  font-weight: 600;
  transition: color 0.15s;
}
.contacts-link:hover {
  color: #e3b108;
  text-decoration: underline;
}
.leader-block {
  margin-top: 2em;
  padding: 16px 18px;
  background: #f8f8f8;
  border-radius: 10px;
  box-shadow: 0 1px 6px #0001;
}
.leader-title {
  font-weight: 700;
  color: #2979ff;
  margin-bottom: 0.7em;
}
.leader-contacts {
  display: flex;
  flex-direction: column;
  gap: 8px;
}
.leader-label {
  color: #888;
  font-size: 0.98em;
  margin-right: 4px;
}
</style>

<!-- Меню -->
<div class="menu-nav">
  <a href="/Beer-Syndicate/" class="menu-btn">Главная</a>
  <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
  <a href="/Beer-Syndicate/members" class="menu-btn">Состав</a>
  <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
  <a href="/Beer-Syndicate/contacts" class="menu-btn active">Контакты</a>
</div>

<!-- Контакты -->
<div class="contacts-wrap">
  <div class="contacts-title">Наши ресурсы</div>
  $1
    <li>📢 <a class="contacts-link" href="https://t.me/BeerSyndicate_aa" target="_blank">Telegram-канал гильдии</a></li>
    <li>🎮 <a class="contacts-link" href="https://discord.gg/wnCxVG2m" target="_blank">Discord сервер</a></li>
  </ul>

  <div class="leader-block">
    <div class="leader-title">Контакты лидера гильдии</div>
    <div class="leader-contacts">
      <span><span class="leader-label">Telegram:</span>
        <a class="contacts-link" href="https://t.me/Mr_NN1" target="_blank">@Mr_NN1</a>
      </span>
      <span><span class="leader-label">Discord:</span>
        <b>mrriooff</b>
      </span>
    </div>
  </div>
</div>
