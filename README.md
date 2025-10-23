# 🏥 Hospital Management System (Java + MySQL)

A full-stack desktop-based Hospital Management System built with Java Swing and connected to a MySQL database using JDBC. This project handles everything from patient registration to doctor appointments, pharmacy stock, blood bank data, and health camp management — all wrapped in a modular architecture.

---

## 🚀 Features

### 🧑‍⚕️ Doctor Module
- Secure login for doctors
- View and manage patient consultations
- Record medical remarks

### 🧍 Patient Module
- Patient signup/login
- Book appointments
- Access medical records and appointment history

### 💊 Pharmacy Module
- Check and update medicine inventory
- Track availability and stock level changes

### 🩸 Blood Bank Module
- Manage blood donations and requests
- Track blood group inventory in real time

### 🏕️ Camp Module
- Organize medical/awareness camps
- View and track camp details

### 🧑‍💻 UI Module
- Login page for patients and doctors
- Central dashboard (main page)
- FAQ/help interface

---

## ⚙️ Tech Stack

- **Language:** Java (JDK 8+)
- **UI Framework:** Swing / AWT
- **Database:** MySQL (via MySQL Workbench)
- **Connectivity:** JDBC
- **IDE:** IntelliJ / Eclipse / NetBeans
- **Version Control:** Git + GitHub

---

## 🗃️ Project Structure
```bash
hospital_management/
├── bloodbank/
├── camp/
├── doctor/
├── patient/
├── pharmacy/
└── ui/
```
Each package contains its respective Java classes, which interact with the database using JDBC.

---

## 🛠️ Setup & Run

### 🔧 Prerequisites

- Java JDK 8 or higher
- MySQL Server + MySQL Workbench
- IDE (e.g., IntelliJ, Eclipse)
- MySQL JDBC Driver (Connector/J)

### 🏗️ Database Setup

1. Open **MySQL Workbench**
2. Run the SQL script provided in `/database/hospital_db.sql` (if available)  
   _or manually create the following tables_:
   - `patients`
   - `doctors`
   - `appointments`
   - `medicines`
   - `blood_inventory`
   - `camps`
3. Update the DB credentials in your code (likely in a `DBConnection.java` or similar):
   ```java
   String url = "jdbc:mysql://localhost:3306/hospital_db";
   String username = "your_mysql_username";
   String password = "your_mysql_password";
   
▶️ Run the App
Clone the repository:

git clone https://github.com/Keerti2504/hospital_management.git
cd hospital_management
Open the project in your IDE

Compile and run:

Start from ui/Mainpage.java or ui/login.java

Ensure MySQL is running


📌 Notes
This project demonstrates integration of GUI + JDBC + MySQL in Java. 
It can be extended with:
Admin module
Role-based access control
Spring Boot REST APIs for web-based versions
Charts/reports using JavaFX or third-party libraries
