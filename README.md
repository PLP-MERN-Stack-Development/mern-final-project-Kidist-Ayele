# 🛍️ E-Commerce Platform - MERN Stack Capstone Project

A full-stack e-commerce application built with the MERN stack, featuring product management, shopping cart, order processing, and admin dashboard.

## 🚀 Live Demo

**User**: https://shopnest-f.vercel.app/ 

**Admin Dashboard**: https://shopnest-adminpanel.vercel.app/

**Video Demonstration**: https://bit.ly/4i9Bb1a

## 📸 Screenshots

- Homepage
  <img width="1301" height="638" alt="image" src="https://github.com/user-attachments/assets/9657f4bd-5351-4a2b-b982-0d3e6e026b0c" />

- Product Catalog
  <img width="1280" height="631" alt="image" src="https://github.com/user-attachments/assets/571e62cb-d277-4849-b73a-217a99633250" />
  
- Shopping Cart
  <img width="1301" height="637" alt="image" src="https://github.com/user-attachments/assets/7d903358-3216-4295-8cc0-6288106204f8" />

- Admin Dashboard
  <img width="1301" height="627" alt="image" src="https://github.com/user-attachments/assets/968697c4-8369-4008-aac2-8a98bcdda0d3" />

- User Profile
  <img width="1315" height="610" alt="image" src="https://github.com/user-attachments/assets/a7bb422e-4a3a-48b1-bf0b-bb8684de0892" />

## 🎯 Project Overview

This capstone project is a comprehensive e-commerce platform that demonstrates full-stack MERN development skills including RESTful API design, authentication, payment integration, and responsive UI development.

### Key Features

- **User Management**: Registration, login, profile management
- **Product Catalog**: Browse products by category, search, and filter
- **Shopping Cart**: Add/remove items, manage quantities
- **Order Processing**: Place orders, track order history
- **Payment Integration**: Stripe and Chapa payment gateways
- **Admin Dashboard**: Product management, order tracking
- **Image Upload**: Cloudinary integration for product images
- **Responsive Design**: Mobile-first approach with Tailwind CSS

## 🛠️ Tech Stack

### Frontend

- React 18
- React Router DOM
- Tailwind CSS
- Framer Motion
- Axios
- React Toastify

### Backend

- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Multer (file upload)
- Cloudinary
- Stripe & Chapa


## 📁 Project Structure

```
mern-final-project-Kidist-Ayele/
├── frontend/          # React frontend application
├── backend/           # Express.js backend API
├── admin/            # Admin dashboard (React)
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher)
- MongoDB Atlas account or local MongoDB
- npm or yarn

### Installation

1. Clone the repository

```bash
git clone https://github.com/PLP-MERN-Stack-Development/mern-final-project-Kidist-Ayele.git
cd mern-final-project-Kidist-Ayele
```

2. Install backend dependencies

```bash
cd backend
npm install
```

3. Install frontend dependencies

```bash
cd ../frontend
npm install
```

4. Install admin dependencies

```bash
cd ../admin
npm install
```

5. Configure environment variables

Create a `.env` file in the `backend/` directory with the following variables:

```env
PORT=3000

MONGODB_URI=your_mongodb_connection_string

CLOUDINARY_CLOUD_NAME=your_cloudinary_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret

JWT_SECRET=your_jwt_secret_key

ADMIN_EMAIL = "admin@example.com"
ADMIN_PASSWORD = "admin12345"

STRIPE_SECRET_KEY=your_stripe_secret_key

CHAPA_URL=https://api.chapa.co/v1/transaction/initialize
CHAPA_AUTH=your_chapa_auth_token
```

**Important Notes:**

- Create the `.env` file in the `backend/` directory (not in root)
- Replace all placeholder values with your actual credentials
- Make sure there are no spaces around the `=` sign
- For local development, use `mongodb://localhost:27017` for MONGODB_URI
- For production, use your MongoDB Atlas connection string
- Keep your `.env` file secure and never commit it to version control

6. Run the application

Backend:

```bash
cd backend
npm run dev
```

Frontend:

```bash
cd frontend
npm run dev
```

Admin:

```bash
cd admin
npm run dev
```

## 📋 API Endpoints

### User Routes

- `POST /api/user/signup` - User registration
- `POST /api/user/login` - User login
- `POST /api/user/getuser` - Get user details

### Product Routes

- `GET /api/product/list` - Get all products
- `POST /api/product/details` - Get product details
- `POST /api/product/add` - Add product (Admin)
- `POST /api/product/remove` - Remove product (Admin)

### Cart Routes

- `POST /api/cart/add` - Add to cart
- `POST /api/cart/remove` - Remove from cart
- `POST /api/cart/get` - Get cart items

### Order Routes

- `POST /api/order/place` - Place order
- `POST /api/order/list` - Get user orders


## 🏗️ Architecture

### Database Schema

- **Users**: Authentication, profile, cart data
- **Products**: Product details, images, reviews, ratings
- **Orders**: Order details, payment status
- **Subscriptions**: Newsletter subscriptions

### Key Technical Decisions

- JWT-based authentication for secure user sessions
- Cloudinary for efficient image storage and delivery
- Multiple payment gateway support for flexibility
- Separate admin dashboard for better UX
- RESTful API design for scalability

