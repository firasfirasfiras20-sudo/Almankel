<!DOCTYPE html><html lang="ar" dir="rtl">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>مطعم المنقل</title>
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Cairo:wght@300;400;600;700;800&display=swap" rel="stylesheet">
  <style>
    * {
      margin: 0;
      padding: 0;
      box-sizing: border-box;
      font-family: 'Cairo', sans-serif;
    }body {
  background: #f7f5f2;
  color: #222;
  line-height: 1.7;
}

header {
  background: #111;
  color: white;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 18px 50px;
  position: sticky;
  top: 0;
  z-index: 1000;
  box-shadow: 0 2px 10px rgba(0,0,0,0.2);
}

.logo {
  display: flex;
  align-items: center;
  gap: 50px;
}

.logo img {
  width: 60px;
  height: 60px;
  border-radius: 50%;
  object-fit: cover;
}

.logo h1 {
  font-size: 28px;
  color: #ffb347;
}

nav a {
  color: white;
  text-decoration: none;
  margin: 0 10px;
  font-weight: 600;
  transition: 0.3s;
}

nav a:hover {
  color: #ffb347;
}

.hero {
  height: 90vh;
  background: linear-gradient(rgba(0,0,0,0.5), rgba(0,0,0,0.5)),
  url('https://i.postimg.cc/BQdk6ccH/hero.jpg') center/cover no-repeat;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  color: white;
  padding: 20px;
}

.hero-content h2 {
  font-size: 60px;
  margin-bottom: 20px;
}

.hero-content p {
  font-size: 22px;
  margin-bottom: 25px;
}

.btn {
  background: #ff9800;
  color: white;
  padding: 14px 30px;
  border-radius: 10px;
  text-decoration: none;
  font-weight: bold;
  transition: 0.3s;
}

.btn:hover {
  background: #e68900;
}

section {
  padding: 70px 8%;
}

.section-title {
  text-align: center;
  margin-bottom: 40px;
  font-size: 38px;
  color: #b85c00;
}

.gallery,
.meals {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
}

.gallery img,
.meal-card img {
  width: 100%;
  border-radius: 18px;
  height: 250px;
  object-fit: cover;
  transition: transform 0.4s;
}

.gallery img:hover,
.meal-card img:hover {
  transform: scale(1.04);
}

.meal-card {
  background: white;
  border-radius: 18px;
  overflow: hidden;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  transition: 0.3s;
}

.meal-card:hover {
  transform: translateY(-8px);
}

.meal-info {
  padding: 18px;
}

.meal-info h3 {
  color: #d35400;
  margin-bottom: 10px;
}

.booking {
  background: white;
  border-radius: 20px;
  padding: 40px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
  max-width: 850px;
  margin: auto;
}

.booking form {
  display: grid;
  gap: 18px;
}

.booking input,
.booking textarea,
.booking select {
  padding: 14px;
  border: 1px solid #ccc;
  border-radius: 10px;
  font-size: 16px;
}

.radio-group {
  display: flex;
  gap: 20px;
  align-items: center;
  font-size: 18px;
}

.booking button {
  background: #25D366;
  color: white;
  border: none;
  padding: 16px;
  border-radius: 12px;
  font-size: 18px;
  cursor: pointer;
  transition: 0.3s;
}

.booking button:hover {
  background: #1ebe5b;
}

.about {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 40px;
  align-items: center;
}

.about img {
  width: 100%;
  border-radius: 20px;
  height: 400px;
  object-fit: cover;
}

.reviews {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 25px;
}

.review-card {
  background: white;
  padding: 25px;
  border-radius: 18px;
  box-shadow: 0 4px 12px rgba(0,0,0,0.08);
}

.stars {
  color: gold;
  margin-bottom: 10px;
  font-size: 22px;
}

.rating {
  text-align: center;
  background: #111;
  color: white;
  border-radius: 20px;
  padding: 50px 20px;
}

.rating h3 {
  font-size: 60px;
  color: gold;
}

.qr-section {
  text-align: center;
}

