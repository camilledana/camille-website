<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Camille Dana | Developer Portfolio</title>
</head>

<body>

    <!-- Navigation -->
    <nav class="navbar">
        <div class="nav-container">
            <a href="#" class="nav-logo">Developer Portfolio</a>

            <ul class="nav-links">
                <li><a href="#work">Work</a></li>
                <li><a href="#experience">Experience</a></li>
                <li><a href="#about">About Me</a></li>
                <li><a href="#speaking">Speaking</a></li>
                <li><a href="#projects">Projects</a></li>
                <li><a href="#musings">Mod Musings</a></li>
                <li><a href="#resources">Resources</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </div>
    </nav>

    <!-- Hero Section -->
    <header class="hero">
        <div class="hero-content">
            <h1>Camille Dana</h1>

            <h2>
                Software Engineer | Graduate Student |
                Building AI-Native Systems
            </h2>

            <p>
                Passionate about software engineering, artificial intelligence,
                cloud computing, backend development, and entrepreneurship.
            </p>

    <div class="hero-buttons">
        <a href="#work" class="btn">View Work</a>
        <a href="#musings" class="btn btn-secondary">Read Musings</a>
        <a href="#contact" class="btn btn-outline">Contact</a>
    </div>

    </header>

    <!-- Work Section -->
    <section id="work">
        <h2>Work & Coursework</h2>

        <article>
            <h3>Employee Gross Wage Calculator</h3>

            <p>
                Python application that calculates employee gross pay,
                including overtime compensation.
            </p>

            <h4>What I Learned</h4>
            <ul>
                <li>User input validation</li>
                <li>Conditional logic</li>
                <li>Numeric calculations</li>
                <li>Python data types</li>
            </ul>

            <pre><code>
user = input("Please enter employee name: ")

hrpay = float(input("Hourly wage in dollars: "))
hours = float(input("Hours worked per week: "))

if hours <= 40:
    basepay = round(hrpay * hours, 2)
    overtime = 0
else:
    basepay = round(40 * hrpay, 2)
    overtime = round((hours - 40) * (1.5 * hrpay), 2)

grosspay = basepay + overtime

print("Employee Name:", user)
print("Base Pay: $", basepay)
print("Overtime: $", overtime)
print("Gross Pay: $", grosspay)
            </code></pre>
        </article>

        <article>
            <h3>Student Grade Dictionary Program</h3>

            <p>
                Interactive Python application for managing student grades
                using dictionary data structures.
            </p>

            <h4>What I Learned</h4>
            <ul>
                <li>Dictionaries</li>
                <li>Loops</li>
                <li>CRUD operations</li>
                <li>User interaction</li>
            </ul>
        </article>

        <article>
            <h3>Class Tally Counter</h3>

            <p>
                Object-oriented Python project that counts and resets values.
            </p>

            <h4>What I Learned</h4>
            <ul>
                <li>Classes and Objects</li>
                <li>Methods</li>
                <li>State management</li>
                <li>Object-oriented programming principles</li>
            </ul>

            <pre><code>
def getValue(self):
    return self._value

def click(self):
    self._value += 1

