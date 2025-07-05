<!DOCTYPE html>
<html lang="en" data-theme="dark">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Abdul Mueed</title>
  <link rel="icon" href="/favicon.ico" />
  <link href="https://fonts.googleapis.com/css2?family=Geist:wght@100..900&family=Bricolage+Grotesque:opsz,wght@12..96,200..800&display=swap" rel="stylesheet">
  <script>
        // Load saved theme
    window.addEventListener('DOMContentLoaded', () => {
      const savedTheme = localStorage.getItem('theme') || 'dark';
      document.documentElement.setAttribute('data-theme', savedTheme);
    });
  </script>
  <style>
    :root {
      --bg-dark: #000;
      --text-dark: #fff;
      --bg-light: #f9f9f9;
      --text-light: #111;
      --accent: #6366f1;
      --transition: 0.3s ease;
      --font-sans: "Geist", sans-serif;
      --font-alt: "Bricolage Grotesque", sans-serif;
    }

    html[data-theme="dark"] {
      background-color: var(--bg-dark);
      color: var(--text-dark);
    }

    html[data-theme="light"] {
      background-color: var(--bg-light);
      color: var(--text-light);
    }

    body {
      margin: 0;
      padding: 0;
      font-family: var(--font-sans);
      transition: background-color var(--transition), color var(--transition);
    }

    a {
      color: inherit;
      text-decoration: underline dotted;
      transition: color var(--transition);
    }

    .theme-toggle {
      cursor: pointer;
      padding: 6px 12px;
      border-radius: 8px;
      font-size: 14px;
      border: 1px solid #ccc;
      background-color: transparent;
      transition: all var(--transition);
    }

    .theme-toggle:hover {
      background-color: rgba(255, 255, 255, 0.1);
    }

    .container {
      max-width: 600px;
      margin: 0 auto;
      padding: 2rem;
      display: flex;
      flex-direction: column;
      gap: 4rem;
    }

    .header, .section {
      display: flex;
      flex-direction: column;
      gap: 1rem;
    }

    .title {
      font-family: var(--font-alt);
      font-weight: 700;
    }

    .subtitle {
      font-weight: 300;
      color: gray;
    }

    .card {
      background-color: rgba(255, 255, 255, 0.05);
      padding: 1rem;
      border-radius: 12px;
      transition: background-color var(--transition);
    }

    .card:hover {
      background-color: rgba(255, 255, 255, 0.1);
    }

    .social-links a {
      margin-right: 1rem;
    }

    .button {
      background: #fff;
      color: #000;
      padding: 0.5rem 1rem;
      border-radius: 8px;
      text-decoration: none;
      font-weight: 500;
      transition: all var(--transition);
    }

    .button:hover {
      background-color: #eee;
    }

    html[data-theme="light"] .button {
      background: #111;
      color: #fff;
    }

    html[data-theme="light"] .button:hover {
      background-color: #222;
    }
  </style>
</head>

<body>
  <div class="container">
    <div class="header">
      <div style="display: flex; justify-content: space-between; align-items: center;">
        <div>
          <h1 class="title">Abdul Mueed</h1>
          <span class="subtitle">Full-Stack Developer</span>
        </div>
        <a class="button" href="https://wa.me/923088200384">Hire Me</a>
      </div>
      <button class="theme-toggle" onclick="toggleTheme()"></button>
    </div>

    <div class="section">
      <h2 class="title">Who am I?</h2>
      <p>I’m an 18-year-old Web & App Developer and freelancer from Pakistan. Currently exploring <span style="text-decoration: underline dotted;">Rust & Go</span>.</p>

      <h2 class="title">What do I do?</h2>
      <p>I build scalable full-stack apps, design front-ends, and architect efficient back-ends. Also available for freelance projects.</p>
    </div>

    <div class="section">
      <h2 class="title">Projects</h2>
      <div class="card"><strong>AiBase</strong><br> A hub of AI tools using JSON storage. <a href="https://am-aibase.vercel.app/">Visit →</a></div>
      <div class="card"><strong>Lyricaa</strong><br> Music discovery and streaming platform. <a href="https://lyricaa.vercel.app/">Visit →</a></div>
      <div class="card"><strong>Codebin</strong><br> Share code snippets with output. <a href="https://am-codebin.vercel.app/">Visit →</a></div>
      <div class="card"><strong>Drawit</strong><br> Online drawing/presentation tool. <a href="https://drawir.vercel.app/">Visit →</a></div>
      <div class="card"><strong>Mysocials</strong><br> Social link-sharing app. <a href="https://msocials.vercel.app/">Visit →</a></div>
      <div class="card"><strong>URL Shortner</strong><br> Trackable short links with dashboard. <a href="https://msocials.vercel.app/">Visit →</a></div>
      <div class="card"><strong>IDE</strong><br> Online live HTML/CSS/JS editor. <a href="https://ide-alpha.vercel.app/">Visit →</a></div>
      <div class="card"><strong>Aurio</strong><br> Modern ad-free music app. <a href="https://github.com/BetaAE/aurioapp/releases/">Visit →</a></div>
      <div class="card"><strong>Cloud UP</strong><br> Free no-login streaming app. <a href="https://github.com/BetaAE/aurioapp/releases/">Visit →</a></div>
    </div>

    <div class="section">
      <h2 class="title">Work Experience</h2>
      <div class="card"><strong>Portals</strong> (04/03/25 - 03/06/25)<br> Frontend Developer - Responsive UI building and collaboration.</div>
      <div class="card"><strong>Agricart</strong> (2024-2025)<br> Fullstack Dev - Built scalable solutions across front and back end.</div>
      <div class="card"><strong>Freelancer</strong><br> Open for projects - worked on diverse client apps.</div>
    </div>

    <div class="section">
      <h2 class="title">Connect</h2>
      <div class="social-links">
        <a href="https://github.com/am-abdulmueed">GitHub</a>
        <a href="https://wa.me/923088200384">WhatsApp</a>
        <a href="https://instagram.com/am_abdulmueed">Instagram</a>
        <a href="mailto:am.abdulmueed3@gmail.com">Email</a>
      </div>
    </div>
  </div>
</body>
</html>
{\rtf1}