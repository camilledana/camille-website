<strong></strong><b></b><h1>Camille Dana</h1>
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
    
    #Handle adding a new student.
    if choice == "A":
    name = input("Enter the name of the student: ")
      if name in grades:
      print("Sorry, that student is already present.")
        else : 
        grade = input("Enter the student's grade: ")
        grades[name] = grade

    #Handle removing a student.
    elif choice == "R":
    name = input("What student do you want to remove? ")
     if name in grades:
     grades.pop(name)
     else :
     print("Sorry, that student doesn't exist and couldn't be removed.")

    #Handle modifying a student grade.
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

    #Handle the case of invalid input.
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

<h1>About Me</h1>
<h3>I'm Camille, a software engineering graduate student at UMGC with a B.A. in CIS and a background in Python development and IT support. I'm fascinated by AI engineering and the challenge of building systems that are intelligent, scalable, and genuinely useful to people.</h3>

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
