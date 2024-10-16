This project is a jupyter notebook that creates 3 classes and uses them together to create a mock registrar.


Excersize 1

It begins by creating a Course class which has methods to:
    - add a student to a course
    - remove a student from a course
    - show all the students in a course
This is done with if statements in each method ensuring methods are being executed appropriatley
    - ex. if the method to remove a student was executed, but the student was not in the course's student list, the method will return that the student is not enrolled


Excersize 2

Similar to the first excersze, a Student class is created with methods to:
    - enroll in a course
    - drop a course
    - show all the courses a student is enrolled in
    - optionally store the address of the student
Initially these are all of the methods necessary, but the class was enhanced to meet the requirements of following excersizes. It now also includes methods to:
    - assign a grade to a course the student is enrolled in
    - calculate the GPA of the student which is done by taking the average grade in all enrolled courses
Grades are stored in a course_grades dictionary which is utilized in Excersize 4.
Again, if statements are used to ensure moethods are being used appropriately.


Excersize 3

This excersize creates a Registrar class to utilize both the Student and Course classes together.
The Registrar class holds lists of all studens and courses in the system and has methods to:
    - add a student to the system
    - add a course to the system
    - enroll a student in a course
        - utilizes a method from the Student class to add the course to the student's list
        - utilizes a method from the Course class to add the student to the class list
    - drop a student from a course
        - utilizes a method from the Student class to remove the course to the student's list
        - utilizes a method from the Course class to remove the student to the class list
    - show all a students enrolled courses
    - show all the students enrolled in a course
These are all of the necesary methods for this class, but it contains two additional methods avoid confusion if there were an error of inconsitency between courses and students. These methods either ensure a student is in the proper list or a course in the porper list before executing a method.


Excersize 4

This excersize overwrites the Registrar class created in Excersize 3. It contains all of the same methods as the class in Ex 3, but it has two additional methods which:
    - assign a grade to a student in a specific course
        - this is done using the course_grades dictionary mentioned in Excersize 2
    - calculate a student's GPA
        - this takes the average of grades a student has been assigned again using the course_grades dictionary


When all cells are run in this notebook Excersize 1 and Excersize 2 will create the Course and Student class respectively. Excersize 4 will create the used Registrar class and Excersize 3 will have no functional value because it has been overwritten by Excersize 4.
