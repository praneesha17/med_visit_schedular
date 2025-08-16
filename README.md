# Med_visit_schedular - Doctor Appointment Booking System (PHP & MySQL)
Secure Doctor Appointment Booking System built with PHP &amp; MySQL.
 

**Open Source Doctor Appointment Booking System using PHP**

Secure eDoc is a simple yet robust web project made for **e-channeling** using **PHP, HTML, CSS, and MySQL**.  
This initiative facilitates **online appointment requests** for clients or patients of medical establishments, including clinics and hospitals.  
It also helps doctors manage their appointments efficiently.  

The system organizes schedules of each patient's appointment, which will be submitted as a request to the selected doctor.  
It provides three main roles: **Administrator, Doctor, and Patient**.  

- **Administrator** manages doctors, schedules, and patient records.  
- **Doctors** can view and manage their own appointments and patients.  
- **Patients** can register, browse doctors by specialty, and request appointments online.  

This version includes **important security hardening** to make it safe for production use.  

---

## 🔑 Demo Accounts

| Role   | Email               | Password |
|--------|---------------------|----------|
| Admin  | admin@edoc.com      | 123      |
| Doctor | doctor@edoc.com     | 123      |
| Patient| patient@edoc.com    | 123      |

---

## ✨ Features

### Admin
- Add, edit, and delete doctors  
- Schedule and remove doctor sessions  
- View patient details  
- View patient bookings  

### Doctor
- View their appointments  
- View scheduled sessions  
- Access patient details  
- Edit account settings  
- Delete account  

### Patient
- Register an account  
- Make online appointments  
- Browse doctors by specialty  
- View appointment history  
- Edit account settings  
- Delete account  

---

## 🔒 Security Improvements

This fork addresses known vulnerabilities from the original project (SQL Injection, XSS, CSRF, missing access controls):

- ✅ All queries converted to **prepared statements**  
- ✅ Implemented **CSRF protection** on forms  
- ✅ Escaped all outputs to prevent **XSS attacks**  
- ✅ Enforced **role-based access control** for admin pages  
- ✅ Session hardening (HTTPOnly, Secure, SameSite)  
- ✅ Proper redirects (`header("Location")` now followed by `exit;`)  
- ✅ Disabled PHP error display in production  
- ✅ `.htaccess` added to restrict sensitive files and prevent code execution in uploads  

---

## ⚡ Getting Started

### Requirements
- Apache 2.4+  
- PHP 8.0+ (works on 7.4 but 8.1+ recommended)  
- MySQL 5.7+ / MariaDB  

### Installation (XAMPP)
1. Open **XAMPP Control Panel** and start **Apache** and **MySQL**.  
2. Clone or download this repository.  
3. Copy the project folder into XAMPP’s `htdocs` directory.  
4. Open **phpMyAdmin** in a browser → [http://localhost/phpmyadmin](http://localhost/phpmyadmin)  
5. Create a new database named `edoc`.  
6. Import the provided SQL file: `edoc.sql`  
7. Update `config.php` with your database credentials (use a **non-root user**).  
8. Run the project at [http://localhost/edoc/](http://localhost/edoc/)  



## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, Bootstrap  
- **Backend**: PHP 8+, MySQL  
- **Server**: Apache 2.4 (works on Nginx + PHP-FPM as well)  
- **Tools**: XAMPP / LAMP stack  

---

