# University Management System

A high-performance Java desktop application designed to manage academic records, student enrollments, and faculty assignments. This project serves as a practical implementation of **Object-Oriented Programming (OOP)** and **Data Structures**, featuring a custom-built collection framework and an interactive Graphical User Interface (GUI).

## 📌 Project Overview

The **University Management System** provides a centralized platform for administrators to handle the lifecycle of students, professors, and courses. Unlike typical applications that rely on built-in Java Collections (like `ArrayList` or `LinkedList`), this system is built upon a **proprietary Singly Linked List** implementation, showcasing a deep understanding of memory management and algorithmic logic.

## 🏗️ Technical Architecture

### 1. Custom Data Structures & Algorithms

The backbone of the project is a custom generic engine found in `MyList.java` and `Node.java`.

* **Custom Linked List:** A generic `MyList<T>` class handles dynamic data without using `java.util`.
* **Bubble Sort:** Manually implemented to ensure data is organized by unique identifiers.
* **Binary Search:** Optimized retrieval logic that performs  searches on sorted academic records, significantly improving performance over standard linear searches.

### 2. Domain Modeling (OOP)

The system uses a clean inheritance hierarchy to maintain dry, reusable code:

* **Abstraction:** An abstract `Person` class defines the core identity (ID, Name) for all university members.
* **Specialization:** `Student` and `Professor` classes extend the base class to add specific attributes like department, GPA, and faculty expertise.
* **Relationship Management:** The `Enrollment` class acts as a bridge, linking students to courses, while the `Course` class manages instructor assignments.

### 3. Modern GUI Design

The interface is built using **Java Swing**, but goes beyond standard components:

* **Custom Rendering:** `RoundedButton` and `RoundedBorder` use `Graphics2D` and anti-aliasing to provide a modern, sleek aesthetic.
* **Interactive Dashboard:** A tabbed interface in `UniversitySystemGUI` allows for seamless switching between Student, Professor, and Course management modules.

## 🛠️ Functional Features

* **Faculty Workload Management:** Automatically enforces a limit of 3 courses per professor.
* **Dynamic Data Persistence:** Loads and saves information from `university_data.txt` to ensure data is maintained between sessions.
* **Search & Filter:** Allows administrators to find any entity instantly using the optimized binary search engine.
* **CRUD Operations:** Full support for Adding, Viewing, and Removing records across all modules.

## 💻 Tech Stack

* **Language:** Java
* **GUI:** Swing / AWT
* **Data Handling:** Custom Singly Linked List
* **Algorithms:** Bubble Sort, Binary Search
* **Storage:** File-based I/O (TXT)
