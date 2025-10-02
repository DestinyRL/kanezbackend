# Kanexpro Project

## Overview
Kanexpro is a web application that provides an API for managing products. It is built using Node.js, Express, and MongoDB, and is designed to be hosted on Render.

## Features
- Connects to a MongoDB database hosted on Render.
- Defines a product schema using Mongoose.
- Provides API endpoints for:
  - Retrieving all products
  - Adding new products
  - Updating existing products
  - Deleting products
- Automatically adds default products to the database if the collection is empty.

## Getting Started

### Prerequisites
- Node.js installed on your machine.
- MongoDB database hosted on Render.
- An environment variable `MONGODB_URI` set with your MongoDB connection string.

### Installation
1. Clone the repository:
   ```
   git clone <repository-url>
   cd kanexpro
   ```

2. Install the dependencies:
   ```
   npm install
   ```

### Running the Application
1. Set the environment variable for MongoDB URI:
   ```
   export MONGODB_URI=<your-mongodb-uri>
   ```

2. Start the server:
   ```
   npm start
   ```

3. The API server will run on the specified port (default is 3001).

### API Endpoints
- `GET /api/products`: Retrieve all products.
- `POST /api/products`: Add a new product (requires admin password).
- `PUT /api/products/:id`: Update an existing product (requires admin password).
- `DELETE /api/products/:id`: Delete a product (requires admin password).

### Default Products
The application will automatically add a set of default products to the database if the products collection is empty.

## License
This project is licensed under the MIT License.