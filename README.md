# HOSPITAL-MANAGEMENT-SYSTEM
Hospital Management System - Code Explanation
We have created a Hospital Management System code written in C with SQLite. The system allows users to manage hospital operations like prescriptions, discharge summaries, and user authentication. It supports role-based access control (Admin/Staff/use).
1. Database Initialization
The `initialize_database` function sets up the SQLite database. It creates tables for users, prescriptions, discharge summaries, and other entities if they do not already exist. It also calls the `initialize_admin` function to ensure a default admin user is present.
2. Admin User Initialization
The `initialize_admin` function inserts a default admin user with username 'admin' and password 'admin123' if no users exist in the database. This ensures the system is accessible after setup.
3. User Authentication
The `authenticate_user` function checks user credentials (username, password, and role) against the database. It ensures only valid users can log in and assigns their role for access control.
4. Add User (Admin Only)
The `add_user` function allows the admin to create new users with specific roles ('admin' or 'staff'). This feature is restricted to admin accounts.
5. Add Prescription
The `add_prescription` function enables staff to add patient prescriptions, including patient name, doctor name, and medications. The details are stored in the `prescriptions` table.
6. Add Discharge Summary
The `add_discharge_summary` function allows adding a discharge summary for a patient. It captures the patient name and summary text and stores them in the `discharge_summary` table.
7. View Discharge Summaries
The `view_discharge_summaries` function retrieves and displays all discharge summaries stored in the database. It shows patient names, summaries, and IDs.
8. Role-Based Menu
The `main` function presents a menu to the user based on their role. Admins have access to all options, including user management, while staff have restricted access to prescriptions and discharge summaries.
Conclusion
We have learnt how to implement the code and logic learnt in class to create a program to solve real world problems and help clients make their businesses run more smoothly.


Velampudi Karthik – 2024006017
Benny Joel Martin – 2024065836
Zeenat Khalid Ahmad - 2024080578
