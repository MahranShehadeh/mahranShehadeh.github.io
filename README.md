# mahranShehadeh.github.io

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="utf-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>My GitHub.io Site</title>
  <meta name="description" content="Personal site hosted on GitHub Pages" />
  <meta name="color-scheme" content="light dark" />
  <link rel="icon" href="favicon.ico" />
  <style>
    :root {
      --bg: #0b0c10;
      --fg: #e5e7eb;
      --muted: #9ca3af;
      --accent: #22d3ee; /* cyan */
      --card: #111827;
      --link: #60a5fa;
    }
    @media (prefers-color-scheme: light) {
      :root {
        --bg: #ffffff;
        --fg: #0b0c10;
        --muted: #6b7280;
        --card: #f3f4f6;
        --link: #2563eb;
      }
    }
    * { box-sizing: border-box; }
    html, body { height: 100%; }
    body {
      margin: 0; font-family: ui-sans-serif, system-ui, -apple-system, Segoe UI, Roboto, Helvetica, Arial, "Apple Color Emoji", "Segoe UI Emoji";
      background: var(--bg); color: var(--fg); line-height: 1.6;
    }
    a { color: var(--link); text-decoration: none; }
    a:hover { text-decoration: underline; }
    .container { max-width: 980px; margin: 0 auto; padding: 24px; }
    header { display: flex; align-items: center; justify-content: space-between; gap: 16px; padding: 24px 0; }
    .brand { font-weight: 800; letter-spacing: 0.5px; font-size: 1.15rem; }
    nav a { margin-left: 16px; font-weight: 600; color: var(--muted); }
    nav a.active, nav a:hover { color: var(--fg); }

    .hero { padding: 72px 0; display: grid; grid-template-columns: 1.1fr 0.9fr; gap: 28px; align-items: center; }
    .hero h1 { font-size: clamp(2rem, 5vw, 3.2rem); line-height: 1.15; margin: 0 0 12px; }
    .hero p { color: var(--muted); font-size: 1.05rem; margin: 0 0 24px; }
    .cta { display: inline-flex; gap: 12px; }
    .btn { border: 1px solid transparent; background: var(--accent); color: #0b0c10; padding: 10px 16px; font-weight: 700; border-radius: 12px; }
    .btn.secondary { background: transparent; border-color: var(--muted); color: var(--fg); }
    .card {
      background: linear-gradient(180deg, var(--card), color-mix(in oklab, var(--card), transparent 40%));
      border: 1px solid color-mix(in oklab, var(--fg), transparent 85%);
      border-radius: 16px; padding: 20px; box-shadow: 0 10px 24px rgba(0,0,0,.10);
    }

    .grid { display: grid; grid-template-columns: repeat(3, minmax(0, 1fr)); gap: 16px; }
    .grid .card h3 { margin: 0 0 6px; font-size: 1.05rem; }
    .grid .card p { margin: 0; color: var(--muted); font-size: 0.95rem; }

    .section { padding: 56px 0; }
    .section h2 { font-size: 1.6rem; margin: 0 0 16px; }

    .about { display: grid; grid-template-columns: 1fr 1fr; gap: 16px; }
    .about .blurb { font-size: 1.05rem; color: var(--muted); }

    footer { padding: 40px 0; color: var(--muted); font-size: 0.95rem; }
    .social { display: flex; gap: 14px; }

    @media (max-width: 860px) {
      .hero { grid-template-columns: 1fr; }
      .grid { grid-template-columns: 1fr; }
      .about { grid-template-columns: 1fr; }
      nav { display:none; }
    }
  </style>
</head>
<body>
  <div class="container">
    <header>
      <div class="brand">Your Name</div>
      <nav>
        <a href="#about" class="active">About</a>
        <a href="#projects">Projects</a>
        <a href="#contact">Contact</a>
      </nav>
    </header>

    <section class="hero">
      <div>
        <h1>Hi, I’m <span style="color:var(--accent)">Your Name</span> — researcher • builder • human.</h1>
        <p>
          This is a clean, single‑file starter for your <strong>username.github.io</strong> site. 
          Replace the text with your story, add links, and ship it in minutes.
        </p>
        <div class="cta">
          <a class="btn" href="#projects">See Projects</a>
          <a class="btn secondary" href="#contact">Get in touch</a>
        </div>
      </div>
      <div class="card">
        <h3>Quick facts</h3>
        <ul>
          <li>Location: Your City</li>
          <li>Focus: What you do best</li>
          <li>Currently: What you’re up to</li>
        </ul>
      </div>
    </section>

    <section id="projects" class="section">
      <h2>Featured Projects</h2>
      <div class="grid">
        <article class="card">
          <h3><a href="#">Project One</a></h3>
          <p>One‑liner about what it is and why it’s cool.</p>
        </article>
        <article class="card">
          <h3><a href="#">Project Two</a></h3>
          <p>What you built, how, and the impact.</p>
        </article>
        <article class="card">
          <h3><a href="#">Project Three</a></h3>
          <p>Link to a repo, demo, paper, or post.</p>
        </article>
      </div>
    </section>

    <section id="about" class="section">
      <h2>About</h2>
      <div class="about">
        <div class="blurb">
          <p>
            Write a short bio here. Mention your interests, expertise, and the kind of opportunities you’re looking for. Keep it friendly and concise.
          </p>
          <p>
            You can also link to your <a href="#">CV</a> and highlight a couple of achievements.
          </p>
        </div>
        <div class="card">
          <h3>Skills</h3>
          <ul>
            <li>Python, MATLAB, C/C++</li>
            <li>Data Analysis, Simulation, Visualization</li>
            <li>Web, ML, Scientific Computing</li>
          </ul>
        </div>
      </div>
    </section>

    <section id="contact" class="section">
      <h2>Contact</h2>
      <p>
        Best way to reach me: <a href="mailto:you@example.com">you@example.com</a>
      </p>
      <div class="social">
        <a href="https://github.com/your-username">GitHub</a>
        <a href="https://www.linkedin.com/in/your-handle">LinkedIn</a>
        <a href="https://twitter.com/your-handle">Twitter/X</a>
      </div>
    </section>

    <footer>
      <div>© <span id="y"></span> Your Name · Built with GitHub Pages</div>
    </footer>
  </div>

  <script>
    // year stamp
    document.getElementById('y').textContent = new Date().getFullYear();
  </script>
</body>
</html>
