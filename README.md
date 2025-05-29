# 📄 WEB-BASED DOCUMENT TRACKING SYSTEM AND MANAGEMENT  
### For National Irrigation Administration Regional Office IV-A (CALABARZON), Pila, Laguna

## 🔍 Short Description
This is a web-based document tracking and management system tailored for the **National Irrigation Administration (NIA) Regional Office IV-A** in Pila, Laguna. The system modernizes document handling by tracking documents in real-time, reducing bottlenecks, and organizing workflows for various user roles.

---

## ✨ Features Added / Enhanced
- 🔄 Migrated from Bootstrap to **Tailwind CSS** for a cleaner, modern look  
- 🎨 Improved and **modernized UI/UX** for better navigation and user experience

---

## 🛠️ Technologies Used
- **Frontend**: HTML, Tailwind CSS, JavaScript  
- **Backend**: PHP  
- **Database**: MySQL  
- **Libraries/Tools**:  
  - PHPMailer – Email handling  
  - PHPQRCode – QR Code generation  
  - SweetAlert – Alert modals  
  - DataTables – Table filtering and pagination

---

## 📦 Installation Instructions
You can run this project using either **XAMPP (recommended for simplicity)** or set up each component manually.

### 🔧 Option 1: XAMPP Setup (Easy Mode)
1. **Download and Install XAMPP**  
   👉 [https://www.apachefriends.org/index.html](https://www.apachefriends.org/index.html)

2. **Start Services**  
   Open the XAMPP Control Panel and start:
   - Apache
   - MySQL

3. **Project Setup**
   - Place the project folder named `document-tracking` into `htdocs`:
     ```
     C:\xampp\htdocs\document-tracking
     ```
   - Open [phpMyAdmin](http://localhost/phpmyadmin)
   - Create a new database named:
     ```
     document-tracking-db
     ```
   - Import the provided SQL file:
     ```
     document-tracking-db.sql
     ```

4. **Run the Project**
   - In your browser, go to: (http://localhost/document-tracking/)

---

### 🧠 Option 2: Manual Setup (Apache + PHP + MySQL + phpMyAdmin)

1. **Ensure these are installed and configured:**
- Apache HTTP Server
- PHP 7.4+
- MySQL Server
- phpMyAdmin (optional)

2. **Project Directory**
- Place the folder `document-tracking` in your server root directory:
  - Linux/macOS: `/var/www/html/document-tracking`
  - Windows: `C:\wamp64\www\document-tracking`

3. **Database Setup**
- Start MySQL
- Create database:
  ```sql
  CREATE DATABASE document-tracking-db;
  ```
- Import SQL dump:
  - phpMyAdmin: import `document-tracking-db.sql`
  - OR CLI:
    ```bash
    mysql -u root -p document-tracking-db < /path/to/document-tracking-db.sql
    ```

4. **Run the Project**
  - Navigate to: (http://localhost/document-tracking/)

---

## ▶️ How to Use / Run the Project
### 🚀 Easy Mode (XAMPP)
Just start Apache and MySQL, then go to: (http://localhost/document-tracking/)

### 🧠 Manual Setup
Follow the manual setup instructions above. After starting services and importing the DB, use the login credentials below to access the system.

---

## 🔐 Default System User Accounts

> These credentials are used to log in to the **web system**, not the MySQL database.

| User Role         | Username   | Password   |
|------------------|------------|------------|
| System Admin      | `admin`    | `admin`    |
| Document Handler  | `handler3` | `P4ss????` |
| Record Office     | `simon2`   | `P4ss????` |
| Guest             | `simon1`   | `P4ss????` |

✅ After logging in, each role has access to their respective dashboards and features based on permission levels.

⚠️ **Note:** These are demo/testing accounts. You can add, modify, or deactivate users via the Admin interface.

---

## 🎥 Demo Video
[🎬 Watch the demo here](https://drive.google.com/file/d/1r5LSeHYg1AEn11REPxOU7F_OD5We-3Ct/view?usp=sharing)

---

## 📁 Folder Structure Description
```
document-tracking/
├── PHPMailer/ # Handles email functionalities
│ ├── language/
│ └── src/
├── assets/ # Static files and frontend dependencies
│ ├── boxicons/
│ ├── cdnjs/
│ ├── cloudflare/
│ ├── css/
│ ├── datatable/
│ ├── fonts/
│ ├── img/
│ ├── jquery/
│ ├── js/
│ ├── jsdelivr/
│ ├── loader/
│ ├── qr-codes/
│ ├── stackpath/
│ ├── sweetalert/
│ ├── template/
│ ├── uploaded-pdf/
│ ├── user-profile/
│ └── webfonts/
├── controller/ # PHP files handling user requests and routing
├── model/ # PHP files for DB queries and logic
├── phpqrcode/ # Library for QR code generation
│ ├── bindings/
│ │ └── tcpdf/
│ ├── cache/
│ └── tools/
└── views/ # HTML views grouped by user roles
├── admin/
│ └── template/
├── guest/
│ └── template/
├── handler/
│ └── template/
├── internal/
│ └── template/
├── record_office/
│ └── template/
├── settings/
└── sysadmin/
└── template/
```

---

## 👥 Contributors
- **Adelan, Jhanna Shammel**
- **Almario, Cel Rick D.**
- **Bayani, Reigniell Ann L.**
- **Delos Santos, Gladys A.**
- **Javier, Geron Simon A.**
- **Redera, Angelo Nicolas A.**
