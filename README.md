# Student Management System (C++)

A menu-driven console application in C++ for managing student records, built to demonstrate core Object-Oriented Programming concepts.

## Features

- Add a new student (roll number, name, marks)
- Display all students
- Search a student by roll number
- Update a student's marks
- Delete a student record
- Show the total number of student objects
- Duplicate roll number check and marks validation (0 to 100)
- Automatic Pass/Fail result (pass mark: 40)

## OOP Concepts Used

| Concept | Where it is used |
|---|---|
| Classes and Encapsulation | `Student` class with private data members |
| Constructor | Initializes roll, name, marks and increments the count |
| Static member | `count` and `showCount()` track total objects |
| Friend function | `showStudent()` accesses private members |
| Inheritance | `Result` class inherits from `Student` |
| Virtual function and overriding | `display()` is overridden in `Result` to show Pass/Fail |
| Virtual destructor | Ensures proper cleanup through base-class pointers |
| Polymorphism | `Student*` array holding `Result` objects |
| Dynamic memory | Objects created with `new` and released with `delete` |

## How to Compile and Run

```bash
g++ studentmanagement.cpp -o student
./student
```

On Windows:

```bash
g++ studentmanagement.cpp -o student.exe
student.exe
```

## Menu

```
===== STUDENT MANAGEMENT SYSTEM =====
1. Add Student
2. Display Students
3. Search Student
4. Update Marks
5. Delete Student
6. Show Total Objects
0. Exit
```

## Project Structure

```
.
├── studentmanagement.cpp
└── README.md
```

## Future Improvements

- Save and load records from a file
- Sort students by marks
- Store full names with spaces

## Author

Your Name
