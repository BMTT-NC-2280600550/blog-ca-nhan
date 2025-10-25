---
title: "Tài liệu & kỹ năng"
url: "/skills/"
draft: false
---

<section class="hero fade-in">
  <h1>📘 Tài liệu & Kỹ năng Mạng Máy Tính</h1>
  <p>Trang học tập dành cho người muốn làm chủ kiến thức mạng từ lý thuyết đến thực hành.</p>
</section>

<section class="section fade-in">
  <h2>📚 Tài liệu học tập</h2>
  <ul>
    <li><strong>Giáo trình mạng máy tính:</strong> Tài liệu lý thuyết + bài tập thực hành.</li>
    <li><strong>Cấu hình IP, DHCP, NAT:</strong> Áp dụng trên thiết bị thật và mô phỏng.</li>
    <li><strong>Mô phỏng mạng bằng Cisco Packet Tracer:</strong> Thiết kế, kiểm thử và phân tích mạng.</li>
  </ul>
</section>

<section class="section fade-in">
  <h2>🧠 Kỹ năng cần thiết</h2>
  <div class="skills-grid">
    <div>✅ Hiểu mô hình OSI và TCP/IP</div>
    <div>✅ Cấu hình thiết bị mạng cơ bản</div>
    <div>✅ Viết chương trình socket TCP/UDP bằng Python hoặc C</div>
  </div>
</section>

<section class="section fade-in">
  <h2>🧪 Kiểm tra kiến thức</h2>
  <button id="startTestBtn">📖 Bắt đầu kiểm tra</button>
  <div id="quiz" class="fade" style="display:none;"></div>
  <div id="result" style="display:none;"></div>
</section>

<style>
body {
  font-family: 'Inter', 'Open Sans', sans-serif;
  margin: 0;
}

.hero {
  text-align: center;
  padding: 3rem 1rem 2.5rem;
  border-bottom: 1px solid var(--border-color, rgba(0,0,0,0.1));
}
.hero h1 {
  margin: 0;
  font-size: 2.5rem;
  font-weight: 700;
}
.hero p {
  font-size: 1.1rem;
  margin-top: 0.5rem;
  opacity: 0.9;
}

.section {
  max-width: 900px;
  margin: 2rem auto;
  padding: 2rem;
  border-radius: 12px;
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}
.section:hover {
  transform: translateY(-3px);
}
.section h2 {
  font-size: 1.7rem;
  margin-bottom: 1rem;
  border-left: 4px solid var(--accent-color, #0078d7);
  padding-left: 10px;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
  gap: 1rem;
}
.skills-grid div {
  padding: 1rem;
  border-radius: 10px;
  border: 1px solid var(--border-color, rgba(0,0,0,0.1));
  text-align: center;
  transition: all 0.3s ease;
}
.skills-grid div:hover {
  transform: scale(1.02);
}

#quiz div {
  padding: 1rem;
  margin-bottom: 1rem;
  border-radius: 10px;
  border: 1px solid var(--border-color, rgba(0,0,0,0.1));
}
#quiz h4 {
  margin-top: 0;
  font-size: 1.1rem;
}
#quiz button, #startTestBtn {
  margin-top: 1rem;
  padding: 0.7rem 1.4rem;
  background: var(--accent-color, #0078d7);
  color: white;
  border: none;
  border-radius: 6px;
  font-size: 1rem;
  cursor: pointer;
  transition: all 0.3s ease;
}
#quiz button:hover, #startTestBtn:hover {
  opacity: 0.9;
  transform: translateY(-2px);
}
#result {
  padding: 1rem;
  margin-top: 2rem;
  border-radius: 10px;
  border: 1px solid var(--border-color, rgba(0,0,0,0.1));
}

.fade {
  opacity: 0;
  transition: opacity 0.8s ease-in-out;
}
.fade.show {
  opacity: 1;
}
.fade-in {
  opacity: 0;
  animation: fadeInUp 0.8s ease forwards;
}
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}
</style>

<script>
const quizData = [
  { question: "Mô hình OSI có bao nhiêu tầng?", options: ["6", "8", "7", "5"], answer: 2, explanation: "Mô hình OSI gồm 7 tầng.", topic: "OSI" },
  { question: "Giao thức nào hoạt động ở tầng Transport?", options: ["Ethernet", "TCP", "HTTP", "IP"], answer: 1, explanation: "TCP là tầng Transport.", topic: "TCP/IP" },
  { question: "Lệnh kiểm tra kết nối mạng trong Windows?", options: ["netstat", "ipconfig", "ping", "tracert"], answer: 2, explanation: "Lệnh ping kiểm tra kết nối.", topic: "Thực hành mạng" },
  { question: "Cisco Packet Tracer dùng để làm gì?", options: ["Mô phỏng mạng", "Thiết kế website", "Lập trình Python", "Quản lý dữ liệu"], answer: 0, explanation: "Packet Tracer dùng để mô phỏng mạng.", topic: "Thực hành mạng" },
  { question: "Hàm tạo socket trong Python?", options: ["socket()", "bind()", "listen()", "connect()"], answer: 0, explanation: "Hàm socket() tạo socket mới.", topic: "Lập trình socket" }
];

document.getElementById("startTestBtn").addEventListener("click", () => {
  const quizContainer = document.getElementById("quiz");
  quizContainer.style.display = "block";
  setTimeout(() => quizContainer.classList.add("show"), 50);
  renderQuiz();
});

function renderQuiz() {
  const container = document.getElementById("quiz");
  container.innerHTML = "";
  quizData.forEach((q, index) => {
    const block = document.createElement("div");
    block.innerHTML = `
      <h4>Câu ${index + 1}: ${q.question}</h4>
      ${q.options.map((opt, i) => `
        <label><input type="radio" name="q${index}" value="${i}"> ${opt}</label><br/>
      `).join("")}
    `;
    container.appendChild(block);
  });

  const submitBtn = document.createElement("button");
  submitBtn.textContent = "📊 Xem kết quả";
  submitBtn.onclick = showResult;
  container.appendChild(submitBtn);
}

function showResult() {
  const result = document.getElementById("result");
  result.innerHTML = "";
  result.style.display = "block";

  let wrongTopics = {};
  let correctCount = 0;

  quizData.forEach((q, index) => {
    const selected = document.querySelector(`input[name="q${index}"]:checked`);
    const userAnswer = selected ? parseInt(selected.value) : null;
    const isCorrect = userAnswer === q.answer;

    if (isCorrect) correctCount++;
    else {
      if (!wrongTopics[q.topic]) wrongTopics[q.topic] = 0;
      wrongTopics[q.topic]++;
    }
  });

  result.innerHTML += `<h3>✅ Bạn đúng ${correctCount}/${quizData.length} câu</h3>`;
  if (correctCount === quizData.length) {
    result.innerHTML += `<p>🎉 Tuyệt vời! Bạn đã nắm vững toàn bộ kiến thức.</p>`;
  } else {
    result.innerHTML += `<p>📌 Cần ôn thêm ở các chủ đề sau:</p><ul>`;
    for (const topic in wrongTopics) {
      result.innerHTML += `<li><strong>${topic}</strong>: ${wrongTopics[topic]} câu sai</li>`;
    }
    result.innerHTML += `</ul>`;
  }
}
</script>