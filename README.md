<!DOCTYPE html>
<html lang = "en">
 <head>
    <meta charset +"UTF-8">
    <meta name = "viewport" content = width = device-width, initial-scale=
 </head>
 <title><strong></strong><b></b><h1>Camille Dana </h1></title>
 <body>
    <!--Navigation Bar-->
    <nav class = "navbar >
      <div class = "nav-container">
      <a href = "#" class="nav-logo"> DeveloperPortfolio<a/>
      <ul class = "nav-links">
        <li><a heref="#about"> About</a></li>
        <li><a heref="#skills"> Skills</a></li>
        <li><a heref="#projects"> Projects</a></li>
       <li><a heref="#contact"> Contact</a></li>
 </body>

<h2>Software Engineering Graduate Student | Building AI-Native Systems
[View Work] [Read Musings] [Contact]<h2/>
<h1>Work</h1>
 
  <h3>Employee gross wage

What I learned: ...

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
</h3>

   <h3>Use a dictionary to track student grades and loop until quit.
 
What I learned: ...
    
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

</h3>


<h3>Count a class tally with a limited number of people in Python.

 What I learned: ...
 
    def getValue(self):
    return self.value
    defClick(self):
    self._value=self._value+1
    def reset(self):
    self._value=0
</h3>

 <h2>EXPERIENCE</h2>

   Systems Engineer with 5+ years of experience in embedded systems, software platforms, and computing systems. 

   **	UMGC | Adelphi, MD 
   AWS & Microservices: Deployed serverless APIs (AWS Lambda, API Gateway) and containerized services (Docker) to handle users. Integrated RDBMS (PostgreSQL) and NoSQL    (MongoDB)...

   **California State University, Stanislaus | Turlock, CA  
   Python Developer | January 2018 – June 2024		Software Engineer| January 2024 – Present 
   High-Performance Compute (HPC), SoC Architecture, GPU/CPU Resource Allocation, Platform Lifecycle (Boot/Shutdown/OTA), Data Integrity...

   **Denair Unified School District | Denair, CA USA 
   IT Support Assistant | January 2019 – November 2019 
   Cloud-Native Data Systems; deployment and maintenance of multiple computer lab software programs...

EDUCATION 

  University of Maryland Global Campus | Adelphi, Maryland 
  Master of Science in Software Engineering / Computer Science | 2028 

  California State University of Stanislaus | Turlock, California 
  Bachelor of Science in Computer Information Systems / Business Administration | 2024 

TECHNICAL SKILLS 

  Operating Systems: Linux (Ubuntu), iOS, Android. Languages: Java, Python, C/C++, JavaScript, SQL, HTML/CSS, English (Native). Tools & Platforms: Git/GitHub, Docker,    MySQL, MongoDB, PostgreSQL, AWS (EC2, S3), Jira, Postman, Visual Studio Code, Intelli J, PyCharm, Jupyter Notebook, Matplotlib. Protocols: RESTful APIs, Agile/Scrum,   CI/CD, Unit Testing (JUnit), Data Structures, Object-Oriented Programming Frameworks and Libraries: React, Node .js, Spring Boot, Express .js, jQuery.


<h1>About Me</h1>
   I'm Camille, a software engineering graduate student at UMGC with a B.S. in CIS and a background in Python development and IT support. I'm fascinated by AI             engineering and the challenge of building systems that are intelligent, scalable, and genuinely useful to people.

<h1>Speaking</h1>
<h1>My Projects</h1>
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
