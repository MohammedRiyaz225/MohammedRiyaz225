<div align="center" style="background: linear-gradient(135deg, #030b1a 0%, #071529 25%, #0c1833 65%, #120d2d 100%); border: 1px solid rgba(103, 190, 255, 0.7); border-radius: 28px; padding: 24px 30px; box-shadow: 0 24px 60px rgba(5, 15, 30, 0.7);">
  <style>
    .app-shell {
      max-width: 1200px;
      margin: 0 auto;
      font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    }

    .intro-wrap {
      display: flex;
      align-items: center;
      justify-content: center;
      gap: 28px;
      flex-wrap: wrap;
      animation: fadeUp 0.9s ease both;
    }

    .intro-copy {
      flex: 1;
      min-width: 260px;
      text-align: center;
    }

    .brand-name {
      margin: 0;
      font-size: 58px;
      line-height: 0.95;
      color: #f2edf9;
      font-weight: 700;
      font-family: Georgia, 'Times New Roman', serif;
      letter-spacing: 1px;
      text-shadow: 0 0 18px rgba(140, 120, 255, 0.22);
    }

    .gradient-text {
      background: linear-gradient(90deg, #7BFFEA, #8EB6FF, #F48DFF);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
      animation: gradientShift 4s ease infinite;
      background-size: 200% 200%;
    }

    .tagline {
      margin: 18px 0 8px;
      font-size: 30px;
      font-weight: 700;
      background: linear-gradient(90deg, #7BFFEA, #8EB6FF, #F48DFF);
      -webkit-background-clip: text;
      background-clip: text;
      color: transparent;
    }

    .subtitle {
      margin: 0;
      font-size: 22px;
      color: #d4ebff;
      font-weight: 500;
      font-family: Georgia, serif;
      font-style: italic;
      white-space: nowrap;
      overflow: hidden;
      border-right: 2px solid rgba(255,255,255,0.8);
      width: 0;
      animation: typing 3.1s steps(36, end) 0.4s forwards, blink 0.9s step-end infinite 3.5s;
    }

    .tech-badges {
      margin-top: 22px;
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
    }

    .tech-badges img,
    .pill,
    .project-card,
    .mini-link {
      transition: transform 0.2s ease, box-shadow 0.2s ease, border-color 0.2s ease;
    }

    .tech-badges img:hover,
    .pill:hover,
    .mini-link:hover {
      transform: translateY(-3px);
    }

    .motto-box {
      width: 18%;
      min-width: 120px;
      text-align: right;
      padding-top: 12px;
    }

    .motto {
      display: flex;
      flex-direction: column;
      gap: 12px;
      align-items: flex-end;
      padding: 8px 14px;
      border-radius: 14px;
      border: 1px solid rgba(78,200,255,0.8);
      background: rgba(20,44,74,0.9);
      color: #b0e6ff;
      font-weight: 700;
      font-size: 15px;
      font-style: italic;
      box-shadow: 0 12px 28px rgba(60, 160, 255, 0.12);
      animation: floatY 5s ease-in-out infinite;
    }

    .quick-pills {
      display: flex;
      justify-content: center;
      gap: 10px;
      flex-wrap: wrap;
      margin-top: 18px;
    }

    .pill {
      display: inline-block;
      background: rgba(17, 38, 54, 0.75);
      border: 1px solid rgba(80, 194, 255, 0.8);
      color: #dffcff;
      border-radius: 999px;
      padding: 9px 14px;
      font-size: 12px;
      font-weight: 600;
      letter-spacing: 0.3px;
    }

    .feature-card {
      background: linear-gradient(180deg, rgba(8, 14, 28, 0.9), rgba(9, 21, 31, 0.92));
      border: 1px solid rgba(80,194,255,0.8);
      border-radius: 22px;
      padding: 18px 16px 10px;
      box-shadow: inset 0 0 18px rgba(98, 208, 255, 0.08);
    }

    .project-grid {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
      gap: 18px;
      margin-top: 16px;
    }

    .project-card {
      background: linear-gradient(180deg, rgba(10, 22, 32, 0.92), rgba(9, 18, 30, 0.96));
      border: 1px solid rgba(90, 200, 255, 0.62);
      border-radius: 18px;
      padding: 18px;
      text-align: left;
      box-shadow: rgba(93, 196, 255, 0.08) 0px 12px 24px;
    }

    .project-card:hover {
      transform: translateY(-6px);
      border-color: rgba(140, 219, 255, 0.85);
      box-shadow: rgba(93, 196, 255, 0.18) 0px 18px 28px;
    }

    .project-head {
      display: flex;
      align-items: center;
      justify-content: space-between;
      gap: 10px;
      margin-bottom: 12px;
    }

    .project-title {
      margin: 0;
      color: #ecf9ff;
      font-size: 22px;
      font-weight: 700;
    }

    .project-badge {
      font-size: 12px;
      color: #98e2ff;
      background: rgba(18, 62, 86, 0.9);
      border: 1px solid rgba(89, 201, 255, 0.6);
      border-radius: 999px;
      padding: 4px 10px;
      white-space: nowrap;
    }

    .project-card p {
      color: #d6ebff;
      line-height: 1.65;
      font-size: 14px;
      margin: 0 0 14px;
    }

    .tech-stack {
      display: flex;
      gap: 8px;
      flex-wrap: wrap;
      margin-bottom: 16px;
    }

    .tech-stack span {
      background: rgba(22, 48, 64, 0.9);
      border: 1px solid rgba(74, 189, 255, 0.5);
      color: #bfeaff;
      border-radius: 999px;
      padding: 5px 8px;
      font-size: 11px;
      font-weight: 600;
    }

    .project-links {
      display: flex;
      justify-content: space-between;
      align-items: center;
      gap: 12px;
      margin-top: 10px;
    }

    .mini-link {
      padding: 8px 12px;
      border-radius: 10px;
      text-decoration: none;
      font-weight: 700;
      font-size: 12px;
      border: 1px solid rgba(93, 196, 255, 0.7);
      background: rgba(15, 38, 54, 0.9);
      color: #dff8ff;
    }

    .mini-link.primary {
      background: linear-gradient(90deg, rgba(21, 92, 122, 0.9), rgba(51, 160, 192, 0.9));
    }

    .section-title {
      display: flex;
      align-items: center;
      gap: 10px;
      margin: 0 0 18px;
      color: #eaf7ff;
      font-size: 28px;
      font-weight: 700;
    }

    .profile-card {
      background: linear-gradient(180deg, rgba(8, 14, 28, 0.94), rgba(10, 24, 36, 0.92));
      border: 1px solid rgba(80, 194, 255, 0.8);
      border-radius: 20px;
      box-shadow: inset 0 0 18px rgba(82, 203, 255, 0.06);
      padding: 18px 16px 16px;
      min-width: 260px;
    }

    .profile-name {
      margin: 18px 0 8px;
      color: #dffaff;
      font-size: 28px;
      text-align: center;
      font-weight: 700;
    }

    .profile-handle {
      margin: 0;
      color: #7fe4ff;
      text-align: center;
      font-size: 18px;
      font-weight: 600;
    }

    .profile-bio {
      margin: 18px 0 14px;
      font-size: 15px;
      line-height: 1.6;
      color: #d9ebff;
      text-align: center;
    }

    .info-list {
      margin-top: 20px;
      padding-top: 10px;
      border-top: 1px solid rgba(88, 163, 255, 0.3);
    }

    .info-list p {
      margin: 8px 0;
      color: #d6efff;
      font-size: 14px;
    }

    .quote-box {
      margin-top: 18px;
      background: rgba(11, 26, 38, 0.8);
      border: 1px solid rgba(77,193,255,0.5);
      border-radius: 16px;
      padding: 14px;
    }

    .quote-box p {
      margin: 0;
      color: #f3f9ff;
      font-size: 18px;
      font-weight: 700;
      font-style: italic;
    }

    @keyframes fadeUp {
      from { opacity: 0; transform: translateY(12px); }
      to { opacity: 1; transform: translateY(0); }
    }

    @keyframes floatY {
      0%, 100% { transform: translateY(0); }
      50% { transform: translateY(-8px); }
    }

    @keyframes gradientShift {
      0% { background-position: 0% 50%; }
      50% { background-position: 100% 50%; }
      100% { background-position: 0% 50%; }
    }

    @keyframes typing {
      from { width: 0; }
      to { width: 100%; }
    }

    @keyframes blink {
      50% { border-color: transparent; }
    }

    @media (max-width: 700px) {
      .brand-name { font-size: 42px; }
      .tagline { font-size: 22px; }
      .subtitle { font-size: 16px; }
      .motto-box { width: 100%; text-align: center; }
      .motto { align-items: center; }
      .section-title { font-size: 24px; }
    }
  </style>

  <div class="app-shell">
    <div class="intro-wrap">
      <div class="intro-copy">
        <h1 class="brand-name">
          <span style="font-style:italic; color:#f9d4ff;">Mohammed</span>
          <span style="font-style:italic; color:#7ae3ff;">Riyaz</span>
          <span style="font-size:52px; color:#f8d8ff;">225</span>
        </h1>
        <h2 class="tagline gradient-text">Full-Stack Developer</h2>
        <p class="subtitle">Turning Ideas into Real-World Solutions</p>
        <div class="tech-badges">
          <img alt="Python" src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" />
          <img alt="JavaScript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
          <img alt="Java" src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" />
          <img alt="SQL" src="https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" />
          <img alt="PHP" src="https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white" />
          <img alt="React" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />
          <img alt="Node.js" src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
        </div>
      </div>

      <div class="motto-box">
        <div class="motto">
          Better<br />Code<br />Bigger<br />Dreams
        </div>
      </div>
    </div>
  </div>
</div>

<div class="quick-pills" align="center">
  <span class="pill">Overview</span>
  <span class="pill">Repositories</span>
  <span class="pill">Projects</span>
  <span class="pill">Achievements</span>
  <span class="pill">Stars</span>
</div>

<table width="100%" cellpadding="18" cellspacing="0" style="margin-top:20px; border-spacing: 18px;">
  <tr valign="top">
    <td width="28%">
      <div class="profile-card">
        <div align="center">
          <img src="https://avatars.githubusercontent.com/u/111334618?v=4" width="150" height="150" alt="Mohammed Riyaz" style="border-radius:50%; border:3px solid #4dc1ff; box-shadow:0 0 24px rgba(77,193,255,0.38);" />
        </div>
        <h3 class="profile-name">Mohammed Riyaz</h3>
        <p class="profile-handle">@MohammedRiyaz225</p>
        <p class="profile-bio">
          Passionate Full-Stack Developer building web applications, exploring AI, and turning ideas into real-world solutions.
        </p>
        <div style="display:flex; justify-content:center; gap:12px; flex-wrap:wrap; margin:16px 0;">
          <span class="pill" style="padding: 8px 12px; font-size: 12px; background: rgba(25, 70, 108, 0.9); border-color: rgba(80,198,255,0.8);">India</span>
          <span class="pill" style="padding: 8px 12px; font-size: 12px; background: rgba(25, 70, 108, 0.9); border-color: rgba(80,198,255,0.8);">B.Tech (L.E.) CSE</span>
        </div>
        <div class="info-list">
          <p>📍 India</p>
          <p>📧 <a href="mailto:riyazmohammed225@gmail.com" style="color:#7ae3ff; text-decoration:none;">riyazmohammed225@gmail.com</a></p>
          <p>🔗 <a href="https://github.com/MohammedRiyaz225" style="color:#7ae3ff; text-decoration:none;">github.com/MohammedRiyaz225</a></p>
          <p>💼 <a href="https://linkedin.com/in/mohammed-riyaz-225" style="color:#7ae3ff; text-decoration:none;">linkedin.com/in/mohammed-riyaz-225</a></p>
        </div>
        <div class="quote-box">
          <p>Every line of code is a step towards my dream career.</p>
        </div>
      </div>
    </td>

    <td width="72%">
      <div class="feature-card">
        <h3 class="section-title">
          <span style="font-size:26px;">✨</span> Featured Projects
        </h3>
        <p style="margin:-6px 0 18px; color:#9ec9e9; font-size:16px;">Projects that blend product thinking, AI, and real-world problem solving.</p>

        <div class="project-grid">
          <div class="project-card">
            <div class="project-head">
              <h4 class="project-title">Focus-Lens</h4>
              <span class="project-badge">AI + Vision</span>
            </div>
            <p>Privacy-preserving productivity app using webcam-based attention analysis to detect distraction and gently adapt focus feedback.</p>
            <div class="tech-stack">
              <span>TypeScript</span>
              <span>React</span>
              <span>AI</span>
            </div>
            <div class="project-links">
              <a class="mini-link primary" href="https://github.com/MohammedRiyaz225/Focus-Lens" target="_blank" rel="noreferrer">View Repo</a>
              <a class="mini-link" href="https://github.com/MohammedRiyaz225/Focus-Lens" target="_blank" rel="noreferrer">Live Demo</a>
            </div>
          </div>

          <div class="project-card">
            <div class="project-head">
              <h4 class="project-title">Medication Reminder Agent</h4>
              <span class="project-badge">Healthcare</span>
            </div>
            <p>Smart medication adherence solution focused on non-compliance detection, reminder workflows, and patient-centric health tracking.</p>
            <div class="tech-stack">
              <span>Python</span>
              <span>AI Agents</span>
              <span>Healthcare</span>
            </div>
            <div class="project-links">
              <a class="mini-link primary" href="https://github.com/MohammedRiyaz225/Medication-Reminder-Agent" target="_blank" rel="noreferrer">View Repo</a>
              <a class="mini-link" href="https://github.com/MohammedRiyaz225/Medication-Reminder-Agent" target="_blank" rel="noreferrer">Explore</a>
            </div>
          </div>

          <div class="project-card">
            <div class="project-head">
              <h4 class="project-title">Event Booking System</h4>
              <span class="project-badge">Laravel</span>
            </div>
            <p>Modern event management platform with ticket booking, payment handling, attendance tracking, and responsive admin workflows.</p>
            <div class="tech-stack">
              <span>PHP</span>
              <span>Laravel</span>
              <span>MySQL</span>
            </div>
            <div class="project-links">
              <a class="mini-link primary" href="https://github.com/MohammedRiyaz225/EVENT-BOOKING-SYSTEM-EBS-" target="_blank" rel="noreferrer">View Repo</a>
              <a class="mini-link" href="https://github.com/MohammedRiyaz225/EVENT-BOOKING-SYSTEM-EBS-" target="_blank" rel="noreferrer">Details</a>
            </div>
          </div>

          <div class="project-card">
            <div class="project-head">
              <h4 class="project-title">Travel Safety Bot</h4>
              <span class="project-badge">Automation</span>
            </div>
            <p>Travel-focused safety solution built to provide guidance, support, and contextual assistance for safer journeys and emergency preparedness.</p>
            <div class="tech-stack">
              <span>Python</span>
              <span>Bot</span>
              <span>Automation</span>
            </div>
            <div class="project-links">
              <a class="mini-link primary" href="https://github.com/MohammedRiyaz225/Travel-Safety-Bot" target="_blank" rel="noreferrer">View Repo</a>
              <a class="mini-link" href="https://github.com/MohammedRiyaz225/Travel-Safety-Bot" target="_blank" rel="noreferrer">Read More</a>
            </div>
          </div>

          <div class="project-card">
            <div class="project-head">
              <h4 class="project-title">AI Chat</h4>
              <span class="project-badge">App</span>
            </div>
            <p>Conversational AI application exploring user-centered chat workflows, modern interfaces, and intelligent assistant experiences.</p>
            <div class="tech-stack">
              <span>Kotlin</span>
              <span>AI</span>
              <span>Mobile</span>
            </div>
            <div class="project-links">
              <a class="mini-link primary" href="https://github.com/MohammedRiyaz225/AI-Chat" target="_blank" rel="noreferrer">View Repo</a>
              <a class="mini-link" href="https://github.com/MohammedRiyaz225/AI-Chat" target="_blank" rel="noreferrer">Explore</a>
            </div>
          </div>

          <div class="project-card">
            <div class="project-head">
              <h4 class="project-title">MEDI-</h4>
              <span class="project-badge">Inventory</span>
            </div>
            <p>Smart inventory and expiry tracking system focused on efficient medication stock management and product lifecycle visibility.</p>
            <div class="tech-stack">
              <span>Python</span>
              <span>Inventory</span>
              <span>Analytics</span>
            </div>
            <div class="project-links">
              <a class="mini-link primary" href="https://github.com/MohammedRiyaz225/MEDI-" target="_blank" rel="noreferrer">View Repo</a>
              <a class="mini-link" href="https://github.com/MohammedRiyaz225/MEDI-" target="_blank" rel="noreferrer">Explore</a>
            </div>
          </div>
        </div>
      </div>
    </td>
  </tr>
</table>

<div align="center" style="margin: 28px 0 12px; color:#ccf2ff; font-weight:700; font-size: 18px; font-style: italic;">
  Built with <span style="color:#ff4d8d;">❤</span> by Mohammed Riyaz
</div>
