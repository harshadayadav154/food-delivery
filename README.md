# Food Delivery App

## Overview
The **Food Delivery App** is a full-stack web application that allows users to browse food items, place orders, and manage their favorite foods. It consists of three main components:

- **Frontend**: User-facing application to browse and order food.
- **Backend**: Handles authentication, user management, and APIs.
- **Admin Panel**: Admins can add food items, manage categories, and update order statuses.

---

## Features
### User (Frontend)
- Browse available food items
- Add favorite foods
- Place an order
- View order history
- User authentication (Login/Register)

### Backend
- User authentication (JWT-based login/signup)
- REST APIs for fetching food items and orders
- Order processing and management
- Secure database storage

### Admin Panel
- Add/edit/delete food items and categories
- View all orders
- Update order statuses (e.g., Pending, In Progress, Delivered)

---

## Technologies Used
| Component   | Technologies |
|------------|-------------|
| Frontend   | React.js, CSS, axios, react-router |
| Backend    | Node.js, Express.js, MongoDB, stripe |
| Admin Panel | React.js, CSS, axios, react-router |
| Authentication | JWT (JSON Web Token) |

---

## Installation Guide

### 1. Clone the Repository
```sh
git clone https://github.com/harshadayadav154/food-delivery.git
cd food-delivery
```

### 2. Install Dependencies
#### Frontend
```sh
cd frontend
npm install
```

#### Backend
```sh
cd backend
npm install
```

#### Admin Panel
```sh
cd admin
npm install
```

### 3. Set Up Environment Variables
Create a `.env` file in the **backend** directory and add:
```env
STRIPE_SECRET_KEY=your_secret_key
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

### 4. Run the Application
#### Start Backend
```sh
cd backend
npm start
```

#### Start Frontend
```sh
cd frontend
npm start
```

#### Start Admin Panel
```sh
cd admin
npm start
```

---

## API Endpoints (Backend)
| Endpoint | Method | Description |
|----------|--------|-------------|
| `/api/user/register` | POST | Register a new user |
| `/api/user/login` | POST | User login |
| `/api/food/list` | GET | Get all food items |
| `/api/food/add` | POST | Add new food item |
| `/api/food/remove` | POST | remove food |
| `/api/cart/add` | POST | Add item to cart |
| `/api/cart/remove` | POST | Remove item from cart |
| `/api/cart/get` | Get | Get items from the cart |
| `/api/order/place` | POST | Place order |
| `/api/order/verify` | POST | Verify order |
| `/api/order/list` | POST | Get orders of the user |
| `/api/order/update` | POST | Update order status of the user |

---
