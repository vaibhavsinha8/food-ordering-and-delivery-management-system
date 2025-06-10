# Food-Ordering-and-Delivery-Management-System

A food ordering website made using Java, JDBC, JSP, and Servlets.

This project was created during my 2nd semester for the OOPS Java course. We were instructed to use JSP and Servlets. The website runs on localhost using a Tomcat server. JDBC and MySQL were used for database operations.

We will now walk you through the different webpages and features of the website.

> All images used were copyright-free at the time of use. If any image belongs to someone, kindly let us know, and we will remove it.

---

## 📌 Features

- User Registration & Login  
- Browse and Search Food Items  
- Add to Cart and Place Orders  
- Track Order Status  
- Admin Panel for Food and Order Management  
- Real-time Data Handling with MySQL  

---

## 🛠️ Technologies Used

| Technology       | Description                              |
|------------------|------------------------------------------|
| **Java (JDK 8+)**| Core programming language for logic       |
| **JSP/Servlets** | Server-side programming                  |
| **MySQL**        | Relational database for storing records  |
| **JDBC**         | Java API for connecting to MySQL         |

---

## 🔐 Login Page

This is a simple HTML page with a form that uses the `POST` method to send form data to `loginCheck.java` for authentication.  
Users can register if they don't have an account.

![Login Page Screenshot](https://github.com/user-attachments/assets/fe036122-1a16-45ae-8bf7-f6327a745b11)

---

## 📝 Register Page

A form is used to collect user data and passes it via `POST` to `registerInput.java` to register the new user in the database.  
Regex is used for email and password format validation.

![Register Page Screenshot](https://github.com/user-attachments/assets/36623bde-a223-4584-b54c-47ef7dd01f04)

---

## 🍽️ Welcome Page

After login, the user is redirected to `Welcome.jsp`, which starts a session.  
It has a navbar with **Logout** and **Cart** buttons and food items with **Add to Cart** options.  
The cart operation is handled via `addToCart.jsp`.

![Welcome Page Screenshot](https://github.com/user-attachments/assets/aff03995-f623-4e2f-b5a8-a00dd6cc34bb)

---

## 🛒 Cart Page

Displays all items added to the cart (`cart.jsp`).  
Users can either **Continue Shopping** or **Checkout**.

![Cart Page Screenshot](https://github.com/user-attachments/assets/312f176b-49da-48f6-a723-6027368d5802)

---

## 💳 Checkout Page

The final step (`Checkout.jsp`). Users can only logout from here.

![Checkout Page Screenshot](https://github.com/user-attachments/assets/54fc3a4e-3ba0-4902-8d07-4bf52728492b)

---

## 🗃️ Database Schema (MySQL via JDBC)

Connected to Java using JDBC. Below are the tables:

### 📋 Tables Overview

![DB Tables Overview](https://github.com/user-attachments/assets/a335feac-8633-424d-aa3a-b77b3c122705)

---

### 👤 Customer Table

![Customer Table](https://github.com/user-attachments/assets/7e300cd2-34fd-4a28-b020-4e9a564c68b1)

### 🍹 Drinks Table

![Drinks Table](https://github.com/user-attachments/assets/77c6e1a8-d147-4001-a47e-2e8aec1fe984)

### 🍲 Food Table

![Food Table](https://github.com/user-attachments/assets/47e753b0-ff93-4bbf-bc31-6cf5d3889596)

### 🧾 Drink Order Table

![Drink Order Table](https://github.com/user-attachments/assets/30ed3009-3853-44d9-b53b-e313785b3a31)

### 🧾 Food Order Table

![Food Order Table](https://github.com/user-attachments/assets/1e144e4c-35bd-4675-843d-364f5065faf1)

### 📦 Total Order Table

![Total Order Table](https://github.com/user-attachments/assets/cbf161af-44d3-440d-84dc-0472a481f748)

---

## ✅ Future Improvements

- Add email verification for registration
- Implement order cancellation
- Improve UI with CSS framework like Bootstrap
- Add admin login functionality
- Implement user reviews/ratings for food

---

## 🧪 Testing

- Login with invalid credentials → displays error
- Registration with invalid email/password → blocked by regex
- Cart behavior verified for multiple items
- Checked session timeout on logout

---

## 📁 Folder Structure
```
FoodOrderingSystem/
│
├── src/
│ ├── db/ # JDBC connection code
│ ├── user/ # Login, Register, Session handling
│ ├── order/ # Cart, Order, Checkout logic
│
├── web/
│ ├── index.html
│ ├── login.jsp
│ ├── register.jsp
│ ├── welcome.jsp
│ ├── cart.jsp
│ ├── checkout.jsp
│
├── docs/
│ ├── screenshots/
│ └── README.md
│
├── sql/
│ └── create_tables.sql
│
└── .gitignore
```
