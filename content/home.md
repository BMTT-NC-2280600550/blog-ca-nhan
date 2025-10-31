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

  .featured-posts, .mission {
    margin-top: 60px;
    text-align: left;
    max-width: 720px;
    margin-left: auto;
    margin-right: auto;
  }

  .featured-posts ul {
    list-style: none;
    padding-left: 0;
  }

  .featured-posts li {
    margin-bottom: 10px;
  }

  .featured-posts a {
    color: #007acc;
    text-decoration: none;
  }

  .featured-posts a:hover {
    text-decoration: underline;
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
    <a href="/contact/">📩 Liên hệ</a>
  </div>

  <div class="featured-posts">
    <h2>📝 Bài viết thực tế về Lập Trình Mạng Máy Tính</h2>
    <ul>
      <li><a href="/posts/mang-may-tinh-co-ban/">🔌 Mạng máy tính cơ bản</a></li>
      <li><a href="/posts/linux-va-devops/">🐧 Linux & DevOps cho người mới</a></li>
      <li><a href="/posts/thuc-hanh-voi-wireshark/">🕵️‍♂️ Phân tích gói tin với Wireshark</a></li>
      <li><a href="/posts/socket-programming/">🔗 Lập trình socket với Python</a></li>
      <li><a href="/posts/http-request-response/">🌐 Hiểu rõ HTTP Request & Response</a></li>
      <li><a href="/posts/tcp-udp/">📡 So sánh TCP và UDP trong lập trình mạng</a></li>
      <li><a href="/posts/firewall-va-an-toan/">🛡️ Cấu hình firewall và bảo mật mạng</a></li>
      <li><a href="/posts/multithread-server/">🧵 Xây dựng server đa luồng</a></li>
      <li><a href="/posts/icmp-ping/">📶 Phân tích ICMP và lệnh ping</a></li>
    </ul>
  </div>

  <div class="mission">
    <h2>🎯 Mục tiêu của blog</h2>
    <p>
      Blog này được xây dựng với mong muốn giúp sinh viên và người mới học lập trình mạng máy tính có một nơi để tham khảo tài liệu, thực hành và kết nối cộng đồng.
    </p>
  </div>

  <p class="footer-note">💡 Cảm ơn bạn đã ghé thăm. Chúc bạn học tập hiệu quả và luôn giữ cảm hứng!</p>
</div>