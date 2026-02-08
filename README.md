<style>
  /* 1. DARK MODE THEME */
  body {
    background-color: #0d1117; /* GitHub Dark Mode Background */
    color: #c9d1d9; /* Soft White Text */
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Helvetica, Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
  }
  
  a { text-decoration: none; color: inherit; }
  
  /* 2. NAVIGATION BAR */
  .navbar {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 40px;
    background: #161b22;
    border-bottom: 1px solid #30363d;
    position: sticky;
    top: 0;
    z-index: 1000;
  }
  .nav-logo { font-weight: bold; font-size: 1.2em; color: #fff; }
  .nav-links a {
    margin-left: 20px;
    color: #8b949e;
    font-size: 0.95em;
    transition: color 0.2s;
  }
  .nav-links a:hover { color: #58a6ff; }
  
  .resume-btn {
    background-color: #238636; /* Green Button */
    color: white !important;
    padding: 8px 16px;
    border-radius: 6px;
    font-weight: 600;
    border: 1px solid rgba(240,246,252,0.1);
  }
  .resume-btn:hover { background-color: #2ea043; }

  /* 3. HERO SECTION */
  .hero {
    text-align: center;
    padding: 100px 20px;
    max-width: 800px;
    margin: 0 auto;
  }
  .hero h1 {
    font-size: 3.5em;
    color: #fff;
    margin-bottom: 10px;
    letter-spacing: -1px;
  }
  .hero p {
    font-size: 1.2em;
    color: #8b949e;
    max-width: 600px;
    margin: 0 auto 30px auto;
  }

  /* 4. SECTIONS (Common Styles) */
  .section {
    padding: 60px 20px;
    max-width: 1000px;
    margin: 0 auto;
    border-top: 1px solid #21262d;
  }
  .section-title {
    font-size: 1.8em;
    color: #fff;
    margin-bottom: 30px;
    border-left: 4px solid #58a6ff; /* Blue Accent Line */
    padding-left: 15px;
  }

  /* 5. EXPERIENCE GRID */
  .experience-item {
    margin-bottom: 30px;
  }
  .role-title {
    font-size: 1.1em;
    font-weight: 700;
    color: #fff;
  }
  .company-name { color: #58a6ff; margin-bottom: 5px; display: inline-block; }
  .date { float: right; font-size: 0.9em; color: #6e7681; }
  .exp-desc { color: #8b949e; margin-top: 5px; }

  /* 6. PROJECT GRID */
  .project-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 20px;
  }
  .project-card {
    background: #161b22;
    border: 1px solid #30363d;
    padding: 25px;
    border-radius: 6px;
    transition: transform 0.2s, border-color 0.2s;
  }
  .project-card:hover {
    transform: translateY(-5px);
    border-color: #8b949e;
  }
  .project-title {
    font-size: 1.2em;
    font-weight: 700;
    color: #58a6ff;
    margin-bottom: 10px;
  }
  .tech-stack {
    font-size: 0.8em;
    color: #8b949e;
    font-family: monospace;
    background: rgba(110,118,129,0.1);
    padding: 4px 8px;
    border-radius: 4px;
  }

  /* 7. CONTACT FOOTER */
  .footer {
    text-align: center;
    padding: 40px;
    background: #161b22;
    margin-top: 60px;
    border-top: 1px solid #30363d;
  }
</style>

<div class="navbar">
  <div class="nav-logo">M.M.</div>
  <div class="nav-links">
    <a href="#about">About</a>
    <a href="#experience">Experience</a>
    <a href="#projects">Work</a>
    <a href="#contact">Contact</a>
    <a href="resume.pdf" target="_blank" class="resume-btn">Resume</a>
  </div>
</div>

<div class="hero">
  <h1>Mihika Maheshwari</h1>
  <p>Computer Science Student @ BITS Pilani | Systems & ML Engineer</p>
</div>

<div id="about" class="section">
  <div class="section-title">About Me</div>
  <p>
    I am a final-year Computer Science student passionate about building robust systems and intelligent applications. 
    My work spans from low-level systems programming (building my own Git and SQL engines) to deploying machine learning models for real-world fraud detection.
    I enjoy solving complex problems that require a deep understanding of how computers work under the hood.
  </p>
</div>

<div id="experience" class="section">
  <div class="section-title">Experience</div>
  
  <div class="experience-item">
    <div class="role-title">Software Intern <span class="date">May 2025 - July 2025</span></div>
    <div class="company-name">Bid Alert</div>
    <div class="exp-desc">
      <ul>
        <li>Engineered <strong>BidGPT</strong>, a context-aware AI tool that reduced manual bid clarification effort by <strong>30%</strong>.</li>
        <li>Implemented on-demand translation and refactored the UI for better mobile responsiveness.</li>
      </ul>
    </div>
  </div>

  <div class="experience-item">
    <div class="role-title">Teaching Assistant <span class="date">Jan 2025 - Mar 2025</span></div>
    <div class="company-name">BITS Pilani</div>
    <div class="exp-desc">
      Assisted in managing laboratory sessions and guiding students in the Chemistry Laboratory.
    </div>
  </div>
</div>

<div id="projects" class="section">
  <div class="section-title">Selected Work</div>
  <div class="project-grid">

    <a href="https://github.com/mihika185/SourceTrack" class="project-card">
      <div class="project-title">SourceTrack</div>
      <span class="tech-stack">PYTHON • SYSTEMS</span>
      <p>A Git-like version control system built from scratch. Features SHA-1 object storage, commit DAGs, and branching logic.</p>
    </a>

    <a href="https://github.com/mihika185/Relix" class="project-card">
      <div class="project-title">Relix</div>
      <span class="tech-stack">PYTHON • SQL</span>
      <p>In-memory SQL engine with a custom parser. Supports nested-loop joins and complex queries, validated by 160+ tests.</p>
    </a>

    <a href="https://github.com/mihika185/MemCore" class="project-card">
      <div class="project-title">MemCore</div>
      <span class="tech-stack">OS INTERNALS</span>
      <p>User-space memory manager implementing First Fit, Best Fit, and Buddy System allocation strategies.</p>
    </a>

    <a href="https://github.com/mihika185/TxnShield" class="project-card">
      <div class="project-title">TxnShield</div>
      <span class="tech-stack">ML • STREAMLIT</span>
      <p>Credit card fraud detection system achieving 85% recall. Optimized for real-time inference with less than 50ms latency.</p>
    </a>

  </div>
</div>

<div id="contact" class="footer">
  <h2>Get In Touch</h2>
  <p>I am currently open to internship and full-time opportunities.</p>
  <div style="margin-top: 20px;">
    <a href="mailto:mihika.m185@gmail.com" class="resume-btn" style="background: #30363d;">Email Me</a>
    <a href="https://linkedin.com/in/mihika91158" class="resume-btn" style="background: #0a66c2;">LinkedIn</a>
  </div>
</div>