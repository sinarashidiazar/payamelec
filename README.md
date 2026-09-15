# 🛒 PayamElectronic — E-commerce Management System

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PHP](https://img.shields.io/badge/PHP-7.4%2B-blue.svg)](https://www.php.net/)
[![MySQL](https://img.shields.io/badge/MySQL-5.7%2B-orange.svg)](https://www.mysql.com/)
[![Bootstrap](https://img.shields.io/badge/Bootstrap-4-purple.svg)](https://getbootstrap.com/)

A lightweight **e-commerce management system** built with **pure PHP** (no framework) and **MySQL**. It provides product management, category handling, user authentication, and a fully functional shopping cart — all wrapped in a responsive Bootstrap UI.

---

## 📋 Description

**PayamElectronic** is a self-contained e-commerce platform developed in pure PHP. It is designed for developers and learners who want a clean, readable codebase without the overhead of a framework. The system includes everything needed to run a small online store: product listing, categorization, user registration, authentication, shopping cart, and a full admin panel.

---

## ✨ Features

- 🛒 **Shopping Cart** — Add and remove products from the cart
- 👥 **User Management** — Registration, login, and authentication
- 📦 **Product Management** — Create, edit, and delete products
- 🏷️ **Category Management** — Manage categories and subcategories
- 🔐 **Admin Panel** — Full control over the entire system
- 📧 **Email Verification** — Email confirmation and password recovery
- 🎨 **Responsive UI** — Clean design powered by Bootstrap
- 🔒 **Security** — Authentication and role-based access control

---

## 🛠️ Technologies Used

| Technology | Purpose |
|------------|---------|
| **PHP 7.4+** | Core programming language |
| **MySQL** | Database |
| **Bootstrap 4** | CSS framework |
| **jQuery** | JavaScript library |
| **PDO** | Secure database connection |
| **SmartMenus** | Smart navigation menu |

---

## 📁 Project Structure

```
payamelec/
├── index.php                 # Entry point & router
├── PayamElectronic/
│   ├── config.php           # Database configuration
│   ├── function.php         # Helper functions
│   ├── Route.php            # Routing class
│   ├── action.php           # Action handlers
│   ├── Pages/               # Application pages
│   │   ├── admin/           # Admin panel pages
│   │   ├── login.php        # Login page
│   │   ├── register.php     # Registration page
│   │   ├── profile.php      # User profile page
│   │   └── ...
│   ├── Template/            # Templates & assets
│   │   ├── css/             # Stylesheets
│   │   ├── js/              # JavaScript files
│   │   ├── img/             # Images
│   │   └── ...
│   └── upload/              # Uploaded files
└── README.md                # This file
```

---

## 🚀 Installation

### Prerequisites

- PHP **7.4** or higher
- MySQL **5.7** or higher
- Apache / Nginx web server
- Composer *(optional)*

### Step-by-Step Setup

**1. Clone the repository**

```bash
git clone https://github.com/yourusername/payamelec.git
cd payamelec
```

**2. Create and configure the database**

Create a MySQL database named `payamelectronic`, then edit `PayamElectronic/config.php`:

```php
define('SERVERNAME', 'localhost');
define('DB_NAME',    'payamelectronic');
define('DB_USERNAME','your_username');
define('DB_PASSWORD','your_password');
define('URL',        'http://localhost/your-project/');
```

**3. Import the database schema**

Create the required tables in your database. At minimum you will need:

- `users`
- `products`
- `categories`
- `basket`

**4. Set folder permissions**

```bash
chmod 755 PayamElectronic/upload/
chmod 755 PayamElectronic/img/
```

**5. Run the project**

Place the project in your web server's root directory and open:

```
http://localhost/your-project/
```

---

## 📖 Usage Guide

### Authentication

- Access the admin panel via `/login`
- New users can register at `/register`

### Product Management

- Go to the **Products** section in the admin panel
- Add, edit, or delete products as needed

### Category Management

- Use the **Categories** section to create new categories
- Subcategories are also supported

---

## 🔧 Configuration

### Change Base URL

Edit the following line in `index.php`:

```php
define('BASEPATH', '/');
```

### Email Settings

To enable the email system, add your SMTP configuration inside `config.php`.

---

## 🤝 Contributing

Contributions are welcome! To contribute:

1. Fork the project
2. Create a feature branch
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. Commit your changes
   ```bash
   git commit -m "Add some AmazingFeature"
   ```
4. Push to the branch
   ```bash
   git push origin feature/AmazingFeature
   ```
5. Open a **Pull Request**

---

## 📝 License

This project is released under the **MIT License**.
See the [LICENSE](LICENSE) file for full details.

---

## ⭐ Support

If you find this project useful, please consider giving it a **star** on GitHub — it helps a lot!

---
