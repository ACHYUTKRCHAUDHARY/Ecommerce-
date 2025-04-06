# MERN E-Commerce Store

A full-featured e-commerce platform built with the MERN (MongoDB, Express.js, React, Node.js) stack.

![E-Commerce Store](thumb.png)

## Features

### User Features
- User authentication (Register, Login, Logout)
- Product browsing and searching
- Product filtering by category and price
- Product reviews and ratings
- Shopping cart management
- Favorites/Wishlist
- Order placement and tracking
- User profile management
- PayPal payment integration
- Responsive design for all devices

### Admin Features
- Admin dashboard with sales analytics
- User management
- Product management (CRUD operations)
- Category management
- Order management
- Sales tracking and reporting

## Tech Stack

### Frontend
- React.js with Vite
- Redux Toolkit for state management
- React Router for navigation
- PayPal integration for payments
- Modern UI/UX with responsive design

### Backend
- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Cookie-based sessions

## Getting Started

### Prerequisites
- Node.js
- MongoDB
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone <repository-url>
cd MERN-E-Commerce-Store
```

2. Install dependencies for backend
```bash
npm install
```

3. Install dependencies for frontend
```bash
cd frontend
npm install
```

4. Create a .env file in the root directory with the following variables:
```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
PAYPAL_CLIENT_ID=your_paypal_client_id
```

5. Start the development servers
```bash
# Start both frontend and backend
npm run dev

# Start backend only
npm run backend

# Start frontend only
npm run frontend
```

The frontend will run on http://localhost:5173 and the backend on http://localhost:5000

## API Endpoints

### Products
- GET /api/products - Get all products
- GET /api/products/:id - Get single product
- POST /api/products - Create a product (Admin)
- PUT /api/products/:id - Update a product (Admin)
- DELETE /api/products/:id - Delete a product (Admin)

### Users
- POST /api/users - Register a new user
- POST /api/users/auth - Login user
- POST /api/users/logout - Logout user
- GET /api/users/profile - Get user profile
- PUT /api/users/profile - Update user profile

### Orders
- POST /api/orders - Create new order
- GET /api/orders/mine - Get logged in user orders
- GET /api/orders/:id - Get order by ID
- PUT /api/orders/:id/pay - Update order to paid
- GET /api/orders - Get all orders (Admin)

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Acknowledgments

- Built with modern web technologies
- Implements best practices for security and performance
- Features a clean and intuitive user interface
