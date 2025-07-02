UNIVERSITY STUDENT MANAGEMENT SYSTEM (USMS)
==========================================

Submitted by: Badia Aantar
Student ID: 20233120011

1. COMPILATION
---------------
Requirements:
- GCC/G++ 9.0 or newer (supports C++17)
- GNU Make

To compile:
1. Open terminal in project folder
2. Run:
   make clean && make

This creates the executable: university_system.exe

2. EXECUTION
------------
Run with:
./university_system.exe (Linux/Mac)
university_system.exe (Windows)

== University Management System Menu ==
1. Display All Students
2. Display All Faculty
3. Display All Courses
4. Enroll Student in Course
5. Assign Faculty to Course
6. Enter/Update Grades
7. Display Student Courses & GPA
8. Display Course Roster
9. Search Students (by ID/Name/GPA)
10. Add New Student
11. Add New Faculty
12. Add New Course
13. Save Data
14. Exit (auto-saves)

3. DATA FILES
-------------
Location: data/
- students.txt (Name,ID,Age,GPA)
- faculty.txt (Name,ID,Age,Specialization)
- courses.txt (Code,Title,FacultyID)
- enrollments.txt (CourseID,StudentID,Grade)

File Format Examples:
students.txt:
John Doe,1001,20,3.5
Jane Smith,1002,21,

courses.txt:
CS101,Introduction to Programming,2001
MATH202,Calculus II,

4. SYSTEM FEATURES
------------------
- OOP implementation with inheritance (Person→Student/Faculty)
- Polymorphic behavior for different person types
- Automatic GPA calculation (4.0 scale)
- Data persistence on exit/load on startup
- Input validation and error handling

5. CLEANUP
----------
To remove compiled files:
make clean

====================================
Developed for: University Management System Final Project
