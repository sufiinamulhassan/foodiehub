![Languages](https://img.shields.io/github/languages/top/sufiinamulhassan/foodiehub)
![Visitors](https://visitor-badge.laobi.icu/badge?page_id=sufiinamulhassanfoodiehub)

# FoodieHub (Food DB Web Application)

## 📖 Project Overview
A simple PHP‑MySQL web application that showcases a food menu, shopping cart, user authentication, and admin‑controlled product listings. The project is built with vanilla PHP, HTML, CSS and a tiny amount of JavaScript. It is perfect for learning basic CRUD operations, session handling and integrating a MySQL database.

---

## ✨ Features
- **Responsive UI** – clean layout with modern fonts and icons.
- **Product catalogue** – browse, filter and view detailed food items.
- **Shopping cart** – add, update, and remove items.
- **User authentication** – register / login with PHP sessions.
- **Admin panel** – manage categories, products and orders.
- **Search & quick view** – instant product preview.

---

## 🛠 Prerequisites
- **XAMPP** (Apache + MySQL) – any recent version works on Windows.
- A modern web browser.
- (Optional) Git – if you want to clone the repo.

---

## 🚀 Installation & Setup (XAMPP)
1. **Download & install XAMPP**
   - Grab the installer from https://www.apachefriends.org/index.html.
   - Run the installer and start **Apache** and **MySQL** from the XAMPP Control Panel.

2. **Place the project in the web root**
   ```
   C:\xampp\htdocs\foodiehub   (or any folder you prefer)
   ```
   - Copy the entire `food_db` folder into the chosen location.
   - Rename the folder to `foodiehub` for a cleaner URL (optional).

3. **Create the MySQL database**
   - Open **phpMyAdmin** (http://localhost/phpmyadmin).
   - Click **New**, name the database `food_db` and click **Create**.
   - Import the provided SQL dump:
     - Click the **Import** tab.
     - Choose `food_db.sql` from the project folder.
     - Press **Go**.

4. **Configure database credentials**
   - Open `components/connect.php`.
   - Ensure the credentials match your XAMPP setup (default is `root` with an empty password):
     ```php
     $db_name = 'mysql:host=localhost;dbname=food_db';
     $user_name = 'root';
     $user_password = '';
     ```
   - Save the file.

5. **Access the application**
   - Open a browser and navigate to:
     ```
     http://localhost/foodiehub/home.php
     ```
   - You should see the home page, be able to browse the menu, register a user, and place orders.

---

## 📂 Project Structure
```
foodiehub/
├─ about.php
├─ admin/                # admin‑only pages (order management, product CRUD)
├─ cart.php
├─ category.php
├─ checkout.php
├─ components/           # reusable header/footer & DB connection
│   ├─ connect.php
│   ├─ user_header.php
│   └─ footer.php
├─ css/                  # stylesheet(s)
├─ images/               # UI assets & product pictures
├─ js/                   # small client‑side scripts
├─ login.php
├─ menu.php
├─ orders.php
├─ profile.php
├─ quick_view.php
├─ register.php
├─ search.php
├─ update_address.php
├─ update_profile.php
└─ food_db.sql           # initial database dump
```

---

## 🧹 .gitignore
A `.gitignore` file is already added to the repository (see below). It excludes typical development artefacts such as IDE settings, OS files, and the local database file.

---

## 📦 Contributing
Feel free to fork the repo, open issues, or submit pull requests. Suggested improvements:
- Replace the inline CSS with a modern framework (e.g., Tailwind or Bootstrap).
- Add password hashing and prepared statements for better security.
- Implement a RESTful API for the frontend.

---

## 📜 License
This project is released under the **MIT License** – you are free to use, modify, and distribute it.

---

## 🏷 Suggested Repository Name
**`foodiehub`** – short, memorable, and reflects the purpose of the application.

---

*Happy coding!*
