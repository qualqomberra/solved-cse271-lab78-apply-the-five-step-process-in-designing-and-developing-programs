Download Link: https://assignmentchef.com/product/solved-cse271-lab78-apply-the-five-step-process-in-designing-and-developing-programs
<br>
For this two-part lab, we are going to apply the five-step process we learned in class to help us design and develop programs:

<ol>

 <li>Gather requirements.</li>

 <li>Use CRC cards to find classes, responsibilities, and collaborators.</li>

 <li>Use UML diagrams to record class relationships.</li>

 <li>Use javadoc to document method behavior.</li>

 <li>Implement your program.</li>

</ol>

We are going to step through this process for a very small and simple use case.    In order to guide you through the process, you can follow through and emulate Section 12.3 in the textbook, which does the exact same thing, but for printing an Invoice.

<span style="font-size: 2.61792em;letter-spacing: -1px">Part 1 – Requirements </span>

(You only need to design and implement what is necessary to achieve the following set of requirements)

We are going to build a very simple course registration system.  A Course has assigned to it 1 Instructor and 1 LectureHall. A Course can have many registered Students. A LectureHall has a capacity, meaning how many students it can hold, and a name/identifier. Students, Instructors, and AdminStaff are all People belonging to the University, and all People have an ID# and an email address.  In addition, Students have a major, a list of Courses they are taking, and a single final cumulative semester GPA.  Instructors and AdminStaff have a salary.  An AdminStaff must be able to (have methods that) 1) enroll a single Student in a Course, 2) assign a Course a LectureHall, and 3) assign a Course an Instructor.  Instructors must have the ability(methods) to 1) assign/change each Student’s single final cumulative semester GPA and 2) retrieve a list of courses they are teaching (that they have been assigned).

In the interest of simplicity, we do not provide a user interface (except for bonus below). Just provide a test program that tests each of the functions/operations applied above.

For the 5 points in part 1, you must list

<ol>

 <li>All the nouns in these requirements, representing candidate classes.</li>

 <li>All the verbs.</li>

</ol>

Save this information as PDF file called Part1.pdf

Part 2 – CRC Cards

As we did in class, discover and identify classes and create CRC cards including classes, responsibilities, and collaborators.   You can/should also follow Section 12.3.2 from the textbook. Make sure to include all appropriate responsibilities and their collaborators.   Also remember that as you discover responsibilities, you may need to add other responsibilities to other classes. A reminder that you do not need to include getters and setters, but can if you think it is integral to that class.

You can create your CRC Cards as tables in word or any other electronic file format you wish.   Save it as a PDF called Part2.pdf

Part 3 – UML Class Diagrams

After you have discovered classes and their relationships with CRC cards, you should record your findings in a UML diagram. The dependency relationships come from the collaboration column on the CRC cards. Each class depends on the classes with which it collaborates.  Ensure you use all appropriate UML relationships that we have taught in class from our selection of 4 relationships.  Follow Section 12.3.3 from the textbook as an example.

You can submit your UML Class diagrams in any electronic format you wish. There are many online UML tools you can use/download for free including ArgoUML, which is fairly popular and easy to use, and <u><a href="https://www.draw.io/">https://www.draw.io/</a></u> tool, which a lot of students have enjoyed in the past.   You could also just draw it by hand and scan it in, ensuring it is legible.

You are allowed to use/create the simplistic UML diagrams we went over in class, or the more complicated full versions you may find online and in advanced courses.

Part 4 – Javadoc

The final step of the design phase is to write the documentation of the discovered classes and methods. Simply write a Java source file for each class, write the method comments for those methods that you have discovered, and leave the bodies of the methods blank until Part 5.  REMEMBER TO USE PACKAGES as we discussed in class (edu.miamioh.<em>yourUserID</em>)!  Then, use Javadoc comments to record the behavior of the classes.

Look at Section 12.3.4 for an example.  You can also search online for tons of resources like <u><a href="https://www.youtube.com/watch?v=Hx-8BD_Osdw">https://www.youtube.com/watch?v=Hx</a><a href="https://www.youtube.com/watch?v=Hx-8BD_Osdw">–</a><a href="https://www.youtube.com/watch?v=Hx-8BD_Osdw">8BD_Osdw</a></u> .

Javadoc is in the form of

/**

Overall method comments

@param param1 Description of parameter 1

@param paramn Description of parameter 2

@return Description of what is returned

*/

Public int myMethod (int param1, String param2){

…

Proper Javadoc in your code is worth 10 points.  We will be looking very closely at it.

Part 5 – Implementation (Lab 8 – 20 Points)

After you have completed the object-oriented design, you are ready to implement the classes.  You already have the method parameter variables and comments from the previous step. Now look at the UML diagram to add instance variables. Aggregated classes prescribe the use of instance variables, which can be collections or individual objects.

Follow all the implementation rules and standards we have been following thus far.  For testing, make an additional tester class program that runs through and tests (Actual versus expected/4 step process) for all functions/operations designed and implemented above.  This includes checking that things were added to the appropriate lists.

Part 6 – Bonus

Create a Graphical User Interface (GUI) for your course registration system.  If you need to learn or review GUIs, read Chapter 10 in the text book.   There are no real requirements here except that the GUI utilizes the classes you developed.  Points here will be given based on how many features and how well laid out your GUI is.  It is bonus because you will have to read ahead and learn some skills on your own. So, do not feel pressured to do it, but it will help you with future material to come.

Tips

Often times, you can think of your collaborators for each responsibility as “method parameters”. For example, in order to enroll a student in a course, I’ll need a method that takes in both a student and a course.

A reminder, class names are singular as they describe a set of individual things.  So, it would be “Person” and not “People”, and “Student” not “Students”.