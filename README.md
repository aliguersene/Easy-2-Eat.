<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<title>Easy 2 Eat - الصفحة الرئيسية</title>
<link rel="shortcut icon" href="image.png" type="image/x-icon" />

<style>
@import url('https://fonts.googleapis.com/css2?family=Cairo:wght@500;700&display=swap');

* {
  box-sizing: border-box;
}

body {
  margin: 0;
  font-family: 'Cairo', sans-serif;
  background: url('3398.png') no-repeat center center fixed;
  background-size: cover;
  color: #fff;
  overflow-x: hidden;
}

/* ====== Header ====== */
header {
  background: rgba(0, 0, 0, 0.75);
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 16px 40px;
  position: sticky;
  top: 0;
  z-index: 1000;
}

.logo {
  font-size: 26px;
  font-weight: bold;
  color: #ffb400;
}

nav {
  display: flex;
  align-items: center;
  gap: 22px;
}

nav a, nav button {
  text-decoration: none;
  color: #fff;
  background: none;
  border: none;
  font-size: 18px;
  cursor: pointer;
  transition: 0.3s;
}

nav a:hover, nav button:hover {
  color: #ffb400;
}

#helpBtn {
  border: 2px solid #ffb400;
  padding: 6px 16px;
  border-radius: 25px;
  font-weight: bold;
}

/* ====== Help Box ====== */
#helpBox {
  position: fixed;
  top: 90px;
  right: 20px;
  background: rgba(0,0,0,0.9);
  border: 2px solid #ffb400;
  border-radius: 15px;
  padding: 20px;
  width: 260px;
  display: none;
  z-index: 9999;
}

/* ====== Main Section ====== */
.main {
  text-align: center;
  margin: 140px auto 120px;
  background: rgba(0, 0, 0, 0.6);
  padding: 70px;
  border-radius: 25px;
  width: 70%;
}

.main h1 {
  font-size: 56px;
  color: #ffb400;
}

.main p {
  font-size: 22px;
}

.main button {
  background-color: #ffb400;
  color: black;
  border: none;
  padding: 16px 50px;
  font-size: 20px;
  border-radius: 40px;
  cursor: pointer;
  font-weight: bold;
}

/* ====== Footer ====== */
footer {
  text-align: center;
  padding: 15px;
  background: rgba(0,0,0,0.85);
  font-size: 14px;
  position: fixed;
  bottom: 0;
  width: 100%;
}

/* ====== Mobile Responsive ====== */
@media (max-width: 768px) {

  header {
    padding: 14px;
    flex-direction: column;
    gap: 10px;
  }

  nav {
    flex-wrap: wrap;
    justify-content: center;
    gap: 14px;
  }

  nav a, nav button {
    font-size: 16px;
  }

  .main {
    width: 92%;
    padding: 35px 20px;
    margin-top: 120px;
  }

  .main h1 {
    font-size: 34px;
  }

  .main p {
    font-size: 17px;
  }

  .main button {
    font-size: 16px;
    padding: 12px 30px;
  }

  #helpBox {
    right: 50%;
    transform: translateX(50%);
    width: 90%;
    top: 100px;
  }

  footer {
    font-size: 13px;
  }
}

/* ====== Small Phones ====== */
@media (max-width: 360px) {
  .main h1 { font-size: 28px; }
  .main p { font-size: 15px; }
}
</style>
</head>

<body>

<header>
  <div class="logo">🍴 Easy 2 Eat</div>
  <nav>
    <a href="menu.html">قائمة المطاعم</a>
    <a href="login.html">تسجيل الدخول</a>
    <button id="helpBtn">مساعدة</button>
  </nav>
</header>

<div id="helpBox">
  <h3 style="color:#ffb400">موقع Easy 2 Eat 🍽️</h3>
  <p>إن واجهت أي مشكلة أثناء الطلب، لا تتردد في التواصل معنا ❤️</p>
  <button onclick="window.location.href='contact.html'">اتصل بنا</button>
</div>

<div class="main">
  <h1>مرحبًا بك في Easy 2 Eat</h1>
  <p>اطلب طعامك المفضل من أفضل المطاعم بسهولة وسرعة 🍕🚴‍♂️</p>
  <button onclick="window.location.href='menu.html'">ابدأ الطلب الآن</button>
</div>

<footer>
  © 2025 جميع الحقوق محفوظة - Easy 2 Eat
</footer>

<script>
const helpBtn = document.getElementById('helpBtn');
const helpBox = document.getElementById('helpBox');
let visible = false;

helpBtn.addEventListener('click', () => {
  visible = !visible;
  helpBox.style.display = visible ? 'block' : 'none';
});
</script>

</body>
</html>
