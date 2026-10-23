<!DOCTYPE html>
<html lang = "en">
 <head>
    <meta charset +"UTF-8">
    <meta name = "viewport" content = width = device-width, initial-scale=
 </head>
 <strong></strong><b></b><h1>Camille Dana </h1>
 <body>
    <!--Navigation Bar-->
    <nav class = "navbar >
      <div class = "nav-container">
      <a href = "#" class="nav-logo"> Developer Portfolio<a/>
      <ul class = "nav-links">
        <li><a heref="#work"> Work</a></li>
        <li><a heref="#about me"> About Me</a></li>
        <li><a heref="#speaking"> Speaking</a></li>
        <li><a heref="#my projects"> My Projects</a></li>
        <li><a heref="#mod musings> Mod Musings</a></li>
        <li><a heref="#resources"> Resources</a></li>
      </ul>
      </div>
      </nav>
        <!--Hero Section-->
        <header class + "hero">
           <div class = "hero-content">
              
 </body>

<h2>Software Engineering Graduate Student | Building AI-Native Systems
[View Work] [Read Musings] [Contact]<h2/>
<h1>Work</h1>
 
  <h3>Employee gross wage

What I learned: ...</h3><h2>

    user=input('Please enter employee name: ')
    hrpay=float(input('hourly wage in dollars: '))
    hrperweek=float(input('hours worked per week: '))
    if hrperweek <= 40:
    basepay= round(hrpay*hrperweek,2)
    overtime=0
    else:
    basepay=round(40*hrpay, 2)
    overtime=round((hrperweek-40)*(1.5*hrpay), 2)
    grosspay=basepay+overtime
    print("Employee Name: " + user)
    print("Base Pay: $" + str(basepay))
    print("Overtime: $" + str(overtime))
    print("Gross Pay: $" + str(grosspay))
</h2>

   <h3>Use a dictionary to track student grades and loop until quit.
 
What I learned: ...</h3><h2>
    
    grades = {}
    choice = ""
    while choice != "Q":
    choice = input("(A)dd, (R)emove, (M)odify, (P)rint all, or (Q)uit? ")
    choice = choice.upper()
    
    # Handle adding a new student.
    if choice == "A":
    name = input("Enter the name of the student: ")
      if name in grades:
      print("Sorry, that student is already present.")
        else : 
        grade = input("Enter the student's grade: ")
        grades[name] = grade

    # Handle removing a student.
    elif choice == "R":
    name = input("What student do you want to remove? ")
     if name in grades:
     grades.pop(name)
     else :
     print("Sorry, that student doesn't exist and couldn't be removed.")

    # Handle modifying a student grade.
     elif choice == "M":
     name = input("Enter the name of the student to modify: ")
     if name in grades:
     print("The old grade is", grades[name])
     grade = input("Enter the new grade: ")
     grades[name] = grade
       else :
       print("Sorry, that student doesn't exist and couldn't be modified.")

    # Handle printing all of the students.
      elif choice == "P":
      for name in sorted(grades):
         print("%s: %s" % (name, grades[name]))

    # Handle the case for quiting.
      elif choice == "Q":
      print("Goodbye!")

    # Handle the case of invalid input.
     else :
     print("Sorry, that wasn't a valid choice.")

</h2>


<h3>Count a class tally with a limited number of people in Python.

 What I learned: ...</h3><h2>
 
    def getValue(self):
    return self.value
    defClick(self):
    self._value=self._value+1
    def reset(self):
    self._value=0
</h2>

 <h2><B>EXPERIENCE</h2></B>

   <b>Systems Engineer with 5+ years of experience in embedded systems, software platforms, and computing systems.</b> 

  <em><b>UMGC </em></b> | Adelphi, MD 
  Software Engineer | <em>Now</em>
   AWS & Microservices: Deployed serverless APIs (AWS Lambda, API Gateway) and containerized services (Docker) to handle users. Integrated RDBMS (PostgreSQL) and NoSQL    (MongoDB)...

  <em><b> California State University, Stanislaus </em></b> | Turlock, CA  
   Python Developer | <em>January 2018 – June 2024</em>		Software Engineer| <em>January 2024 – Present</em> 
   High-Performance Compute (HPC), SoC Architecture, GPU/CPU Resource Allocation, Platform Lifecycle (Boot/Shutdown/OTA), Data Integrity...

  <em><b> Denair Unified School District </em></b> | Denair, CA USA 
   IT Support Assistant | <em>January 2019 – November 2019</em> 
   Cloud-Native Data Systems; deployment and maintenance of multiple computer lab software programs...

<b>EDUCATION</b> 

  <B>University of Maryland Global Campus</B> | Adelphi, Maryland 
  Master of Science in Software Engineering / <em> Computer Science </em> | 2028 

  <B>California State University of Stanislaus</b> | Turlock, California 
  Bachelor of Science in Computer Information Systems / <em> Business Administration </em> | 2024 

<b>TECHNICAL SKILLS</b>
  Operating Systems: Linux (Ubuntu), iOS, Android. Languages: Java, Python, C/C++, JavaScript, SQL, HTML/CSS, English (Native). Tools & Platforms: Git/GitHub, Docker,    MySQL, MongoDB, PostgreSQL, AWS (EC2, S3), Jira, Postman, Visual Studio Code, Intelli J, PyCharm, Jupyter Notebook, Matplotlib. Protocols: RESTful APIs, Agile/Scrum,   CI/CD, Unit Testing (JUnit), Data Structures, Object-Oriented Programming Frameworks and Libraries: React, Node .js, Spring Boot, Express .js, jQuery.


<h1>About Me</h1>
   I'm Camille, a software engineering graduate student at UMGC with a B.S. in CIS and a background in Python development and IT support. I'm fascinated by AI             engineering and the challenge of building systems that are intelligent, scalable, and genuinely useful to people.

<h1>Speaking</h1>
<h1>My Projects</h1>
<!--Projects Section-->
<section id= = "projects" class = "section alt-by">
   <h2>Featured Projects</h2>
   <div class ="projects-grid">
    <!--Project 1-->
    <div class="project-card">
      <h3>Hotel Management System</h3>
      <p>An object-oriented Java application built utilizing rigorous OOA&D design patterns, featuring custom room tracking and reservation flows.</p>
      <div class = "project-tags"><span>Java/span<span>OOP</span></div>
       <aref="#" class="project-link">View Repository --></a>
      <div>
    <!--Project 2-->
    <div class="project-card">
    <h3>Custom Web Application</h3>
     <p>A responsive front-end project engineered with semantics, accessibility, and modern layouts optimized for performance.</p>
     <div class-"project-tags"><span>HTML5</span><span> CSS3</span><span> UI Mockup</span></div>
     <a href="#"class="project-link">View Repository--></a>
    <div></div>
    </section>
      </div>
<h1>Mod Musings</h1>
<h2>"How I learned StarUML in two weeks"</h2>
<h2>"Balancing grad school and life"</h2>
<h3>Title
Date | Tags
Intro paragraph
Body (headers, code blocks, images)
Takeaway or call to action</h3>
<h1>Resources</h1>
       
<h2>AI Engineering

Anthropic's Prompt Engineering Guide — Practical guide for working with Claude and other LLMs.

LangChain Docs — Framework for building LLM-powered applications.</h2>

<!=Footer/Contact Section-->
<footer id="contact">
   <p>Let's build something together.</p>
   <div class="social-links">
   <a href="#">GitHub</a>
    
   <a href="#">LinkedIn</a>
</div>
 <p class="copyright">&copy;
</footer>
</body>
</html>

