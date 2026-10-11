<div align="center">
  <img src="https://cdn-icons-png.flaticon.com/512/3514/3514491.png" alt="ShopNest Logo" width="80" />
  <h1>ShopNest - Full-Stack MERN E-Commerce App</h1>
  <p>A modern, full-stack E-commerce platform built with React, Node.js, Express, and MongoDB.</p>
  
  <p>
    <strong>Author:</strong> <a href="https://portfolio.vanshprojects.in/">Vansh Raturi</a> &bull; 
    <a href="https://www.linkedin.com/in/003va/">LinkedIn</a> &bull; 
    <a href="https://portfolio.vanshprojects.in/">Portfolio</a>
  </p>
</div>

---

## 🚀 Overview

**ShopNest** is a full-featured e-commerce web application engineered with modern MERN stack architecture. It features product exploration, Redux-managed shopping cart, secure JWT authentication, Cloudinary image hosting, automated email notifications via Nodemailer, Razorpay payment processing, and an Admin dashboard.

---

## 🛠 Tech Stack

- **Frontend:** React.js, Redux Toolkit (state management), React Router v6, Context API (Authentication).
- **Backend:** Node.js, Express.js REST API with middleware architecture.
- **Database:** MongoDB with Mongoose ORM.
- **Image Storage:** Cloudinary (via Multer).
- **Payments:** Razorpay API (with test transaction support and student fallback).
- **Emails:** Nodemailer (Gmail integration for order confirmations).

---

## ✨ Features

- 🔐 **User Authentication & Authorization:** Secure signup, login, JWT token verification, and role-based access (User & Admin).
- 🛍️ **Product Catalog & Management:** Browse products by category, view detailed specs, and real-time inventory tracking.
- 🛒 **Shopping Cart:** Persistent cart state using Redux Toolkit and localStorage.
- 💳 **Online Payments:** Razorpay integration for seamless order creation and cryptographic signature verification.
- 📦 **Order Management:** Place orders, receive automated confirmation emails, and view complete order history.
- 🖼️ **Cloudinary Uploads:** Admin panel with direct media upload for new products.
- 👑 **Admin Dashboard:** Add, edit, and delete products, plus monitor incoming customer orders.

---

## ⚙️ Environment Configuration

### Backend Setup (`backend/.env`)

Create a `.env` file inside the `backend/` directory based on [`.env.example`](backend/.env.example):

```env
PORT=5000
NODE_ENV=development
MONGO_URI=mongodb://127.0.0.1:27017/shopnest
JWT_SECRET=your_jwt_secret_key
CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret
GMAIL_USER=your_email@gmail.com
GMAIL_PASS=your_gmail_app_password
FRONTEND_URL=http://localhost:3000
```

### Frontend Setup (`frontend/.env`)

Create a `.env` file inside the `frontend/` directory based on [`.env.example`](frontend/.env.example):

```env
DANGEROUSLY_DISABLE_HOST_CHECK=true
REACT_APP_RAZORPAY_KEY_ID=your_razorpay_key_id
```

---

## 🏃 Getting Started Locally

### 1. Clone the Repository
```bash
git clone https://github.com/MastMaula1017/ShopNest.git
cd ShopNest
```

### 2. Install Dependencies
Install dependencies for root, backend, and frontend with a single command:
```bash
npm run install-all
```

### 3. Seed Database (Optional Starter Data)
Populate your database with sample products and a ready-to-use Admin user:
```bash
npm run seed
```
> **Default Admin Credentials:**
> - **Email:** `admin@shopnest.com`
> - **Password:** `password123`

### 4. Run Development Servers
Start both backend (Port 5000) and frontend (Port 3000) concurrently:
```bash
npm run dev
```

Visit **`http://localhost:3000`** in your browser.

---

## 📄 API Documentation (Postman)

A pre-configured Postman collection is included in the root directory: **`ShopNest_Postman_Collection.json`**.  
Import it into Postman to test authentication, products, orders, and payment endpoints.

---

## 📜 License

This project is licensed under the MIT License.
