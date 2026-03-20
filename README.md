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

## 📸 Screens 

* Welcome Page
  
  <img width="640" height="391" alt="image" src="https://github.com/user-attachments/assets/d64bb642-8258-48e0-8573-5e1c9c716386" />

* Login Page
<img width="640" height="335" alt="image" src="https://github.com/user-attachments/assets/f9010f0e-7370-402c-aec9-9b0bdf49fd93" />

* Admin Dashboard
<img width="640" height="329" alt="image" src="https://github.com/user-attachments/assets/71c9e579-d249-4208-8413-ae37e325a9fb" />
<img width="640" height="332" alt="image" src="https://github.com/user-attachments/assets/85ef20d9-05b8-4b44-8b1f-c4109b91a4d1" />
<img width="640" height="322" alt="image" src="https://github.com/user-attachments/assets/1e466e40-d5ad-4b25-b4f3-f27f1b96b647" />

* Search Page
  
  <img width="640" height="301" alt="image" src="https://github.com/user-attachments/assets/4c3a7c28-2d36-40c8-891e-5d73d596ee65" />


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
