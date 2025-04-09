# Hello, I'm [Shenghua Wang] 👋

## 🌍 About Me / 私について
**English:**
I'm a passionate developer and tech enthusiast dedicated to creating innovative solutions and exploring the endless possibilities of technology. With a love for open-source development and continuous learning, I strive to build meaningful projects that make a difference.

**日本語:**
テクノロジーの無限の可能性を探求し、革新的なソリューションを作り出すことに情熱を注ぐ開発者です。オープンソース開発と継続的な学習に対する愛を胸に、意味のあるプロジェクトを構築することに努めています。

## 🚀 Projects / プロジェクト
- [Project 1 japanese_text_speech_processor](https://github.com/zixuniaowu/japanese_text_speech_processor) 
- [Project 2 warehouse-management-ai-generator](https://github.com/zixuniaowu/warehouse-management-ai-generator) 
- [Project 3 TBD](https://github.com/yourusername/project3) - Short description

## 📚 Blog & Resources / ブログとリソース
- **Blog:** [zixuniao](https://zenn.dev/articles/0d98c6906a1c82/)
- **Books:** [ビッグ言語モデルノLLM詳細分解](https://zenn.dev/books/20887370158c19)

## 🌟 Technologies & Skills / 技術とスキル
![Python](https://img.shields.io/badge/-Python-3776AB?style=flat-square&logo=python&logoColor=white)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![React](https://img.shields.io/badge/-React-61DAFB?style=flat-square&logo=react&logoColor=white)
![Docker](https://img.shields.io/badge/-Docker-2496ED?style=flat-square&logo=docker&logoColor=white)

## 📊 GitHub Stats / GitHubの統計
![Your GitHub Stats](https://github-readme-stats.vercel.app/api?username=yourusername&show_icons=true&theme=radical)

## 🌌 Cosmic Visualization / 宇宙の可視化

<div align="center">
  <img src="https://cdnjs.cloudflare.com/ajax/libs/p5.js/1.4.0/p5.min.js" style="display:none;">
  <canvas id="cosmicCanvas" width="800" height="400"></canvas>
</div>

<script>
let stars = [];
let planets = [];

function setup() {
  let canvas = createCanvas(800, 400);
  canvas.parent('cosmicCanvas');
  background(0);
  
  // Create stars
  for (let i = 0; i < 200; i++) {
    stars.push({
      x: random(width),
      y: random(height),
      size: random(1, 3),
      speed: random(0.1, 0.5)
    });
  }
  
  // Create planets
  for (let i = 0; i < 5; i++) {
    planets.push({
      x: width/2,
      y: height/2,
      angle: random(TWO_PI),
      radius: random(100, 250),
      size: random(10, 30),
      speed: random(0.01, 0.03),
      color: color(random(100, 255), random(100, 255), random(100, 255))
    });
  }
}

function draw() {
  background(0);
  
  // Draw stars
  fill(255);
  stars.forEach(star => {
    ellipse(star.x, star.y, star.size);
    star.x += star.speed;
    if (star.x > width) star.x = 0;
  });
  
  // Draw planets
  planets.forEach(planet => {
    fill(planet.color);
    let x = width/2 + cos(planet.angle) * planet.radius;
    let y = height/2 + sin(planet.angle) * planet.radius;
    ellipse(x, y, planet.size);
    
    planet.angle += planet.speed;
  });
  
  // Draw sun
  fill(255, 255, 0);
  ellipse(width/2, height/2, 50);
}
</script>

## 🤝 Connect with Me / 私と繋がる
[![Email](https://img.shields.io/badge/-Email-D14836?style=flat-square&logo=gmail&logoColor=white)](mailto:zixuniaowu@gmail.com)

---

*Explore, Learn, Create / 探索し、学び、創造する*
