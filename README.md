<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Easy 2 Eat - الصفحة الرئيسية</title>
    <link rel="shortcut icon" href="image.png" type="image/x-icon" />

<style>
  @import url('https://fonts.googleapis.com/css2?family=Cairo:wght@500;700&display=swap');

  body {
    margin: 0;
    font-family: 'Cairo', sans-serif;
    background: url('3398.png') no-repeat center center fixed;
    background-size: cover;
    color: #fff;
  }

  /* رأس الصفحة */
  header {
    background: rgba(0, 0, 0, 0.75);
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 18px 60px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.5);
    position: sticky;
    top: 0;
    z-index: 1000;
  }

  .logo {
    font-size: 26px;
    font-weight: bold;
    color: #ffb400;
    text-transform: uppercase;
    letter-spacing: 1px;
  }

  nav {
    display: flex;
    align-items: center;
    gap: 25px;
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
    transform: scale(1.1);
  }

  #helpBtn {
    border: 2px solid #ffb400;
    padding: 6px 14px;
    border-radius: 25px;
    font-weight: bold;
  }

  #helpBtn:hover {
    background-color: #ffb400;
    color: #000;
  }

  /* نافذة المساعدة */
  #helpBox {
    position: fixed;
    top: 90px;
    right: 40px;
    background: rgba(0,0,0,0.85);
    border: 2px solid #ffb400;
    border-radius: 15px;
    padding: 20px;
    color: #fff;
    width: 260px;
    box-shadow: 0 6px 20px rgba(0,0,0,0.4);
    font-size: 15px;
    display: none;
    animation: fadeIn 0.4s ease-in-out;
    z-index: 9999;
  }

  #helpBox h3 {
    margin-top: 0;
    color: #ffb400;
  }

  #helpBox button {
    margin-top: 10px;
    background: #ffb400;
    color: #000;
    border: none;
    padding: 8px 16px;
    border-radius: 25px;
    cursor: pointer;
    font-weight: bold;
    transition: 0.3s;
  }

  #helpBox button:hover {
    background: #e0a600;
  }

  /* القسم الرئيسي */
  .main {
    text-align: center;
    margin-top: 140px;
    background: rgba(0, 0, 0, 0.55);
    padding: 70px;
    border-radius: 25px;
    width: 70%;
    margin-right: auto;
    margin-left: auto;
    box-shadow: 0 8px 25px rgba(0,0,0,0.5);
    animation: fadeIn 1.2s ease-in-out;
  }

  .main h1 {
    font-size: 56px;
    color: #ffb400;
    margin-bottom: 20px;
  }

  .main p {
    font-size: 22px;
    color: #eee;
    margin-bottom: 40px;
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
    transition: 0.3s;
  }

  .main button:hover {
    transform: scale(1.08);
    background-color: #e0a600;
  }

  footer {
    text-align: center;
    padding: 18px;
    background: rgba(0,0,0,0.8);
    font-size: 15px;
    position: fixed;
    bottom: 0;
    width: 100%;
    letter-spacing: 1px;
  }

  @keyframes fadeIn {
    from {opacity: 0; transform: translateY(25px);}
    to {opacity: 1; transform: translateY(0);}
  }

  @media (max-width: 768px) {
    header {
      flex-direction: column;
      gap: 10px;
    }

    .main {
      width: 90%;
      padding: 40px;
    }

    .main h1 { font-size: 38px; }
    .main p { font-size: 18px; }
    .main button { font-size: 16px; padding: 12px 30px; }
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
    <h3>موقع Easy 2 Eat 🍽️</h3>
    <p>مرحبًا بك! إن واجهت أي متاعب أثناء الطلب أو التصفح، يمكنك دائمًا التواصل معنا ❤️</p>
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
