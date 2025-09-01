<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8">
  <title>Cà phê Hoa Tím</title>
</head>
<body>
  <h1>Chào mừng bạn đến quán Cà phê Hoa Tím ☕💜</h1>
  <p>Đây là website menu thử nghiệm đầu tiên của bạn.</p>
</body>
</html>
<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Cà phê Hoa Tím – Quán nhỏ, vị lớn</title>
  <meta name="description" content="Cà phê Hoa Tím – menu nước ngon, không gian dễ thương, giá dễ chịu. Mở cửa mỗi ngày." />
  <style>
    /* Reset nhỏ */
    * { box-sizing: border-box; }
    body { margin: 0; font-family: system-ui, Arial, sans-serif; color: #222; background: #faf7ff; }

    /* Màu thương hiệu tím nhẹ */
    :root {
      --purple: #7b2cbf;
      --purple-2: #9d4edd;
      --bg-card: #ffffff;
      --text-dim: #5c5c5c;
    }

    /* Header */
    header {
      position: sticky; top: 0; z-index: 10;
      background: #fff; border-bottom: 1px solid #eee;
      display: flex; gap: 16px; align-items: center; justify-content: space-between;
      padding: 10px 16px;
    }
    .brand { display: flex; align-items: center; gap: 10px; text-decoration: none; color: #222; }
    .brand img { width: 36px; height: 36px; border-radius: 8px; object-fit: cover; }
    .brand strong { font-size: 18px; }

    nav a {
      color: var(--purple); text-decoration: none; font-weight: 600; margin-left: 14px;
    }
    nav a:hover { text-decoration: underline; }

    /* Hero */
    .hero {
      position: relative; overflow: hidden; border-bottom: 1px solid #eee;
      background: linear-gradient(180deg, rgba(123,44,191,0.12), transparent);
    }
    .hero-inner {
      max-width: 1100px; margin: 0 auto; padding: 28px 16px 18px;
      display: grid; grid-template-columns: 1.1fr 1fr; gap: 20px;
    }
    .hero h1 { margin: 0 0 10px; font-size: clamp(26px, 4vw, 40px); color: #2a2a2a; }
    .hero p { margin: 0 0 18px; color: var(--text-dim); }
    .cta {
      display: inline-block; padding: 10px 16px; border-radius: 10px;
      background: var(--purple); color: #fff; text-decoration: none; font-weight: 700;
      box-shadow: 0 6px 18px rgba(123,44,191,0.25);
    }
    .hero figure {
      margin: 0; aspect-ratio: 4/3; border-radius: 14px; overflow: hidden; background: #eee;
      box-shadow: 0 10px 30px rgba(0,0,0,0.06);
    }
    .hero img { width: 100%; height: 100%; object-fit: cover; display: block; }

    /* Section khối */
    section { max-width: 1100px; margin: 24px auto; padding: 0 16px; }
    h2 { margin: 0 0 12px; font-size: 22px; }

    /* Thẻ (card) */
    .cards {
      display: grid; gap: 16px; grid-template-columns: repeat(auto-fit, minmax(220px, 1fr));
    }
    .card {
      background: var(--bg-card); border: 1px solid #eee; border-radius: 14px; overflow: hidden;
      box-shadow: 0 8px 24px rgba(0,0,0,0.04);
    }
    .card img { width: 100%; height: 150px; object-fit: cover; display: block; }
    .card .body { padding: 12px; }
    .price { color: var(--purple); font-weight: 700; }

    /* Bảng giờ mở cửa */
    .hours { width: 100%; border-collapse: collapse; background: #fff; border-radius: 12px; overflow: hidden; }
    .hours th, .hours td { padding: 10px 12px; border-bottom: 1px solid #eee; text-align: left; }
    .hours tr:last-child td { border-bottom: none; }

    /* Footer */
    footer {
      margin-top: 28px; background: #fff; border-top: 1px solid #eee;
      padding: 16px; text-align: center; color: #666;
    }

    /* Responsive hero 1 cột trên mobile */
    @media (max-width: 800px) {
      .hero-inner { grid-template-columns: 1fr; }
    }
  </style>
</head>
<body>
  <!-- HEADER -->
  <header>
    <a class="brand" href="#top">
      <!-- Thay logo.png khi bạn upload -->
      <img src="images/logo.png" alt="Logo Cà phê Hoa Tím" onerror="this.style.display='none'">
      <strong>Cà phê Hoa Tím</strong>
    </a>
    <nav>
      <a href="#gioi-thieu">Giới thiệu</a>
      <a href="#menu">Menu</a>
      <a href="#lien-he">Liên hệ</a>
    </nav>
  </header>

  <!-- HERO -->
  <section class="hero" id="gioi-thieu">
    <div class="hero-inner">
      <div>
        <h1>Quán nhỏ, vị lớn 💜</h1>
        <p>Không gian tím dễ thương, cà phê đậm đà – nơi bạn có thể ngồi chill, trò chuyện và lên năng lượng mỗi ngày.</p>
        <a class="cta" href="#menu">Xem menu</a>
      </div>
      <figure>
        <!-- Thay hero.jpg sau khi upload -->
        <img src="images/hero.jpg" alt="Không gian Cà phê Hoa Tím" />
      </figure>
    </div>
  </section>

  <!-- MENU NỔI BẬT -->
  <section id="menu">
    <h2>✨ Món nổi bật</h2>
    <div class="cards">
      <article class="card">
        <img src="images/cafe-sua.jpg" alt="Cà phê sữa đá">
        <div class="body">
          <strong>Cà phê sữa đá</strong>
          <div class="price">20.000đ</div>
        </div>
      </article>
      <article class="card">
        <img src="images/cafe-den.jpg" alt="Cà phê đen">
        <div class="body">
          <strong>Cà phê đen</strong>
          <div class="price">15.000đ</div>
        </div>
      </article>
      <article class="card">
        <img src="images/cacao-sua.jpg" alt="Cacao sữa">
        <div class="body">
          <strong>Cacao sữa</strong>
          <div class="price">28.000đ</div>
        </div>
      </article>
      <article class="card">
        <img src="images/chanh-day.jpg" alt="Chanh dây">
        <div class="body">
          <strong>Chanh dây</strong>
          <div class="price">25.000đ</div>
        </div>
      </article>
    </div>
  </section>

  <!-- GIỜ MỞ CỬA -->
  <section>
    <h2>🕒 Giờ mở cửa</h2>
    <table class="hours">
      <tr><th>Thứ 2 – Thứ 6</th><td>06:30 – 21:30</td></tr>
      <tr><th>Thứ 7 – Chủ nhật</th><td>07:00 – 22:00</td></tr>
    </table>
  </section>

  <!-- LIÊN HỆ & BẢN ĐỒ -->
  <section id="lien-he">
    <h2>📍 Liên hệ & Địa chỉ</h2>
    <p><strong>Địa chỉ:</strong> 123 Hoa Tím, Lai Vung, Đồng Tháp</p>
    <p><strong>Điện thoại:</strong> <a href="tel:0909123456">0909 123 456</a></p>
    <p><strong>Facebook:</strong> <a href="#" target="_blank" rel="noopener">fb.com/cafehoatim</a></p>

    <!-- Nhúng bản đồ: bạn có thể thay bằng iframe Google Maps của quán -->
    <div style="margin-top:12px; border:1px solid #eee; border-radius:12px; overflow:hidden;">
      <iframe
        title="Bản đồ quán"
        src="https://www.openstreetmap.org/export/embed.html?bbox=105.0%2C10.2%2C106.0%2C10.8&layer=mapnik"
        style="width:100%; height:300px; border:0;">
      </iframe>
    </div>
  </section>

  <footer>
    © <span id="y"></span> Cà phê Hoa Tím • Rất vui được phục vụ bạn!
  </footer>

  <script>
    // Năm động
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
