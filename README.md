<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Camille Dana | Software Engineer</title>
    <style>
      :root {
        --bg: #0b1020;
        --bg-soft: #121a2b;
        --card: #ffffff;
        --card-alt: #f4f7fb;
        --text: #1a2433;
        --muted: #586579;
        --primary: #2563eb;
        --primary-dark: #1d4ed8;
        --accent: #14b8a6;
        --border: #dfe7f1;
        --shadow: 0 10px 30px rgba(15, 23, 42, 0.12);
      }

      * {
        box-sizing: border-box;
      }

      html {
        scroll-behavior: smooth;
      }

      body {
        margin: 0;
        font-family: Arial, Helvetica, sans-serif;
        background: #f5f7fb;
        color: var(--text);
        line-height: 1.6;
      }

      a {
        text-decoration: none;
        color: inherit;
      }

      img {
        max-width: 100%;
      }

      .container {
        width: min(1100px, calc(100% - 32px));
        margin: 0 auto;
      }

      .navbar {
        background: rgba(11, 16, 32, 0.96);
        position: sticky;
        top: 0;
        z-index: 1000;
        backdrop-filter: blur(8px);
      }

      .nav-container {
        width: min(1100px, calc(100% - 32px));
        margin: 0 auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        min-height: 70px;
      }

      .nav-logo {
        color: #fff;
        font-weight: 700;
        letter-spacing: 0.04em;
        font-size: 1.05rem;
      }

      .nav-links {
        display: flex;
        flex-wrap: wrap;
        list-style: none;
        gap: 20px;
        margin: 0;
        padding: 0;
      }

      .nav-links a {
        color: #dfe7f4;
        font-size: 0.95rem;
        transition: color 0.2s ease;
      }

      .nav-links a:hover {
        color: #fff;
      }

      .hero {
        background: linear-gradient(135deg, #0b1020 0%, #14213d 42%, #1f3a5f 100%);
        color: #fff;
        padding: 110px 0 90px;
      }

      .hero-content {
        display: grid;
        grid-template-columns: 1.2fr 0.8fr;
        gap: 32px;
        align-items: center;
      }

      .eyebrow {
        display: inline-block;
        margin-bottom: 14px;
        background: rgba(20, 184, 166, 0.15);
        border: 1px solid rgba(20, 184, 166, 0.35);
        color: #7ef0df;
        padding: 7px 12px;
        border-radius: 999px;
        font-size: 0.82rem;
        letter-spacing: 0.06em;
        text-transform: uppercase;
        font-weight: 700;
      }

      h1 {
        font-size: clamp(2.5rem, 5vw, 4.5rem);
        line-height: 1.05;
        margin: 0 0 16px;
      }

      .hero h2 {
        font-size: clamp(1.2rem, 2vw, 1.8rem);
        line-height: 1.4;
        margin: 0 0 18px;
        color: #dbe8ff;
      }

      .hero p {
        max-width: 620px;
        margin: 0 0 28px;
        color: #dce5f6;
        font-size: 1.05rem;
      }

      .hero-actions {
        display: flex;
        flex-wrap: wrap;
        gap: 16px;
      }

      .btn {
        display: inline-flex;
        align-items: center;
        justify-content: center;
        padding: 14px 24px;
        border-radius: 10px;
        font-weight: 700;
        transition: transform 0.2s ease, box-shadow 0.2s ease;
      }

      .btn:hover {
        transform: translateY(-2px);
      }

      .btn-primary {
        background: var(--primary);
        color: white;
        box-shadow: 0 10px 20px rgba(37, 99, 235, 0.28);
      }

      .btn-primary:hover {
        background: var(--primary-dark);
      }

      .btn-secondary {
        background: transparent;
        color: white;
        border: 1px solid rgba(255, 255, 255, 0.4);
      }

      .hero-card {
        background: rgba(255, 255, 255, 0.08);
        border: 1px solid rgba(255, 255, 255, 0.12);
        border-radius: 20px;
        padding: 28px;
        box-shadow: var(--shadow);
      }

      .stat-grid {
        display: grid;
        grid-template-columns: repeat(2, minmax(120px, 1fr));
        gap: 18px;
        margin-top: 18px;
      }

      .stat {
        background: rgba(255, 255, 255, 0.05);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 14px;
        padding: 16px;
      }

      .stat strong {
        display: block;
        font-size: 1.6rem;
        margin-bottom: 4px;
      }

      .stat span {
        color: #d7e3fb;
        font-size: 0.9rem;
      }

      section {
        padding: 90px 0;
      }

      .section-header {
        max-width: 760px;
        margin-bottom: 34px;
      }

      .section-header h2 {
        font-size: clamp(2rem, 4vw, 2.8rem);
        margin: 0 0 12px;
      }

      .section-header p {
        margin: 0;
        color: var(--muted);
        font-size: 1.02rem;
      }

      .about-grid {
        display: grid;
        grid-template-columns: 1.2fr 0.8fr;
        gap: 32px;
      }

      .about-card,
      .project-card,
      .experience-item,
      .skill-group,
      .education-card {
        background: var(--card);
        border: 1px solid var(--border);
        border-radius: 18px;
        box-shadow: var(--shadow);
      }

      .about-card {
        padding: 28px;
      }

      .about-card p {
        color: var(--muted);
        margin: 0 0 18px;
      }

      .about-highlights {
        display: grid;
        grid-template-columns: repeat(3, 1fr);
        gap: 18px;
        margin-top: 18px;
      }

      .highlight {
        background: var(--card-alt);
        border: 1px solid var(--border);
        border-radius: 14px;
        padding: 16px;
      }

      .highlight strong {
        display: block;
        margin-bottom: 8px;
        font-size: 1rem;
      }

      .highlight span {
        color: var(--muted);
        font-size: 0.92rem;
      }

      .profile-box {
        padding: 28px;
      }

      .profile-box h3 {
        margin-top: 0;
        font-size: 1.25rem;
      }

      .profile-list {
        list-style: none;
        padding: 0;
        margin: 18px 0 0;
      }

      .profile-list li {
        margin-bottom: 12px;
        color: var(--muted);
      }

      .experience-list {
        display: grid;
        gap: 22px;
      }

      .experience-item {
        padding: 28px;
      }

      .experience-item h3 {
        margin: 0 0 8px;
        font-size: 1.35rem;
      }

      .role {
        color: var(--primary);
        font-weight: 700;
        margin: 0 0 10px;
      }

      .date {
        color: var(--muted);
        margin: 0 0 10px;
      }

      .experience-item ul {
        margin: 0;
        padding-left: 18px;
        color: var(--muted);
      }

      .experience-item li + li {
        margin-top: 8px;
      }

      .projects-grid {
        display: grid;
        grid-template-columns: repeat(3, minmax(0, 1fr));
        gap: 24px;
      }

      .project-card {
        padding: 24px;
        display: flex;
        flex-direction: column;
      }

      .project-card h3 {
        margin-top: 0;
        font-size: 1.35rem;
      }

      .project-card p {
        color: var(--muted);
        margin: 0 0 16px;
      }

      .project-tag {
        display: inline-block;
        padding: 6px 10px;
        border-radius: 999px;
        background: #e0f2fe;
        color: #0f4d8d;
        font-weight: 700;
        font-size: 0.76rem;
        letter-spacing: 0.04em;
        text-transform: uppercase;
        margin-bottom: 12px;
      }

      .project-links {
        margin-top: auto;
      }

      .project-links a {
        color: var(--primary);
        font-weight: 700;
      }

      .skills-grid {
        display: grid;
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 24px;
      }

      .skill-group {
        padding: 24px;
      }

      .skill-group h3 {
        margin-top: 0;
        margin-bottom: 14px;
      }

      .skill-pills {
        display: flex;
        flex-wrap: wrap;
        gap: 10px;
      }

      .skill-pills span {
        background: var(--card-alt);
        border: 1px solid var(--border);
        border-radius: 999px;
        padding: 8px 12px;
        font-size: 0.92rem;
        color: var(--text);
      }

      .education-grid {
        display: grid;
        grid-template-columns: repeat(2, minmax(0, 1fr));
        gap: 24px;
      }

      .education-card {
        padding: 24px;
      }

      .education-card h3 {
        margin-top: 0;
      }

      .education-card p {
        color: var(--muted);
        margin: 0;
      }

      .contact {
        background: #0b1020;
        color: white;
      }

      .contact-box {
        background: rgba(255, 255, 255, 0.04);
        border: 1px solid rgba(255, 255, 255, 0.1);
        border-radius: 20px;
        padding: 32px;
      }

      .contact-box p {
        color: #dfe8f8;
        margin: 0 0 20px;
      }

      .contact-links {
        display: flex;
        flex-wrap: wrap;
        gap: 16px;
      }

      .contact-links a {
        color: white;
        background: rgba(255, 255, 255, 0.06);
        padding: 12px 18px;
        border-radius: 10px;
        border: 1px solid rgba(255, 255, 255, 0.12);
        font-weight: 700;
      }
      <div class="contact-links">
  <a href="https://github.com/camilledana" target="_blank" rel="noopener noreferrer">
    GitHub
  </a>
  <a href="https://linkedin.com/in/camilledana" target="_blank" rel="noopener noreferrer" class="icon-btn">
    <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" aria-hidden="true">
      <path d="M20.45 20.45h-3.55v-5.57c0-1.33-.02-3.04-1.85-3.04-1.86 0-2.14 1.45-2.14 2.94v5.67H9.35V9h3.41v1.56h.05c.48-.9 1.64-1.85 3.37-1.85 3.6 0 4.27 2.37 4.27 5.46v6.28zM5.34 7.43a2.06 2.06 0 1 1 0-4.12 2.06 2.06 0 0 1 0 4.12zM7.12 20.45H3.56V9h3.56v11.45zM22.22 0H1.77C.79 0 0 .77 0 1.72v20.56C0 23.23.79 24 1.77 24h20.45c.98 0 1.78-.77 1.78-1.72V1.72C24 .77 23.2 0 22.22 0z"/>
    </svg>
    LinkedIn
  </a>
  <a href="mailto:camilledana@gmail.com">Email</a>
</div>

      @media (max-width: 860px) {
        .hero-content,
        .about-grid,
        .projects-grid,
        .skills-grid,
        .education-grid {
          grid-template-columns: 1fr;
        }

        .nav-container {
          flex-direction: column;
          justify-content: center;
          padding: 12px 0;
        }

        .nav-links {
          justify-content: center;
          padding-bottom: 10px;
        }

        .hero {
          padding-top: 80px;
        }
      }
    </style>
  </head>
  <body>
    <nav class="navbar">
      <div class="nav-container">
        <a href="#home" class="nav-logo">CAMILLE DANA</a>
        <ul class="nav-links">
          <li><a href="#about">About</a></li>
          <li><a href="#experience">Experience</a></li>
          <li><a href="#projects">Projects</a></li>
          <li><a href="#skills">Skills</a></li>
          <li><a href="#education">Education</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </div>
    </nav>

    <header id="home" class="hero">
      <div class="container hero-content">
        <div>
          <span class="eyebrow">Software Engineer</span>
          <h1>Camille Dana</h1>
          <h2>Building reliable systems and AI-native experiences.</h2>
          <p>
            I’m a software engineer and graduate student passionate about
            backend systems, cloud architecture, artificial intelligence, and
            building products that solve real-world problems.
          </p>

          <div class="hero-actions">
            <a href="#projects" class="btn btn-primary">View Work</a>
            <a href="#contact" class="btn btn-secondary">Contact Me</a>
          </div>
        </div>

        <div class="hero-card">
          <h3>Core Focus</h3>
          <div class="stat-grid">
            <div class="stat">
              <strong>5+</strong>
              <span>Years Learning & Building</span>
            </div>
            <div class="stat">
              <strong>Java</strong>
              <span>Backend & OOP</span>
            </div>
            <div class="stat">
              <strong>Python</strong>
              <span>Automation & Analysis</span>
            </div>
            <div class="stat">
              <strong>AWS</strong>
              <span>Cloud & APIs</span>
            </div>
          </div>
        </div>
      </div>
    </header>

    <main>
      <section id="about">
        <div class="container">
          <div class="section-header">
            <h2>About Me</h2>
            <p>
              I enjoy designing software that is practical, scalable, and
              meaningful — from backend services to AI-enabled solutions.
            </p>
          </div>

          <div class="about-grid">
            <div class="about-card">
              <p>
                I’m Camille Dana, a software engineering graduate student and
                computer information systems graduate with experience in software
                development, Python, databases, and IT support. I enjoy exploring
                how software, AI, and business strategy intersect to create
                meaningful digital experiences.
              </p>

              <p>
                My work combines engineering fundamentals with modern tools and
                practices, including object-oriented design, REST APIs, cloud
                platforms, and collaborative development workflows.
              </p>

              <div class="about-highlights">
                <div class="highlight">
                  <strong>Languages</strong>
                  <span>Java, Python, SQL, JavaScript, HTML, CSS</span>
                </div>
                <div class="highlight">
                  <strong>Cloud</strong>
                  <span>AWS, Docker, GitHub, Dev workflows</span>
                </div>
                <div class="highlight">
                  <strong>Focus</strong>
                  <span>AI, backend, architecture, software quality</span>
                </div>
              </div>
            </div>

            <div class="about-card profile-box">
              <h3>Profile</h3>
              <ul class="profile-list">
                <li><strong>Education:</strong> MS in Software Engineering (UMGC)</li>
                <li><strong>Degree:</strong> BS in Computer Information Systems</li>
                <li><strong>Interests:</strong> AI-native systems, cloud, automation</li>
                <li><strong>Goal:</strong> Build purpose-driven technology solutions</li>
              </ul>
            </div>
          </div>
        </div>
      </section>

      <section id="experience">
        <div class="container">
          <div class="section-header">
            <h2>Experience</h2>
            <p>Professional and academic experience in engineering, software delivery, and technical support.</p>
          </div>

          <div class="experience-list">
            <article class="experience-item">
              <h3>University of Maryland Global Campus</h3>
              <p class="role">Software Engineering Graduate Student</p>
              <p class="date">2025 – Present</p>
              <ul>
                <li>Studying modern software engineering and architecture practices.</li>
                <li>Exploring AI systems, distributed design, and software lifecycle methods.</li>
                <li>Applying object-oriented design and technical problem-solving in coursework.</li>
              </ul>
            </article>

            <article class="experience-item">
              <h3>California State University, Stanislaus</h3>
              <p class="role">Python Developer Student Projects</p>
              <p class="date">January 2018 – June 2024</p>
              <ul>
                <li>Built Python applications to solve technical and business problems.</li>
                <li>Worked with data structures, database concepts, and software fundamentals.</li>
                <li>Created practical projects using OOP, logic design, and user interaction.</li>
              </ul>
            </article>

            <article class="experience-item">
              <h3>Denair Unified School District</h3>
              <p class="role">IT Support Assistant</p>
              <p class="date">January 2019 – November 2019</p>
              <ul>
                <li>Provided technical support to faculty and staff.</li>
                <li>Maintained labs, systems, and software configurations.</li>
                <li>Diagnosed hardware and software issues while documenting fixes.</li>
              </ul>
            </article>
          </div>
        </div>
      </section>

      <section id="projects">
        <div class="container">
          <div class="section-header">
            <h2>Featured Projects</h2>
            <p>Selected work spanning software engineering, application design, and product development.</p>
          </div>

          <div class="projects-grid">
            <article class="project-card">
              <span class="project-tag">Java</span>
              <h3>Hotel Management System</h3>
              <p>
                An object-oriented Java application for room management, customer
                tracking, reservations, and validation.
              </p>
              <div class="project-links">
                <a href="https://github.com/camilledana/hotel-management-system" target="_blank" rel="noopener noreferrer">
                  View Repository →
                </a>
              </div>
            </article>

            <article class="project-card">
              <span class="project-tag">Web</span>
              <h3>Personal Portfolio Website</h3>
              <p>
                A responsive portfolio site built to showcase technical projects,
                skills, and professional growth in a polished user experience.
              </p>
              <div class="project-links">
                <a href="https://github.com/camilledana/camille-website" target="_blank" rel="noopener noreferrer">
                  View Repository →
                </a>
              </div>
            </article>

            <article class="project-card">
              <span class="project-tag">Python</span>
              <h3>Employee Gross Wage Calculator</h3>
              <p>
                A Python app that calculates gross pay with overtime logic and
                validates user-entered values for accurate payroll results.
              </p>
              <div class="project-links">
                <a href="#work">See Example →</a>
              </div>
            </article>
          </div>
        </div>
      </section>

      <section id="skills">
        <div class="container">
          <div class="section-header">
            <h2>Technical Skills</h2>
            <p>Tools, languages, and technologies I use to design and build software solutions.</p>
          </div>

          <div class="skills-grid">
            <div class="skill-group">
              <h3>Languages</h3>
              <div class="skill-pills">
                <span>Java</span>
                <span>Python</span>
                <span>SQL</span>
                <span>JavaScript</span>
                <span>HTML5</span>
                <span>CSS3</span>
                <span>C/C++</span>
              </div>
            </div>

            <div class="skill-group">
              <h3>Databases</h3>
              <div class="skill-pills">
                <span>Oracle</span>
                <span>PostgreSQL</span>
                <span>MongoDB</span>
                <span>MySQL</span>
              </div>
            </div>

            <div class="skill-group">
              <h3>Tools & Platforms</h3>
              <div class="skill-pills">
                <span>Git</span>
                <span>GitHub</span>
                <span>Docker</span>
                <span>VS Code</span>
                <span>IntelliJ IDEA</span>
                <span>PyCharm</span>
                <span>Postman</span>
              </div>
            </div>

            <div class="skill-group">
              <h3>Core Engineering</h3>
              <div class="skill-pills">
                <span>AWS</span>
                <span>REST APIs</span>
                <span>Agile</span>
                <span>Scrum</span>
                <span>OOP</span>
                <span>Software Testing</span>
              </div>
            </div>
          </div>
        </div>
      </section>

      <section id="education">
        <div class="container">
          <div class="section-header">
            <h2>Education</h2>
            <p>Academic background in software engineering and information systems.</p>
          </div>

          <div class="education-grid">
            <article class="education-card">
              <h3>University of Maryland Global Campus</h3>
              <p><strong>M.S. in Software Engineering</strong></p>
              <p>Expected Graduation: 2028</p>
            </article>

            <article class="education-card">
              <h3>California State University, Stanislaus</h3>
              <p><strong>B.S. in Computer Information Systems</strong></p>
              <p>Minor in Business Administration</p>
              <p>Graduated: 2024</p>
            </article>
          </div>
        </div>
      </section>
    </main>

    <footer id="contact" class="contact">
      <div class="container">
        <div class="contact-box">
          <h2>Let’s Build Something Meaningful</h2>
          <p>
            I’m open to software engineering opportunities, collaborative
            projects, and conversations around AI, cloud systems, and product
            development.
          </p>

          <div class="contact-links">
            <a href="https://github.com/camilledana" target="_blank" rel="noopener noreferrer">GitHub</a>
            <a href="https://linkedin.com/in/camilledana" target="_blank" rel="noopener noreferrer">LinkedIn</a>
            <a href="mailto:camille@gmail.com">Email</a>
          </div>
        </div>
      </div>
    </footer>
  </body>
</html>
