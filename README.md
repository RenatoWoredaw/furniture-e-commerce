# Furniture E-Commerce Web Application

A full-stack furniture marketplace web application built with JavaScript, Node.js, Express, and MongoDB. The platform allows users to browse furniture products, create accounts, manage carts, complete secure online payments, and receive order confirmations.

---

# Features

## User Authentication

* User sign up and login system
* Secure password hashing
* Email verification system
* JWT-based authentication
* Dynamic UI updates based on authentication state

## Product & Cart System

* Browse furniture products
* Add items to cart
* Remove items from cart
* Increment and decrement item quantities
* Persistent cart storage per user

## Payment Integration

* Integrated Chapa payment gateway
* Secure payment verification
* Transaction reference tracking
* Payment success and failure handling
* Printable payment receipt

## Order Management

* Save completed orders to database
* Automatically clear cart after successful payment
* Store delivery address with each order
* Generate order receipts

## Address System

* Structured address collection for Ethiopia (Addis Ababa)
* Sub-city and district (Woreda) support
* Delivery information confirmation after purchase

## Deployment

* Frontend and backend deployed on Render
* MongoDB Atlas cloud database integration

---

# Technologies Used

## Frontend

* HTML
* CSS
* Vanilla JavaScript

## Backend

* Node.js
* Express.js

## Database

* MongoDB
* Mongoose
* MongoDB Atlas

## Authentication & Security

* bcrypt
* JSON Web Tokens (JWT)

## Payment

* Chapa Payment Gateway

## Email Service

* Resend API

## Deployment & Tools

* Git
* GitHub
* Render
* Postman

---

# System Flow

1. User creates an account
2. Verification code is sent to email
3. User verifies account
4. User logs in
5. User adds products to cart
6. User proceeds to checkout
7. Chapa payment is initialized
8. Payment is verified on the server
9. Order is saved to database
10. Cart is cleared
11. User receives printable receipt and delivery confirmation

---

# Project Structure

```bash
project-root/
│
├── models/
│   ├── User.js
│   └── Order.js
│
├── public/
│   ├── index.html
│   ├── cart.html
│   ├── payment-success.html
│   ├── payment-failed.html
│   └── js/
│       ├── authUI.js
│       ├── checkout.js
│       └── paymentSuccess.js
│
├── routes/
├── server.js
├── package.json
└── README.md
```

---

# Key Backend Features

## Authentication

* Password hashing using bcrypt
* JWT token generation and validation
* Protected API routes

## Payment Verification

* Server-side verification with Chapa API
* Prevents fake payment confirmations
* Secure transaction processing

## Database Design

* Structured user schema
* Cart persistence
* Order history storage
* Delivery address management

---

# Example Order Receipt

```text
Payment Successful

Items:
- Modern Chair x2
- Wooden Table x1

Total: 8,500 ETB

Delivery Address:
Ethiopia, Addis Ababa
Bole, Woreda 03

Status: Paid
```

---

# Challenges Solved During Development

* MongoDB local and Atlas connection setup
* JWT authentication implementation
* Dynamic multi-page authentication UI
* Chapa payment verification flow
* Cart synchronization with database
* Email verification system
* Secure order processing
* Render deployment issues and debugging

---

# Future Improvements

* Admin dashboard
* Product search and filtering
* Image upload system
* Delivery tracking
* Mobile app version
* User order history dashboard
* Product reviews and ratings
* PDF invoice generation

---

# About the Developer

Built by Renato Woredaw, a junior Computer Science graduate focused on full-stack web development and backend systems.

This project was created to strengthen practical skills in:

* Backend development
* Authentication systems
* Database design
* Payment integration
* API communication
* Deployment and debugging

---

# Contact

Email: renatonytadu@gmail.com

---

# License

This project is open for learning, collaboration, and portfolio demonstration purposes.
