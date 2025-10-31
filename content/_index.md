---
title: "Blog của Đại"
type: "page"
markup: html
---

<style>
  .intro-section {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: flex-start;
    padding: 40px 20px;
    gap: 30px;
    min-height: 80vh;
  }

  .intro-image {
    width: 100%;
    max-width: 960px;
    border-radius: 12px;
    overflow: hidden;
    box-shadow: 0 4px 12px rgba(0,0,0,0.1);
    animation: fadeInUp 0.8s ease forwards;
    opacity: 0;
  }

  .intro-image img {
    width: 100%;
    height: auto;
    display: block;
  }

  .intro-content {
    max-width: 800px;
    text-align: center;
    animation: fadeInUp 1s ease forwards;
    opacity: 0;
  }

  .intro-title {
    font-size: 2.5rem;
    font-weight: 700;
    margin-bottom: 20px;
  }

  .intro-title span {
    font-weight: 600;
  }

  .intro-lead {
    font-size: 1.15rem;
    line-height: 1.8;
    margin-bottom: 20px;
  }

  .intro-subtext {
    font-size: 1rem;
    opacity: 0.85;
    margin-bottom: 30px;
  }

  .intro-buttons {
    margin-top: 20px;
  }

  .btn {
    display: inline-block;
    padding: 0.7rem 1.4rem;
    font-size: 1rem;
    font-weight: 500;
    border-radius: 6px;
    background-color: #f0f0f0;
    color: inherit;
    text-decoration: none;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 6px 12px rgba(0,0,0,0.1);
  }

  @keyframes fadeInUp {
    from {
      transform: translateY(30px);
      opacity: 0;
    }
    to {
      transform: translateY(0);
      opacity: 1;
    }
  }

  @media (max-width: 768px) {
    .intro-title {
      font-size: 2rem;
    }
    .intro-lead {
      font-size: 1.05rem;
    }
  }
</style>

<section class="intro-section">
  <!-- Ảnh bìa -->
  <div class="intro-image">
    <img src="/images/anhtrangtri.jpg" alt="Ảnh bìa blog của Đại" />
  </div>

  <!-- Nội dung giới thiệu -->
  <div class="intro-content">
    <h1 class="intro-title">👨‍💻 Xin chào, mình là <span>Trần Quốc Đại</span></h1>
    <p class="intro-lead">
      Chào mừng bạn đến với blog cá nhân — nơi mình chia sẻ kiến thức về
      <strong>lập trình mạng máy tính</strong>, <strong>Socket Programming</strong>,
      và các công nghệ hiện đại trong ngành CNTT.
    </p>

    <p class="intro-subtext">
      Nếu bạn đang tìm hiểu về lập trình mạng, hy vọng bạn sẽ tìm thấy điều gì đó hữu ích tại đây 💡
    </p>

    <div class="intro-buttons">
      <a href="https://blogcuadai.netlify.app/home/" class="btn">🏡 Vào trang chủ</a>
    </div>
  </div>
</section>