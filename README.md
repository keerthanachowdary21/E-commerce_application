# E-Commerce App

This project is a mock e-commerce application built using modern web development practices. It includes features like product listing, shopping cart management, checkout simulation, and user authentication.

## Table of Contents

- [Key Features](#key-features)
- [Setup Instructions](#setup-instructions)
- [Usage](#usage)
- [API Integration](#api-integration)
- [Authentication](#authentication)
- [Technologies Used](#technologies-used)

## Key Features

### Product Listing
- Displays a list of products fetched from a mock e-commerce API.
- Each product includes:
  - Name
  - Image
  - Price
  - "Add to Cart" button
- Pagination or infinite scrolling for loading additional products.
- Handles loading states and errors gracefully.
- Optionally implements caching and a loader for improved performance.

### Shopping Cart
- Users can:
  - Add products to the cart.
  - Remove products from the cart.
- Displays a cart summary with:
  - Total items
  - Total price
- Includes a checkout button leading to a simple checkout page.

### Checkout Simulation
- A mock checkout form requesting:
  - Name
  - Address
  - Payment details (no real payment processing).
- Displays a confirmation message with the order summary upon submission.

### Authentication
- User authentication system with login and registration features.
- Restricts access to the checkout page for unauthenticated users.

### HTML/CSS Design
- Clean and responsive layout for:
  - Product listing
  - Cart summary
  - Checkout page
- User-friendly and visually appealing design.

## Setup Instructions

### Prerequisites
- Node.js (v14+)
- Git

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```

## Usage

1. Open the app in your browser at `http://localhost:3000`.
2. Browse the product listing, add items to the cart, and proceed to checkout.
3. Register or log in to complete the checkout process.

## API Integration

This project uses the [Fake Store API](https://fakestoreapi.com/docs) to fetch product data. 

### Example Endpoint:
- Fetch all products:
  ```bash
  https://fakestoreapi.com/products
  ```

### Error Handling:
- Displays error messages if the API fails to respond.
- Shows a loader while data is being fetched.

## Authentication

### Features:
- Registration and login system.
- Ensures only authenticated users can proceed to the checkout page.

### Implementation:
- Stores user authentication status locally (e.g., in local storage or cookies).
- Redirects unauthenticated users to the login page.

## Technologies Used

- **Frontend:** HTML, CSS, JavaScript (or React.js if applicable).
- **Backend:** Node.js (optional for handling authentication or mock server).
- **API:** Fake Store API.

