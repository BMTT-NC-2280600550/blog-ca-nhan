---
title: "Trang chủ"
url: "/home/"
draft: false
---

<style>


  .hero {
    width: 100%;
    height: 320px;
    background-image: url('/images/anhlaptrinh.jpg');
    background-size: cover;
    background-position: center;
    box-shadow: inset 0 0 60px rgba(0,0,0,0.2);
  }

  .home-container {
    max-width: 880px;
    margin: 0 auto;
    padding: 60px 30px;
    text-align: center;
    animation: fadeIn 1.2s ease forwards;
    opacity: 0;
  }

  @keyframes fadeIn {
    to { opacity: 1; }
  }


  .nav-buttons {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin-top: 40px;
  }

  .nav-buttons a {
    display: inline-block;
    padding: 14px 28px;
    font-size: 1.05em;
    color: #fff;
    background: linear-gradient(135deg, #0d1316ff, #00c6ff);
    border: none;
    border-radius: 8px;
    text-decoration: none;
    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .nav-buttons a:hover {
    transform: scale(1.07);
    box-shadow: 0 6px 20px rgba(0,0,0,0.3);
  }

  .footer-note {
    margin-top: 50px;
    font-size: 1em;
    color: #666;
  }
</style>

<div class="hero"></div>

<div class="home-container">
  <h1>💻 Blog Lập Trình Mạng Máy Tính</h1>

  <p>
    Mình là <strong>Trần Quốc Đại</strong> – sinh viên trường Đại học HUTECH.<br>
    Mình yêu thích môn Lập Trình Mạng Máy Tính và tạo blog này để chia sẻ tài liệu học tập, kỹ năng thực hành và kinh nghiệm cá nhân đến mọi người.
  </p>

  <div class="nav-buttons">
    <a href="/skills/">📚 Tài liệu & kỹ năng</a>
    <a href="/about/">👤 Giới thiệu bản thân</a>   
  </div>

  <p class="footer-note">💡 Cảm ơn bạn đã ghé thăm. Chúc bạn học tập hiệu quả và luôn giữ cảm hứng!</p>
</div>