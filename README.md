# 👋 Hi there — I'm **Md Abdul Haseeb Sagri**
![Profile Views](https://komarev.com/ghpvc/?username=reck07&color=blue)

👨‍💻 Computer Science Graduate • Aspiring Polymath  
🚀 Python | JavaScript | Web Development  
🎯 I build efficient systems & smart automation

---

![Typing SVG](https://readme-typing-svg.herokuapp.com?color=00F7FF&lines=Crafting+Solutions+with+Code;Driven+by+Curiosity;Building+Real+Impact)

---

## 🌐 Connect With Me
- 🔗 **LinkedIn:** https://www.linkedin.com/in/md-abdul-haseeb-sagri/  
- 📸 **Instagram:** https://www.instagram.com/the_reckoner076/  
- 🐦 **Twitter (X):** https://x.com/SagriHasee7509  
- 💬 **WhatsApp:** https://wa.me/917090884656  
- 📧 **Email:** abdulhaseebsagri@gmail.com

---

## 🛠️ Tech Stack
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-003B57?style=for-the-badge&logo=mysql&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![VSCode](https://img.shields.io/badge/VSCode-007ACC?style=for-the-badge&logo=visual-studio-code&logoColor=white)

---

## 🚀 Featured Projects (click to open)
<p>
  <a href="https://github.com/reck07/AI-Powered-Data-Entry-Agent">🤖 AI-Powered-Data-Entry-Agent</a> — Python automation to simplify repetitive data-entry workflows.<br>
  <a href="https://github.com/reck07/Ai-powered-crop-recommendation-Project-System">🌱 AI-Powered Crop Recommendation System</a> — Python system to suggest crops based on input data.<br>
  <a href="https://github.com/reck07/coffee-web-page">☕ coffee-web-page</a> — Responsive front-end demo built with HTML & CSS.<br>
  <a href="https://github.com/reck07/photo-gallery">🖼️ photo-gallery</a> — Python project for organizing & displaying images.<br>
  <a href="https://github.com/reck07/The-Calculator">🧮 The-Calculator</a> — JavaScript calculator with DOM interactions.<br>
  <a href="https://github.com/reck07/PANTECH_MARINE">🚢 PANTECH_MARINE</a> — Academic/system project demonstrating structured implementation.
</p>

---

## 📊 GitHub Stats & Activity (dynamic)
<!-- Primary stats -->
<a href="https://github.com/reck07">
  <img align="center" src="https://github-readme-stats.vercel.app/api?username=reck07&show_icons=true&theme=radical" alt="Md Abdul Haseeb Sagri's GitHub stats" />
</a>

<!-- Top languages (fallback note below) -->
<a href="https://github.com/reck07">
  <img align="center" src="https://github-readme-stats.vercel.app/api/top-langs/?username=reck07&layout=compact&theme=radical" alt="Top Languages" />
</a>

> **Note:** If the above cards or the Top Languages image appears blank or fails to load, that is usually due to external service rate limits or the public service being temporarily paused. To ensure a reliable display you can:
> 1. Try the faster alternate endpoint: `https://github-readme-stats-fast.vercel.app/api?username=reck07&show_icons=true&theme=radical`  
> 2. Or self-host the `github-readme-stats` service with a GitHub token (recommended for long-term reliability).

---

## 🏆 Achievements & Trophies
<a href="https://github.com/reck07">
  <img align="center" src="https://github-profile-trophy.vercel.app/?username=reck07&theme=radical" alt="GitHub Trophies" />
</a>

<!-- Streak & contribution visuals -->
<p>
[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=reck07&theme=radical)](https://github.com/reck07)  
![Contribution Snake](https://github.com/Platane/snk/raw/output/github-contribution-grid-snake.svg)
</p>

> **Two quick lines about stats failures:**  
> • If GitHub Stats / Top Languages don’t render, it’s usually due to the external SVG generator being rate-limited or unavailable.  
> • Self-hosting or using an alternate endpoint will make these cards load consistently.

---

## 📚 Currently Learning
- Advanced JavaScript (Async/Await, Event Loop & Patterns)  
- Building smarter automation systems using Python & ML tools  
- Designing scalable backend architectures and clean APIs

---

## ✨ Career Goal (inspiring)
To craft elegant, human-centered systems that automate the tedious, amplify human potential, and multiply impact — one thoughtful line of code at a time.  
I build tools that free people to focus on creativity and meaning, while code takes care of the rest.

---

## 🧩 Small Demo — Embedded Snake Game (open in browser)
Below is a simple Snake game you can save as `snake.html` and open in a browser. (Fun demo to share on your profile.)

```html
<!doctype html>
<html>
<head>
  <meta charset="utf-8" />
  <title>Simple Snake</title>
  <style>
    body { display:flex; align-items:center; justify-content:center; height:100vh; margin:0; background:#0b0b0b; }
    canvas { background:#000; display:block; border:4px solid #111; }
    .hint { color:#ccc; font-family:Arial; text-align:center; margin-top:12px; }
  </style>
</head>
<body>
  <div>
    <canvas id="game" width="400" height="400"></canvas>
    <div class="hint">Use arrow keys to play. Refresh to restart.</div>
  </div>
<script>
const canvas = document.getElementById('game');
const ctx = canvas.getContext('2d');
const grid = 20;
let vx = grid, vy = 0;
let snake = [{x:200,y:200}];
let food = randomFood();

function randomFood() {
  return { x: Math.floor(Math.random()*20)*grid, y: Math.floor(Math.random()*20)*grid };
}
document.addEventListener('keydown', e => {
  if (e.key === 'ArrowUp' && vy === 0){ vx=0; vy=-grid; }
  if (e.key === 'ArrowDown' && vy === 0){ vx=0; vy=grid; }
  if (e.key === 'ArrowLeft' && vx === 0){ vx=-grid; vy=0; }
  if (e.key === 'ArrowRight' && vx === 0){ vx=grid; vy=0; }
});

function loop(){
  // move
  const head = { x: snake[0].x + vx, y: snake[0].y + vy };
  // wall collision (wrap-around)
  head.x = (head.x + 400) % 400;
  head.y = (head.y + 400) % 400;
  // self collision -> reset
  for (let i=0;i<snake.length;i++){
    if (snake[i].x===head.x && snake[i].y===head.y){
      snake = [{x:200,y:200}];
      vx = grid; vy = 0;
      food = randomFood();
      return;
    }
  }
  snake.unshift(head);
  if (head.x===food.x && head.y===food.y){
    food = randomFood();
  } else {
    snake.pop();
  }

  // draw
  ctx.fillStyle = '#000';
  ctx.fillRect(0,0,400,400);
  ctx.fillStyle = '#e74c3c';
  ctx.fillRect(food.x, food.y, grid, grid);
  ctx.fillStyle = '#2ecc71';
  snake.forEach(part => ctx.fillRect(part.x, part.y, grid-1, grid-1));
}

setInterval(loop, 100);
</script>
</body>
</html>
