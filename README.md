<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Anurag Jha - Portfolio</title>
  <link rel="stylesheet" href="https://unpkg.com/aos@2.3.1/dist/aos.css" />
  <style>
    body { font-family: sans-serif; margin: 0; padding: 0; scroll-behavior: smooth; background: #0d1117; color: white; }
    section { padding: 50px; text-align: center; }
    img { border-radius: 10px; }
  </style>
</head>
<body>

  <section data-aos="fade-up">
    <h1>👋 Hi, I'm Anurag Jha</h1>
    <h3>🚀 Full Stack Developer | Web3 Learner</h3>
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=500&size=22&pause=1000&color=F73B94&center=true&vCenter=true&width=500&lines=Full+Stack+Developer;MERN+Stack+Enthusiast;Web3+%7C+Socket.io+%7C+Cloud+Lover;Let%27s+Build+Something+Awesome+Together!" />
  </section>

  <section data-aos="zoom-in">
    <img src="https://github-readme-streak-stats.herokuapp.com/?user=ajdevx&theme=radical" width="500" />
  </section>

  <section data-aos="fade-right">
    <img src="https://github-readme-stats.vercel.app/api?username=ajdevx&show_icons=true&theme=radical" width="500" />
  </section>

  <script src="https://unpkg.com/aos@2.3.1/dist/aos.js"></script>
  <script>
    AOS.init();

    // Reload GitHub SVG images when in view
    const imgs = document.querySelectorAll("img[src*='github-readme']");
    const observer = new IntersectionObserver((entries) => {
      entries.forEach(entry => {
        if (entry.isIntersecting) {
          const img = entry.target;
          const src = img.getAttribute("src").split("?")[0];
          img.setAttribute("src", `${src}?v=${Date.now()}`);
        }
      });
    }, { threshold: 0.5 });

    imgs.forEach(img => observer.observe(img));
  </script>

</body>
</html>
