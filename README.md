# 🍔 FoodHub – Web-Based Food Ordering and Order Management System

A responsive web-based food ordering platform developed using **React.js, JavaScript, PHP, and MySQL**. FoodHub allows customers to browse food products, manage their shopping carts, place orders, and track order statuses. It also provides an administrator dashboard for managing food products, categories, customer orders, and sales.

---

## 📌 Project Overview

**FoodHub** is designed to make online food ordering easier, faster, and more convenient. Customers can explore different food categories, select their preferred meals, add items to their shopping cart, and complete their orders through an organized checkout process.

The system also helps restaurant administrators manage food menus, monitor incoming orders, update order statuses, and review sales performance through an administrative dashboard.

### 🎯 Main Objective

To develop a user-friendly and efficient online food ordering system that simplifies the ordering process for customers and improves restaurant order management through a centralized web-based platform.

---

## 👥 System Users

### 1. Customer

Customers can perform the following functions:

- Register and log in to their accounts.
- Browse available food products and categories.
- View food descriptions, prices, and images.
- Search for specific food items.
- Filter products by category and price.
- Add food items to the shopping cart.
- Increase or decrease item quantities.
- Remove items from the shopping cart.
- View order summaries and total costs.
- Enter delivery information.
- Select an available payment method.
- Place food orders.
- Track current order statuses.
- View previous orders and transaction history.
- Cancel orders when cancellation is permitted.

### 2. Administrator / Staff

Administrators or authorized staff can perform the following functions:

- Log in to the administrative dashboard.
- Add, edit, and delete food products.
- Manage food categories.
- Upload and update food images.
- Manage product prices and descriptions.
- Mark food products as available or unavailable.
- View and manage customer orders.
- Confirm or reject incoming orders.
- Update order statuses.
- View customer information.
- Monitor daily and overall sales.
- Generate sales reports.
- Manage customer accounts.

---

## ⚙️ Main System Modules

### 1. Food Menu and Categories

Displays available food products organized into different categories.

**Features:**
- Food categories such as Meals, Snacks, Beverages, and Desserts.
- Food images and descriptions.
- Product prices and availability.
- Search and filtering functionality.
- Featured and best-selling products.

### 2. Shopping Cart

Allows customers to temporarily store their selected food items before checkout.

**Features:**
- Add food items to the cart.
- Increase or decrease product quantities.
- Remove selected items.
- Automatically calculate item subtotals.
- Display the overall cart total.

### 3. Order Summary and Checkout

Provides customers with a complete overview of their selected items before confirming their orders.

**Features:**
- Display ordered food items.
- Show product quantities and prices.
- Calculate the subtotal.
- Display delivery fees.
- Calculate the final payment amount.
- Enter customer and delivery information.
- Select a payment method.
- Confirm and submit orders.

### 4. Order Status Tracking

Allows customers to monitor the progress of their food orders.

**Order Statuses:**

| Status | Description |
|---|---|
| Pending | Order has been submitted. |
| Confirmed | Restaurant has accepted the order. |
| Preparing | Food is currently being prepared. |
| Ready for Pickup | Order is ready for collection. |
| Out for Delivery | Order is being delivered. |
| Completed | Order has been successfully fulfilled. |
| Cancelled | Order has been cancelled. |

---

## ✨ Additional Features

- **User Authentication** – Provides secure customer and administrator login and registration.
- **Search Function** – Allows customers to search for food products by name.
- **Food Filtering** – Enables customers to filter products based on categories and prices.
- **Order History** – Displays customers' previous orders and transactions.
- **Notifications** – Provides updates regarding order confirmations and status changes.
- **Sales Dashboard** – Displays daily, monthly, and overall sales information.
- **Inventory Management** – Monitors product availability.
- **Responsive Design** – Supports desktop, tablet, and mobile devices.

---

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| React.js | Frontend interface and component development |
| JavaScript | Application logic and user interactions |
| PHP | Backend processing and API development |
| MySQL | Database management and data storage |
| HTML5 | Website structure |
| CSS3 | Website styling and layout |
| Figma | UI/UX design and prototyping |
| XAMPP | Local development server |
| Git & GitHub | Version control and source code management |

---

## 🏗️ System Architecture

FoodHub follows a client-server architecture in which React handles the frontend, PHP processes backend requests, and MySQL stores application data.

**System Workflow:**

