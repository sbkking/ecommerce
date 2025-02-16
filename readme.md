# E-Commerce API

This is a simple RESTful API for an e-commerce platform, built with Node.js, Express, and MongoDB.

## Prerequisites

Before you start, ensure you have the following installed:
- [Node.js](https://nodejs.org/) (v14 or later recommended)
- [MongoDB](https://www.mongodb.com/) (Local or Atlas cloud instance)
- [Git](https://git-scm.com/) (Optional but recommended)

## Installation

1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/ecommerce-api.git
   cd ecommerce-api
   ```
2. Install dependencies:
   ```sh
   npm install
   ```

## Configuration

1. Create a `.env` file in the root directory and add:
   ```env
   PORT=5000
   MONGO_URI=mongodb://localhost:27017/ecommerce
   JWT_SECRET=your_secret_key
   ```
   Replace `your_secret_key` with a strong secret key.

## Running the Server

To start the server, run:
```sh
npm start
```
The server will be running at `http://localhost:5000`

## API Endpoints

### User Routes
- **Register User:** `POST /api/users/register`
- **Login User:** `POST /api/users/login`

### Product Routes
- **Create Product:** `POST /api/products`
- **Get All Products:** `GET /api/products`

### Order Routes
- **Create Order:** `POST /api/orders`
- **Get Orders by User:** `GET /api/orders/:userId`

## API Documentation

Swagger API documentation is available at:
[http://localhost:5000/api-docs](http://localhost:5000/api-docs)

## Additional Notes
- Make sure MongoDB is running before starting the server.
- Use [Postman](https://www.postman.com/) or [Swagger UI](http://localhost:5000/api-docs) to test API requests.
- Contributions and improvements are welcome!

## License
This project is open-source and available under the [MIT License](LICENSE).

