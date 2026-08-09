# Expense Tracker

A full-stack **Expense Tracker** built with the **MERN stack** that helps users securely manage income and expenses, track transaction history, and analyze financial data through dashboard summaries and charts.

## Overview

This project is a personal finance application where authenticated users can:

* Add, update, and delete income and expense transactions
* View financial summaries on a dashboard
* Analyze spending patterns using charts and analytics
* Filter and manage transaction history
* Use a responsive and user-friendly interface

The project follows a frontend-backend architecture where the **React frontend** communicates with the **Node.js + Express backend** through REST APIs, and **MongoDB** stores user and transaction data. Authentication is handled using **JWT**.

## Features

* User authentication and authorization
* Secure login and protected routes
* Income and expense CRUD operations
* Dashboard with summaries and analytics
* Transaction history management
* Filtering and searching transactions
* Responsive UI
* Error handling and input validation

## Tech Stack

**Frontend**

* React
* HTML
* CSS
* JavaScript

**Backend**

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcrypt

## Project Structure

```bash
Expense-Tracker/
├── frontend/
├── backend/
└── .gitignore
```

## How It Works

1. The user logs in or registers.
2. The frontend sends requests to protected backend APIs.
3. The backend validates the request and identifies the authenticated user.
4. Transactions are saved in MongoDB with the user’s ID.
5. Dashboard totals and charts are generated from the stored data.

## Security Practices

* Passwords are hashed before storing
* JWT is used for authentication
* User data is separated by authenticated user ID
* Environment variables are used for secrets
* Input validation is applied on both frontend and backend

## Installation

### Frontend

```bash
cd frontend
npm install
npm run dev
```

### Backend

```bash
cd backend
npm install
npm start
```

## Environment Variables

Create a `.env` file in the backend folder and add values such as:

```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000
```

## API Features

Typical API capabilities include:

* Authentication
* Transaction CRUD
* Dashboard summary data
* Monthly or category-wise analytics

## Future Improvements

* Recurring transactions
* Budget limits
* CSV/PDF export
* Notifications
* Better pagination
* Automated tests

## Interview Note

This project is also designed for interview preparation, so be ready to explain:

* Project architecture
* Authentication flow
* MongoDB collections
* Dashboard calculations
* Security handling
* Error handling and deployment approach

## License

This project is for learning and portfolio purposes.
