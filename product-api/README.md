# SBA – Build a Product API

## Project Overview

This project is a RESTful API built for the fictional e-commerce company **Zenith**. The API manages product inventory and supports full CRUD operations along with advanced querying features such as filtering, sorting, and pagination.

The application is built using Node.js, Express, MongoDB, and Mongoose. It is structured in a modular way and follows backend best practices at a junior developer level.

---

## Technologies Used

* Node.js
* Express.js
* MongoDB Atlas
* Mongoose
* dotenv

---

## Project Setup

### 1. Create Project Folder

```bash
mkdir product-api
cd product-api
```

### 2. Initialize Node Project

```bash
npm init -y
```

### 3. Install Dependencies

```bash
npm install express mongoose dotenv
```

---

## Folder Structure

```text
product-api/
├── config/
│   └── connection.js
├── models/
│   └── Product.js
├── routes/
│   └── productRoutes.js
├── server.js
├── .env
├── .gitignore
├── README.md
└── Reflection.md
```

---

## Environment Configuration

### .env

```text
MONGO_URI=your_mongodb_connection_string
PORT=3000
```

### .gitignore

```text
node_modules
.env
```

---

## Database Connection

### config/connection.js

This file handles the MongoDB connection using Mongoose.

---

## Product Model

### models/Product.js

The Product schema includes validation rules, default values, and required fields based on the project requirements.

---

## API Endpoints

### Create a Product

**POST /api/products**

* Creates a new product
* Returns status 201 on success

### Get All Products (Advanced Querying)

**GET /api/products**

* Supports filtering by category and price
* Supports sorting by price
* Supports pagination using page and limit

### Get One Product

**GET /api/products/:id**

* Retrieves a single product by ID

### Update a Product

**PUT /api/products/:id**

* Updates an existing product

### Delete a Product

**DELETE /api/products/:id**

* Deletes a product by ID

---

## Running the Server

```bash
node server.js
```

If successful, the console will log that MongoDB is connected and the server is running.

---

## Testing the API

All endpoints were tested using Postman. Different combinations of filters, sorting, and pagination were tested for the GET all products endpoint.

---

## Resources Used

* Node.js Documentation
* Express.js Documentation
* MongoDB Atlas Documentation
* Mongoose Documentation
* Course labs and lecture notes
