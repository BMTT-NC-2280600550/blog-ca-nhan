---
title: "Giới thiệu bản thân"
url: "/about/"
draft: false
markup: html
---

<style>
  .about-wrapper {
    max-width: 880px;
    margin: 60px auto;
    padding: 40px 30px;
    animation: fadeIn 1s ease forwards;
    opacity: 0;
  }

  @keyframes fadeIn {
    to { opacity: 1; }
  }

  .profile-header {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    justify-content: center;
    gap: 30px;
    margin-bottom: 40px;
  }

  .profile-header img {
    width: 180px;
    height: 180px;
    object-fit: cover;
    border-radius: 50%;
    box-shadow: 0 4px 12px rgba(0,0,0,0.2);
    transition: transform 0.3s ease;
  }

  .profile-header img:hover {
    transform: scale(1.05);
  }

  .profile-info {
    max-width: 500px;
  }

  .profile-info h2 {
    font-size: 2em;
    margin-bottom: 10px;
  }

  .profile-info p {
    font-size: 1.15em;
    line-height: 1.8;
    text-align: justify;
  }

  .section-title {
    font-size: 1.5em;
    margin-top: 40px;
    margin-bottom: 20px;
    text-align: center;
  }

  .cert-gallery {
    display: flex;
    justify-content: center;
    gap: 40px;
    flex-wrap: nowrap;
    overflow-x: auto;
    padding-bottom: 10px;
    scroll-snap-type: x mandatory;
  }

  .cert-card {
    flex: 0 0 auto;
    width: 160px;
    background: var(--card-bg);
    border-radius: 12px;
    padding: 16px;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    transition: transform 0.4s ease, box-shadow 0.4s ease;
    text-align: center;
    scroll-snap-align: center;
    animation: slideUp 0.8s ease forwards;
    opacity: 0;
  }

  .cert-card img {
    width: 100%;
    height: 120px;
    object-fit: cover;
    border-radius: 8px;
    margin-bottom: 10px;
    transition: transform 0.4s ease;
  }

  .cert-card h3 {
    font-size: 0.9rem;
    font-weight: 600;
    color: var(--text);
    transition: transform 0.4s ease;
  }

  .cert-card:hover {
    transform: translateY(-8px) scale(1.05);
    box-shadow: 0 12px 24px rgba(0,0,0,0.2);
  }

  .cert-card:hover img {
    transform: scale(1.08);
  }

  .cert-card:hover h3 {
    transform: translateY(-2px);
  }

  @keyframes slideUp {
    0% {
      transform: translateY(30px);
      opacity: 0;
    }
    100% {
      transform: translateY(0);
      opacity: 1;
    }
  }

  /* Dark mode hỗ trợ */
  :root {
    --card-bg: #f7f7f7;
    --text: #111;
  }

  [data-theme="dark"] {
    --card-bg: #1f1f1f;
    --text: #eee;
  }
</style>

<div class="about-wrapper">
  <!-- Giới thiệu bản thân -->
  <div class="profile-header">
    <img src="/images/Dai.jpg" alt="Ảnh đại diện Trần Quốc Đại" />
    <div class="profile-info">
      <h2>👨‍💻 Trần Quốc Đại</h2>
      <p>
        Xin chào! Mình là sinh viên ngành <strong>Công nghệ Thông tin</strong> tại <strong>Đại học HUTECH</strong>, với niềm đam mê đặc biệt dành cho <strong>lập trình mạng máy tính</strong> và các công nghệ hệ thống.<br><br>
        Blog này là nơi mình chia sẻ kiến thức, tài liệu học tập, và kỹ năng thực hành nhằm hỗ trợ cộng đồng sinh viên và những người yêu thích công nghệ phát triển tư duy và kỹ năng chuyên môn.<br><br>
        Từ khi bắt đầu học lập trình, mình đặc biệt yêu thích các lĩnh vực liên quan đến <strong>mạng máy tính</strong>, <strong>an toàn thông tin</strong> và <strong>hệ thống phân tán</strong>. Mình đã thực hiện nhiều dự án nhỏ như xây dựng ứng dụng chat qua socket, mô phỏng giao thức TCP, và triển khai hệ thống giám sát mạng nội bộ.<br><br>
        Ngoài giờ học, mình thường dành thời gian để tìm hiểu thêm về <strong>Linux server</strong>, <strong>Docker</strong>, và các công nghệ backend như <strong>Node.js</strong> và <strong>Python</strong>. Mình cũng đang học thêm về <strong>cloud computing</strong> để chuẩn bị cho các chứng chỉ như <strong>AWS Certified Cloud Practitioner</strong>.<br><br>
        Mục tiêu của mình là trở thành một <strong>Kỹ sư hệ thống mạng</strong> hoặc <strong>DevOps Engineer</strong> trong tương lai, có thể thiết kế và vận hành các hệ thống mạng hiệu quả, bảo mật và có khả năng mở rộng cao.<br><br>
        Blog này không chỉ là nơi lưu giữ hành trình học tập của mình, mà còn là nơi mình mong muốn kết nối với những người có cùng đam mê để cùng nhau phát triển.
      </p>
    </div>
  </div>

  <!-- Chứng chỉ -->
  <div class="section-title">🎓 Chứng chỉ & Thành tích</div>
  <div class="cert-gallery">
    <div class="cert-card">
      <a href="/images/cert1.jpg" target="_blank">
        <img src="/images/app-networking.png" alt="Networking Basics" />
        <h3>Networking Basics</h3>
      </a>
    </div>
    <div class="cert-card">
      <a href="/images/cert2.jpg" target="_blank">
        <img src="/images/js1.png" alt="JavaScript Essentials 1" />
        <h3>JavaScript Essentials 1</h3>
      </a>
    </div>
    <div class="cert-card">
      <a href="/images/cert3.jpg" target="_blank">
        <img src="/images/js2.png" alt="JavaScript Essentials 2" />
        <h3>JavaScript Essentials 2</h3>
      </a>
    </div>
  </div>
</div>