.qr-section img {
  width: 250px;
  margin-top: 20px;
  border-radius: 20px;
  background: white;
  padding: 10px;
  box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

footer {
  background: #111;
  color: white;
  text-align: center;
  padding: 25px;
  margin-top: 40px;
}

@media(max-width: 768px) {
  header {
    flex-direction: column;
    gap: 15px;
    padding: 20px;
  }

  .hero-content h2 {
    font-size: 40px;
  }

  .hero-content p {
    font-size: 18px;
  }

  .booking {
    padding: 25px;
  }
}

  </style>
</head>
<body>  <header>
    <div class="logo">
      <img src="https://i.postimg.cc/WpJg6GcQ/logo-63030618005.png" alt="شعار مطعم المنقل">
      <h1>مطعم المنقل</h1>
    </div><nav>
  <a href="#gallery">المعرض</a>
  <a href="#meals">الوجبات</a>
  <a href="#booking">الحجز</a>
  <a href="#about">عن المطعم</a>
  <a href="#reviews">الآراء</a>
</nav>

  </header>  <section class="hero">
    <div class="hero-content">
      <h2>أهلاً بكم في مطعم المنقل</h2>
      <p>أفضل الأطباق والمشاوي الشرقية في شارع الناصرة</p>
      <a href="#booking" class="btn">احجز الآن</a>
    </div>
  </section>  <section id="gallery">
    <h2 class="section-title">معرض صور المطعم</h2><div class="gallery">
  <img src="https://i.postimg.cc/9Q9dmyJY/gallery1.jpg" alt="صورة مطعم">
  <img src="https://i.postimg.cc/bYFk1m5r/gallery2.jpg" alt="صورة مطعم">
  <img src="https://i.postimg.cc/s2cZxmSM/gallery3.jpg" alt="صورة مطعم">
  <img src="https://i.postimg.cc/BQdk6ccH/hero.jpg" alt="صورة مطعم">
</div>

  </section>  <section id="meals">
    <h2 class="section-title">أشهر وجبات المطعم</h2><div class="meals">
  <div class="meal-card">
    <img src="https://i.postimg.cc/ryS2rHsP/FB-IMG-1779049070859.jpg" alt="مشاوي">
    <div class="meal-info">
      <h3>مشاوي مشكلة</h3>
      <p>تشكيلة مميزة من الكباب والشيش والطاووق المشوي على الفحم.</p>
    </div>
  </div>

  <div class="meal-card">
    <img src="https://i.postimg.cc/cJrNt4tr/food3.jpg" alt="برجر">
    <div class="meal-info">
      <h3> سلطات المنقل </h3>
      <p>تشكيلة واسعة من السلطات ولا أطيب  .</p>
    </div>
  </div>

  <div class="meal-card">
    <img src="https://i.postimg.cc/d0zg7RYq/food1.jpg" alt="سلطات">
    <div class="meal-info">
      <h3> منسف باللحم البلدي</h3>
      <p>    أفضل وأطيب المناسف على الأصول   .</p>
    </div>
  </div>
</div>

  </section>  <section id="booking">
    <h2 class="section-title">نظام الحجز</h2><div class="booking">
  <form id="bookingForm">
    <input type="text" id="name" placeholder="الاسم الكامل" required>

    <input type="tel" id="phone" placeholder="رقم الهاتف" required>

    <input type="number" id="people" placeholder="عدد الأشخاص" required>

    <input type="text" id="meal" placeholder="الوجبات المفضلة">

    <div class="radio-group">
      <label>
        <input type="radio" name="orderType" value="داخل المطعم" checked>
        داخل المطعم
      </label>

      <label>
        <input type="radio" name="orderType" value="سفري">
        سفري
      </label>
    </div>

    <textarea id="notes" rows="5" placeholder="ملاحظات إضافية"></textarea>

    <button type="submit">تأكيد الحجز عبر واتساب</button>
  </form>
</div>

  </section>  <section id="about">
    <h2 class="section-title">نبذة عن المطعم</h2><div class="about">
  <div>
    <p>
      مطعم المنقل من أشهر المطاعم في شارع الناصرة، يقدم أشهى المشاوي والأطباق الشرقية
      بجودة عالية وأجواء عائلية مميزة.
    </p>

    <br>

    <p>
      يشرف على المطعم الأستاذ <strong>سليمان الجبعي</strong> الذي يحرص على تقديم أفضل خدمة
      وتجربة طعام فريدة لجميع الزبائن.
    </p>
  </div>

  <img src="https://i.postimg.cc/NfzDfstz/owner.jpg" alt="صاحب المطعم">
</div>

  </section>  <section id="reviews">
    <h2 class="section-title">آراء الزبائن</h2><div class="reviews">
  <div class="review-card">
    <div class="stars">★★★★★</div>
    <p>أفضل مطعم مشاوي جربته، الطعم رائع والخدمة ممتازة.</p>
    <strong>- أحمد</strong>
  </div>

  <div class="review-card">
    <div class="stars">★★★★★</div>
    <p>جلسات جميلة وأسعار مناسبة والموظفون محترمون جداً.</p>
    <strong>- محمد</strong>
  </div>

  <div class="review-card">
    <div class="stars">★★★★★</div>
    <p>أنصح الجميع بتجربة مشاوي المنقل، جودة عالية جداً.</p>
    <strong>- سارة</strong>
  </div>
</div>

  </section>  <section>
    <div class="rating">
      <h2>تقييم المطعم</h2>
      <h3>4.9 ★</h3>
      <p>بناءً على تقييمات الزبائن</p>
    </div>
  </section>  <section class="qr-section">
    <h2 class="section-title">تواصل معنا عبر واتساب</h2><p>امسح رمز QR للتواصل المباشر مع المطعم</p>

<img src="https://api.qrserver.com/v1/create-qr-code/?size=300x300&data=https://wa.me/97259-932-5261" alt="QR واتساب">

  </section>  <footer>
    <h3>مطعم المنقل - شارع الناصرة</h3>
    <p>المالك: سليمان الجبعي</p>
    <p>جميع الحقوق محفوظة © 2026</p>
  </footer>  <script>
    document.getElementById('bookingForm').addEventListener('submit', function(e) {
      e.preventDefault();

      const name = document.getElementById('name').value;
      const phone = document.getElementById('phone').value;
      const people = document.getElementById('people').value;
      const meal = document.getElementById('meal').value;
      const notes = document.getElementById('notes').value;
      const orderType = document.querySelector('input[name="orderType"]:checked').value;

      const message = `
طلب حجز جديد في مطعم المنقل

الاسم: ${name}
رقم الهاتف: ${phone}
عدد الأشخاص: ${people}
الوجبات المفضلة: ${meal}
نوع الطلب: ${orderType}
ملاحظات: ${notes}
      `;

      const whatsappNumber = '972599325261';
      const whatsappURL = `https://wa.me/${whatsappNumber}?text=${encodeURIComponent(message)}`;

      window.open(whatsappURL, '_blank');
    });
  </script></body>
</html>