1. Customers interact with the React-based website.
2. React sends requests to the PHP backend API.
3. PHP processes the requests and communicates with the MySQL database.
4. MySQL stores and retrieves the necessary information.
5. PHP returns the response to React in JSON format.
6. React displays the updated information to the customer or administrator.

---

## 🗄️ Database Structure

The system uses MySQL to manage customer information, food products, shopping carts, and order transactions.

**Recommended Database Tables:**

| Table Name | Description |
|---|---|
| users | Stores customer and administrator accounts. |
| categories | Stores food categories. |
| products | Stores food product information. |
| cart | Stores customer shopping carts. |
| cart_items | Stores individual items in shopping carts. |
| orders | Stores customer order information. |
| order_items | Stores products included in each order. |
| order_status_history | Records order status changes. |

---

## 📂 Project Structure

```text
FoodHub/
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   ├── App.jsx
│   │   ├── App.css
│   │   ├── index.css
│   │   └── main.jsx
│   ├── package.json
│   └── vite.config.js
│
├── backend/
│   ├── config/
│   ├── api/
│   ├── uploads/
│   └── index.php
│
├── database/
│   └── foodhub.sql
│
└── README.md
```

---

## 🚀 Installation and Setup

### Prerequisites

Before running the project, ensure that the following are installed:

- [Node.js (LTS)](https://nodejs.org/)
- [Visual Studio Code](https://code.visualstudio.com/)
- [XAMPP](https://www.apachefriends.org/)
- MySQL / phpMyAdmin
- Git (optional)

### Step 1: Clone the Repository

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

Navigate to the project directory:

```bash
cd FoodHub
```

### Step 2: Install Frontend Dependencies

Navigate to the frontend folder:

```bash
cd frontend
```

Install the required packages:

```bash
npm install
```

### Step 3: Set Up the Database

1. Open XAMPP Control Panel.
2. Start Apache and MySQL.
3. Open phpMyAdmin at `http://localhost/phpmyadmin`.
4. Create a database named `foodhub`.
5. Import the provided `foodhub.sql` file.
6. Configure the PHP database connection settings.

### Step 4: Configure the Backend

Place the backend folder inside the XAMPP `htdocs` directory or configure an appropriate Apache virtual host.

Example:

```text
C:\xampp82\htdocs\FoodHub\backend\
```

Configure the database connection using your local MySQL credentials.

### Step 5: Run the React Application

Inside the frontend directory, execute:

```bash
npm run dev
```

Open the local development URL provided by Vite, usually:

```text
http://localhost:5173
```

### Step 6: Access the PHP Backend

Example local backend URL:

```text
http://localhost/FoodHub/backend/
```

---

## 🔐 Security Considerations

- Store passwords using secure password hashing.
- Use prepared statements to prevent SQL injection.
- Validate and sanitize user inputs.
- Implement session-based or token-based authentication.
- Apply role-based access control.
- Protect administrator-only endpoints.
- Validate uploaded food images.
- Use HTTPS when deploying the application.

---

## 🎨 UI/UX Design

The interface is designed using Figma, focusing on a modern, clean, and user-friendly food ordering experience.

**Recommended Design Elements:**
- Orange primary color.
- White and light-gray backgrounds.
- Modern food product cards.
- Rounded buttons and input fields.
- Clear navigation and category filters.
- Responsive layouts for different screen sizes.

---

## 📱 Expected Project Output

The completed FoodHub system is expected to provide:

1. A functional customer food ordering website.
2. A responsive food menu and category interface.
3. A working shopping cart with automatic calculations.
4. An order summary and checkout system.
5. An order tracking interface.
6. An administrator dashboard.
7. Food product and category management.
8. Customer order management.
9. A MySQL relational database.
10. A complete Figma UI/UX prototype.

---

## 👨‍💻 Development Tools

- Visual Studio Code
- Figma
- XAMPP
- phpMyAdmin
- Git
- GitHub

---

## 📄 Project Information

**Project Name:** FoodHub – Web-Based Food Ordering and Order Management System

**Project Type:** Web-Based Application

**Frontend:** React.js and JavaScript

**Backend:** PHP

**Database:** MySQL

**Development Environment:** Visual Studio Code and XAMPP

**Design Tool:** Figma

---

*FoodHub – Making Food Ordering Easier, Faster, and More Convenient.*
