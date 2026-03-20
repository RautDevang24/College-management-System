# 🎓 College Management System (Java Swing + JDBC)

## 📌 Project Overview

The **College Management System** is a desktop-based application built using **Java Swing** for the user interface and **JDBC** for database connectivity.
This system allows administrators to manage student records efficiently and provides users with a simple way to search student information.

---

## 🚀 Features

### 👋 Welcome Page

* Entry point of the application
* Provides two options:

  * 🔐 **Admin Login**
  * 🔍 **Search Student**

---

### 🔐 Admin Module

After selecting **Admin**, the user is directed to a login page:

#### ✅ Login Page

* Admin authentication using username and password
* Secure validation using database (JDBC)

#### 🛠️ Admin Dashboard

After successful login, admin gets access to:

* ➕ **Add Student**
* ❌ **Delete Student**
* ✏️ **Update Student**
* 🔍 **Search Student**

---

### 🔍 Search Module (Public Access)

* Accessible directly from the welcome page
* User can search student details
* Uses **ComboBox** to select search criteria (e.g., Roll No, Name, City)
* Displays results in a **JTable**

---

## 🖥️ Technologies Used

* **Java Swing** – GUI Development
* **JDBC (Java Database Connectivity)** – Database operations
* **MySQL** – Backend database
* **Apache NetBeans** – IDE used for development

---

## 📂 Project Structure

```
college_management/
│
├── src/
│   ├── Welcome.java
│   ├── Login.java
│   ├── Admin.java
│   ├── AddStudent.java
│   ├── DeleteStudent.java
│   ├── UpdateStudent.java
│   └── SearchStudent.java
│
├── database/
│   └── student_data.sql
│
└── README.md
```

---

## 🗄️ Database Details

### Table: `student_data`

| Column   | Type     |
| -------- | -------- |
| rollno   | INT (PK) |
| name     | VARCHAR  |
| city     | VARCHAR  |

### Table: `admin_login`
| Column   | Type     |
| -------- | -------- |
| username | VARCHAR  |
| password | VARCHAR  |

---

## ⚙️ How to Run

1. Clone the repository:

```bash
git clone https://github.com/your-username/college-management-system.git
```

2. Open the project in **Apache NetBeans**

3. Configure MySQL database:

   * Create database
   * Import `student_data.sql`

4. Update database credentials in your Java code:

```java
String url = "jdbc:mysql://localhost:3306/your_db";
String username = "root";
String password = "your_password";
```

5. Run the project 🚀

---

## 📸 Screens (Optional – You can add later)

* Welcome Page
* Login Page
* Admin Dashboard
* Search Page

---

## 🔐 Future Enhancements

* Password encryption (BCrypt)
* Role-based access (Admin/User)
* Better UI design
* Export data (PDF/Excel)

---

## 🙌 Author

**Devang**

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