def reset(self):
    self._value = 0
            </code></pre>
        </article>
    </section>

    <!-- Experience -->
    <section id="experience">
        <h2>Experience</h2>

        <p>
            Computer Information Systems graduate and Software Engineering
            graduate student with experience in software development,
            Python programming, database systems, and IT support.
        </p>

        <article>
            <h3>University of Maryland Global Campus (UMGC)</h3>

            <p>
                <strong>Software Engineering Graduate Student</strong><br>
                2025 – Present
            </p>

            <ul>
                <li>Developing advanced software engineering skills through graduate coursework.</li>
                <li>Studying software architecture, AI systems, and modern development practices.</li>
                <li>Applying object-oriented design and software lifecycle methodologies.</li>
            </ul>
        </article>

        <article>
            <h3>California State University, Stanislaus</h3>

            <p>
                <strong>Python Developer Student Projects</strong><br>
                January 2018 – June 2024
            </p>

            <ul>
                <li>Built Python applications to solve business and technical problems.</li>
                <li>Created programs using object-oriented programming principles.</li>
                <li>Worked with databases, data structures, and software development fundamentals.</li>
            </ul>
        </article>

        <article>
            <h3>Denair Unified School District</h3>

            <p>
                <strong>IT Support Assistant</strong><br>
                January 2019 – November 2019
            </p>

            <ul>
                <li>Provided technical support for faculty and staff.</li>
                <li>Maintained computer labs and software installations.</li>
                <li>Troubleshot hardware and software issues.</li>
                <li>Assisted with system maintenance and documentation.</li>
            </ul>
        </article>
    </section>

    <!-- Education -->
    <section id="education">
        <h2>Education</h2>

        <p>
            <strong>University of Maryland Global Campus</strong><br>
            Master of Science in Software Engineering<br>
            Expected Graduation: 2028
        </p>

        <p>
            <strong>California State University, Stanislaus</strong><br>
            Bachelor of Science in Computer Information Systems<br>
            Minor in Business Administration<br>
            Graduated: 2024
        </p>
    </section>

    <!-- Technical Skills -->
    <section id="skills">
        <h2>Technical Skills</h2>

        <h3>Languages</h3>
        <p>
            Java, Python, SQL, JavaScript, HTML5, CSS3, C/C++
        </p>

        <h3>Databases</h3>
        <p>
            Oracle, PostgreSQL, MongoDB, MySQL
        </p>

        <h3>Tools & Platforms</h3>
        <p>
            Git, GitHub, Docker, VS Code, IntelliJ IDEA,
            PyCharm, Jupyter Notebook, Postman
        </p>

        <h3>Cloud & Development</h3>
        <p>
            AWS, REST APIs, Agile, Scrum,
            Object-Oriented Programming, Software Testing
        </p>

        <h3>Operating Systems</h3>
        <p>
            Linux (Ubuntu), Windows, Android, iOS
        </p>
    </section>

    <!-- About -->
    <section id="about">
        <h2>About Me</h2>

        <p>
            I'm Camille Dana, a Software Engineering graduate student at
            the University of Maryland Global Campus and a Computer
            Information Systems graduate from California State University,
            Stanislaus.
        </p>

        <p>
            I enjoy building software that solves real-world problems,
            learning emerging technologies, and exploring the intersection
            of artificial intelligence, software engineering, and business.
        </p>

        <p>
            My long-term goal is to build purpose-driven technology
            solutions that create meaningful impact.
        </p>
    </section>

    <!-- Speaking -->
    <section id="speaking">
        <h2>Speaking</h2>

        <p>
            Upcoming presentations, webinars, and technical talks
            will be featured here.
        </p>
    </section>

    <!-- Projects -->
    <section id="projects">
        <h2>Featured Projects</h2>

        <div class="project-card">
            <h3>Hotel Management System</h3>

            <p>
                Object-oriented Java application featuring room
                management, reservations, customer tracking,
                and data validation.
            </p>

            <p>
                <strong>Technologies:</strong>
                Java, OOP, XML, UML
            </p>

            <a href="#">View Repository</a>
        </div>

        <div class="project-card">
            <h3>Personal Portfolio Website</h3>

            <p>
                Responsive web design project showcasing software
                engineering projects, skills, and professional growth.
            </p>

            <p>
                <strong>Technologies:</strong>
                HTML5, CSS3, JavaScript
            </p>

            <a href="#">View Repository</a>
        </div>
    </section>

    <!-- Blog -->
    <section id="musings">
        <h2>Mod Musings</h2>

        <article>
            <h3>How I Learned StarUML in Two Weeks</h3>
        </article>

        <article>
            <h3>Balancing Graduate School and Life</h3>
        </article>

        <article>
            <h3>My Journey into AI Engineering</h3>
        </article>
    </section>

    <!-- Resources -->
    <section id="resources">
        <h2>Resources</h2>

        <h3>AI Engineering</h3>

        <ul>
            <li>Anthropic Prompt Engineering Guide</li>
            <li>LangChain Documentation</li>
            <li>OpenAI Platform Documentation</li>
            <li>Hugging Face Learning Resources</li>
        </ul>

        <h3>Software Engineering</h3>

        <ul>
            <li>Oracle Documentation</li>
            <li>Spring Boot Documentation</li>
            <li>MDN Web Docs</li>
            <li>GitHub Learning Lab</li>
        </ul>
    </section>

    <!-- Footer -->
    <footer id="contact">

        <h2>Contact</h2>

        <p>Let's build something together.</p>

        <div class="social-links">
            <a href="https://github.com/camilledana">GitHub</a>
            <a href="#">LinkedIn</a>
        </div>

        <p>
           
