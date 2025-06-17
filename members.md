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
.members-wrap {
  max-width: 700px;
  margin: 0 auto 36px auto;
  background: #fcfcfd;
  border-radius: 18px;
  box-shadow: 0 2px 12px #0001;
  padding: 32px 28px 28px 28px;
  font-size: 1.15em;
}
.members-title {
  font-size: 1.3em;
  font-weight: 700;
  color: #145ba0;
  margin-bottom: 18px;
}
.members-table {
  width: 100%;
  border-collapse: separate;
  border-spacing: 0 8px;
}
.rank-header {
  background: #e3f1ff;
  color: #2979ff;
  font-weight: 700;
  font-size: 1.07em;
  border-radius: 10px 10px 0 0;
  padding: 10px 0 10px 14px;
  border-left: 5px solid #7dbdff;
  margin-top: 20px;
}
.member-row {
  background: #f9f9f9;
  border-radius: 7px;
  box-shadow: 0 1px 4px #0001;
}
.member-cell {
  padding: 10px 18px;
  border: none;
  font-size: 1.07em;
}
.leader-badge {
  background: #ffda73;
  color: #b48b0a;
  border-radius: 7px;
  font-weight: 700;
  padding: 2px 8px;
  margin-left: 8px;
  font-size: 0.93em;
}
}
</style>

<!-- Меню -->
<div class="menu-nav">
  <a href="/Beer-Syndicate/" class="menu-btn">Главная</a>
  <a href="/Beer-Syndicate/about" class="menu-btn">О гильдии</a>
  <a href="/Beer-Syndicate/members" class="menu-btn active">Состав</a>
  <a href="/Beer-Syndicate/recruit" class="menu-btn">Как вступить</a>
  <a href="/Beer-Syndicate/contacts" class="menu-btn">Контакты</a>
</div>

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
    <tr class="member-row">
      <td class="member-cell">Офицер 1</td>
    </tr>
    <tr class="member-row">
      <td class="member-cell">Офицер 2</td>
    </tr>
    <tr class="member-row">
      <td class="member-cell">Офицер 3</td>
    </tr>
    <tr class="member-row">
      <td class="member-cell">Офицер 4</td>
    </tr>
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
