# 📋 JavaFX Database Viewer  
**Author:** Simranjeet Kaur  
**Student ID:** 23099687
**Date:** June 18, 2025



## 🧩 Project Description

This JavaFX application connects to a MySQL database, retrieves data from a table, and displays it in a user-friendly GUI using a **TableView**. Users can load data on a button click.

---

## 📁 Project Structure

```
├── src/
│   ├── Person.java              # Model class for table data
│   ├── DBUtil.java              # Database connection helper
│   ├── PrimaryController.java   # Controls GUI actions
│   ├── SecondaryController.java # Optional additional controller
│   └── module-info.java         # Java module definition
├── resources/
├── pom.xml                      # Maven config with JavaFX dependencies
├── README.md                    # This file
```

---

## 🖥️ GUI Features

- TableView to display database records  
- Button to load/reload data from the database  
- Styled with JavaFX controls  
- Your name, student ID, and date are visible in the layout

> 📸 *Screenshot is saved in `/screenshots/` folder.*

---

## ⚙️ Technologies Used

- **Java 17+**
- **JavaFX 21**
- **MySQL 8+**
- **Maven**
- **IDE: VS Code or IntelliJ IDEA**

---

## 🔌 Database Setup

1. Create a MySQL database.
2. Add a table like:

```sql
CREATE TABLE people (
    id INT PRIMARY KEY,
    name VARCHAR(100),
    age INT
);
```

3. Insert sample data for testing.

4. Update your DB credentials in `DBUtil.java`:

```java
private static final String URL = "jdbc:mysql://localhost:3306/your_database";
private static final String USER = "your_username";
private static final String PASSWORD = "your_password";
```

---

## 🚀 How to Run

1. Make sure you have JavaFX SDK downloaded and set up.
2. Run with Maven:
   ```
   mvn clean javafx:run
   ```
   or run from your IDE with proper VM options:
   ```
   --module-path "C:\path\to\javafx-sdk-21.0.1\lib" --add-modules javafx.controls,javafx.fxml
   ```

---

## 🔗 GitHub Repository

**GitHub URL:** https://github.com/simranvirk23/lab1
---


