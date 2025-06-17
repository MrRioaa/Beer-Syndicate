<style>
.menu-nav {
  display: flex; 
  justify-content: center; 
  gap: 18px; 
  background: #f7f7f7; 
  padding: 18px 0 16px 0; 
  border-radius: 0 0 14px 14px; 
  box-shadow: 0 2px 8px #0001;
}
.menu-btn {
  background: #fff;
  color: #2d2d2d;
  font-weight: 600;
  border-radius: 8px;
  padding: 10px 26px;
  text-decoration: none;
  transition: background 0.18s, box-shadow 0.18s;
  box-shadow: 0 2px 6px #0002;
  border: 1px solid #ececec;
  display: inline-block;
}
.menu-btn:hover, .menu-btn:focus {
  background: #ffda73;
  border-color: #f3c143;
  outline: none;
}
.menu-btn.active {
  background: #ffda73;
  border-color: #f3c143;
}
</style>

<div class="menu-nav">
  <a href="index.md" class="menu-btn active">Главная</a>
  <a href="about.md" class="menu-btn">О гильдии</a>
  <a href="members.md" class="menu-btn">Состав</a>
  <a href="recruit.md" class="menu-btn">Как вступить</a>
  <a href="contacts.md" class="menu-btn">Контакты</a>
</div>
