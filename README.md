
# **Library Management System (LMS)**

The Must University Library Management System (LMS) is a web-based platform tailored for the efficient management of library operations at Must University. It serves as a bridge between students, faculty, and administrators to enhance accessibility and streamline library workflows.
---

## **Features**

### **General Features**
1. **Book Management**:
   - Add, edit, and delete book records.
   - Categorize books into various genres.
2. **User Management**:
   - Register, view, and manage library users.
3. **Author Management**:
   - Maintain a list of book authors .
4. **Issue & Return Management**:
   - Manage the issuance and return of books.
5. **Secure Login System**:
   - Includes user authentication and change password functionalities.

---

## **Repositories and Files**

### **1. Admin Repository**
The admin repository contains all backend files required for administrative functionalities.

#### **Key Directories and Files**
- **Directories**:
  - **`assets/`**: Static assets like CSS, JS, and images for styling and interactivity.
  - **`includes/`**: Shared PHP scripts (e.g., database connection and utility functions).
  
- **Important PHP Files-Admin**:
  - **`add-author.php`**: Add a new author.
  - **`add-book.php`**: Add a new book.
  - **`add-category.php`**: Add a new book category.
  - **`edit-author.php`**: Edit existing author details.
  - **`edit-book.php`**: Edit existing book records.
  - **`edit-category.php`**: Edit existing categories.
  - **`dashboard.php`**: Displays the admin dashboard with an overview of statistics.
  - **`manage-authors.php`**: Manage authors.
  - **`manage-books.php`**: Manage book records.
  - **`manage-categories.php`**: Manage book categories.
  - **`manage-issued-books.php`**: Track issued books and their statuses.
  - **`reg-students.php`**: View and manage registered students.
  - **`logout.php`**: Admin logout functionality.

  - **Important PHP Files-User**:
   - **`signup.php`**: User registration form for creating new accounts.
  - **`index.php`**: Home page for users to log in and navigate to their accounts.
  - **`user-forgot-password.php`**: Enables users to recover their password.
  - **`logout.php`**: Logs out the current user from the session.
  - **`my-profile.php`**: Allows users to manage and update their profile information.
  - **`issued-books.php`**: Displays the list of books currently issued to the logged-in user.
  - **`check_availability.php`**: check if the email is valid and available.


---

### **2. SQL File Repository**
The SQL repository contains the database structure and sample data required to run the Library Management System.

#### **Files**
- **`library.sql`**:
  - Contains the database schema.
  - Includes tables for `books`, `authors`, `categories`, `users`, `issued_books`, and more.
  - Includes sample data for initial setup.
  
- **`read me.txt`**:
  - Instructions on how to import the SQL file and configure the database connection.

---

## **Setup Instructions**

### **1. Clone or Download the Project**
- Place the `LMS` folder in the `www` or `htdocs` directory of your local server (e.g., EasyPHP, XAMPP, WAMP).

### **2. Import the SQL File**
- Open **phpMyAdmin** or a similar database tool.
- Create a new database, e.g., `library`.
- Import the `library.sql` file from the `sql file` folder.

### **3. Configure Database Connection**
- Edit the `includes/config.php` file:
  ```php
  $host = "localhost";
  $dbname = "library";
  $username = "root";
  $password = ""; // Replace with your database password
  ```

### **4. Run the Project**
- Access the project in your browser:
  ```
  http://localhost/LMS
  ```

---

## **Admin Dashboard Login**
Use the following credentials to log in as an admin:
- **Username**: `admin`
- **Password**: `Test@123` .

---

## **User Dashboard Login**
Use the following credentials to log in as a User:
- **Username**: `Ammar1@gmail.com`
- **Password**: `Test@123` .

---


## **Technologies Used**

- **Backend**: PHP
- **Frontend**: HTML, CSS, JavaScript (Bootstrap for responsive design).
- **Database**: MySQL
- **Server**: EasyPHP Devserver

---

## **Contributing**
If you wish to contribute:
1. Fork this repository.
2. Create a feature branch: `git checkout -b feature-name`.
3. Commit your changes: `git commit -m "Add feature"`.
4. Push the branch: `git push origin feature-name`.
5. Submit a pull request.

---

## **Acknowledgments**
- Bootstrap for frontend styling.
- EasyPHP Devserver for local server development.

---

