# Student Registration Form

This project is a simple Java Swing application for registering student information. It allows users to add, delete, and edit student records, which are stored in a MySQL database.  The application provides a graphical user interface (GUI) for easy interaction.

## Features

* **Add Student:**  Allows users to input student name, mobile number, and course, and then add the record to the database.
* **Delete Student:** Enables users to select a student record from the table and delete it from the database.
* **Edit Student:**  Permits users to select a student record, modify the information, and update the record in the database.
* **Display Student Records:** Shows all registered students in a table format within the application.
* **Database Integration:** Connects to a MySQL database named "judeuni" (you'll need to create this database and the "record" table) to store and retrieve student data.

## Prerequisites

* **Java Development Kit (JDK):** Make sure you have a compatible JDK installed on your system.
* **NetBeans IDE (or similar):** This project was developed in NetBeans.
* **MySQL Database:** You need a MySQL server running and a database named "judeuni" created.
* **MySQL JDBC Driver:** The project uses the MySQL Connector/J JDBC driver to connect to the database. Ensure this driver is added to your project's libraries.

## Setup and Running

1. **Download:** Download the project files (the Java code and any associated resources).
2. **Open in NetBeans:** Open the project in NetBeans IDE.
3. **Database Configuration:**
    * **Create Database and Table:** If you haven't already, create a MySQL database named "judeuni".
    * Create a table named "record" with the following structure:
        ```sql
        CREATE TABLE record (
            id INT AUTO_INCREMENT PRIMARY KEY,
            name VARCHAR(255),
            mobile VARCHAR(11),
            course VARCHAR(255)
        );
        ```
    * **JDBC Driver:** Make sure the MySQL JDBC driver is in your project's libraries.  In NetBeans, you can usually add this by right-clicking on Libraries in the Project view and adding a JAR file.
4. **Build and Run:** Build the project in NetBeans. Then, run the `schoolForm.java` file (the main form).

## How to Use

1. **Enter Student Information:** In the "Registration" panel, enter the student's name, mobile number, and course.
2. **Add Record:** Click the "Add" button to save the student's information to the database.
3. **Select Record:** Click on a row in the table to select a student record.  The selected record's data will populate the text fields.
4. **Edit Record:** After selecting a record, modify the information in the text fields and click the "Edit" button to update the record.
5. **Delete Record:** After selecting a record, click the "Delete" button to remove the record from the database.
