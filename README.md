# Hospital Management System
## Overview

This project is a simple, console-based Hospital Management System developed in C++ and C. It was created as a collaborative first-year, first-semester project with a focus on applying fundamental programming concepts and integrating an external database. The core logic of the application was a joint effort between myself and my collaborators, Velampudi Karthik and Zeenath Khalid Ahmad.

The project simulates a basic hospital system with user authentication and role-based access control, allowing different types of users to perform specific tasks.

## Key Features

1. Role-Based Access Control: Users are assigned roles (admin or staff) at login. Admin users have elevated privileges, such as the ability to add new users to the system.

2. Patient Record Management: The system allows for the creation of prescriptions and automated discharge summaries for patients.

3. Data Persistence: Patient and user data are stored in a local SQLite database, ensuring that information is saved between sessions.

4. Database Integration: The application connects to an external database to read and write user credentials and patient information.

## Technologies and Tools
1. C++: The primary programming language used to build the application's logic, control flow, and user interface.

2. SQLite3: A C library used for the database functionality. The implementation of this library was assisted by [Name of Assistance Tool, e.g., ChatGPT] as a learning exercise for database integration. The overall structure and application logic were designed and written entirely by our team.

3. Unix/Linux Environment: The code is designed to be compiled and run in a standard Unix-like environment.

## How to Compile and Run

To compile and run this program, you will need a C++ compiler and the SQLite3 development libraries installed on your system.

1. Save the file: Save the code to a file named Hospital_management_System.cpp.

2. Open your terminal: Navigate to the directory where you saved the file.

3. Compile the code: Run the following command. The -lsqlite3 flag links the SQLite library.

4. g++ Hospital_management_System.cpp -o HospitalManagementSystem -lsqlite3

5. Run the executable:

      >>On macOS/Linux: ./HospitalManagementSystem

      >>On Windows: HospitalManagementSystem.exe

## Future Improvements

This project was a great foundation for learning. Here are some potential improvements that could be made:

1. Enhanced Security: Implement secure password handling (e.g., hiding password input in the console, using salted hashes instead of plaintext).

2. Advanced Features: Add functionality to update or delete existing records, search for specific patients, and view prescription history.

3. Code Refactoring: Separate the codebase into different files (e.g., headers for function declarations, a main file for the application loop) for a more modular     and scalable design.

4. Error Handling: Improve validation for user inputs to prevent crashes and ensure data integrity.

## The Team

1. Velampudi Karthik – 2024006017
2. Benny Joel Martin (me) – 2024065836
3. Zeenat Khalid Ahmad - 2024080578
