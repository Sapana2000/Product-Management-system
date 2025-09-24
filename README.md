# Product-Management-system
E-Commerce Website with Admin Panel  This project is a full-stack E-commerce platform that provides a frontend shopping experience for customers and  Admins can manage categories, brands, products, orders, sliders, and website settings.  
E-Commerce Website with Admin Panel – Documentation
📖 Project Overview

This project is a full-stack E-commerce platform that provides a frontend shopping experience for customers and a backend admin panel for managing the store.

Frontend (Customer View): Users can browse products, add items to the cart, checkout, and manage accounts.

Backend (Admin Panel): Admins can manage categories, brands, products, orders, sliders, and website settings.

This system is designed with scalability and usability in mind.

✨ Features
🔹 Frontend (User Side)

Homepage

Product listings with pagination

Featured & new products sections

Search functionality

User Authentication

Register, Login, Logout

Product Management

Browse products by category or brand

View product details

Shopping Cart

Add to cart, remove from cart

Update cart quantities

Checkout process

Responsive Design

Works on desktop, tablet, and mobile

🔹 Backend (Admin Panel)

Dashboard Overview

Total Users, Orders, Categories, Products, Brands, Income

Category Management

Add, Edit, Delete Categories

Brand Management

Add, Edit, Delete Brands

Product Management

Add Product (with multiple images, price, description, stock)

Manage Products (update, delete, view)

Slider Management

Add/Manage homepage sliders

Theme Options

Control website theme (logos, colors, banners)

Order Management

View all orders with user details and order status

Update status (pending, shipped, delivered, cancelled)

User Management

Manage registered users

🏗️ System Architecture
1. Frontend (Client-Side)

Built using HTML, CSS, Bootstrap, JavaScript (or React if applicable).

Displays products, manages shopping cart, and provides checkout flow.

2. Backend (Server-Side)

Developed using PHP (CodeIgniter/Laravel) or Node.js/Express (depending on your tech).

Provides APIs for authentication, product management, cart, and orders.

3. Database

MySQL relational database used.

Schema includes:

users

categories

brands

products

orders

order_items

sliders

settings

📊 Database Design (Simplified Schema)
Users Table
Field	Type	Description
id	INT	Primary key
name	VARCHAR	Full name
email	VARCHAR	Unique email
password	VARCHAR	Hashed password
role	ENUM(admin,user)	Role-based access
Categories Table

| id | INT | PK |
| name | VARCHAR | Category name |

Brands Table

| id | INT | PK |
| name | VARCHAR | Brand name |

Products Table

| id | INT | PK |
| name | VARCHAR | Product name |
| price | DECIMAL | Product price |
| description | TEXT | Product details |
| category_id | INT | FK (categories) |
| brand_id | INT | FK (brands) |
| stock | INT | Quantity |

Orders Table

| id | INT | PK |
| user_id | INT | FK (users) |
| total_amount | DECIMAL | Order total |
| status | ENUM | pending, shipped, delivered, cancelled |
| created_at | TIMESTAMP | Order date |

Order Items Table

| id | INT | PK |
| order_id | INT | FK (orders) |
| product_id | INT | FK (products) |
| quantity | INT | Ordered qty |
| price | DECIMAL | Product price |

📌 User Flow
Frontend

User visits homepage → browses products

Adds items to Cart

Logs in / registers

Proceeds to checkout → places order

Backend

Admin logs in to admin panel

Can add/manage categories, brands, products

Manages orders & updates order status

Views dashboard reports (users, income, sales stats)

📷 Sample Pages
Admin Panel

Dashboard: Shows metrics like users, orders, products, income

Add Product Page: Form to upload product details

Manage Orders: Table view of all orders

Frontend

Homepage: Featured + new products

Product Page: Product details & add-to-cart

Cart Page: List of selected items

Checkout Page: Order summary

🛠️ Tech Stack

Frontend: HTML5, CSS3, Bootstrap, JavaScript (optionally React)

Backend: PHP (CodeIgniter/Laravel) or Node.js/Express

Database: MySQL

Version Control: Git & GitHub

Deployment: XAMPP / WAMP (local), or cloud hosting (Heroku, AWS, cPanel)

📈 Future Enhancements

Payment Gateway Integration (Stripe, Razorpay, PayPal)

Product Reviews & Ratings

Inventory Management System

Multi-language & Multi-currency Support

Advanced Analytics Dashboard

👩‍💻 Developed By

Sapana Sonawane
Web Developer
