# Fast React Pizza Co.

## Table of Contents

1. [Introduction](#introduction)
2. [Project Structure](#project-structure)
3. [Features](#features)
4. [Services](#services)
5. [Redux Setup](#redux-setup)
6. [User Geolocation](#user-geolocation)
7. [How to Run](#how-to-run)
8. [Future Improvements](#future-improvements)
9. [Contributing](#contributing)

## Introduction

Fast-React-Pizza is a web application developed using React.js and Redux Toolkit for managing pizza orders. It provides users with an easy-to-use interface to browse a menu, add items to their cart, create orders, and view/update their orders. The project utilizes modern web development tools like Vite for fast bundling, React Router for routing, and Tailwind CSS for styling.

## Project Structure

The project follows a structured directory layout for maintainability and scalability. Here's an overview of the directory structure:

```
FAST-REACT-PIZZA/
├── node_modules/
├── public/
│   └── vite.svg
├── src/
│   ├── features/
│   │   ├── cart/
│   │   │   ├── Cart.jsx
│   │   │   ├── CartItem.jsx
│   │   │   ├── CartOverview.jsx
│   │   │   ├── cartSlice.js
│   │   │   ├── DeleteItem.jsx
│   │   │   ├── EmptyCart.jsx
│   │   │   └── UpdateItemQuantity.jsx
│   │   ├── menu/
│   │   │   ├── Menu.jsx
│   │   │   └── MenuItem.jsx
│   │   ├── order/
│   │   │   ├── CreateOrder.jsx
│   │   │   ├── Order.jsx
│   │   │   ├── CreateItem.jsx
│   │   │   ├── SearchOrder.jsx
│   │   │   └── UpdateOrder.jsx
│   │   └── user/
│   │       ├── CreateUser.jsx
│   │       ├── Username.jsx
│   │       └── userSlice.js
│   ├── services/
│   │   ├── apiGeoconding.js
│   │   └── apiRestaurant.js
│   ├── ui/
│   │   ├── AppLayout.jsx
│   │   ├── Button.jsx
│   │   ├── Error.jsx
│   │   ├── Header.jsx
│   │   ├── Home.jsx
│   │   ├── LinkButton.jsx
│   │   └── Loader.jsx
│   ├── utils/
│   │   └── helpers.js
│   ├── App.jsx
│   ├── index.css
│   ├── main.jsx
│   └── store.js
├── .eslintrc.json
├── .gitignore
├── index.html
├── package-lock.json
├── package.json
├── postcss.config.js
├── prettier.config.cjs
├── tailwind.config.js
└── vite.config.js
```

## Features

The Fast React Pizza Ordering System includes the following features:

### Cart Management

The cart feature allows users to add, remove, and update the quantity of items in their cart. It provides functionalities like adding items to the cart, deleting items, increasing/decreasing item quantities, and clearing the entire cart.

### Menu Display

The menu feature displays a list of available pizzas for users to browse. Each menu item includes details such as the pizza name, price, and description. Users can view the menu to select items to add to their cart.

### Order Management

The order feature enables users to create new orders and view/update existing orders. Users can create orders by selecting items from the menu and adding them to their cart. They can then proceed to create a new order, providing necessary details like delivery address and contact information. Additionally, users can view their order history and update any existing orders as needed.

### User Management

The user feature allows users to manage their profile information. Users can update their username and access their geolocation-based address for order delivery.

## Services

### API Integration

The project integrates with external APIs to fetch geolocation data and restaurant information. It utilizes services like `apiGeocoding` and `apiRestaurant` to retrieve user addresses based on their geolocation and fetch menu items from the restaurant database.

## Redux Setup

Redux Toolkit is used for state management in the application. It provides a simplified API for configuring the Redux store, creating slices for managing specific parts of the state, and defining asynchronous actions using `createAsyncThunk`.

## User Geolocation

The application leverages the browser's geolocation API to fetch the user's current position. This information is then used to retrieve the user's address through reverse geocoding. The user's address is displayed in the order form, allowing them to verify and correct it if necessary.

## Technologies Used

- **React.js**: Frontend library for building user interfaces.
- **Redux Toolkit**: State management library for predictable state container.
- **React Router DOM**: Declarative routing for React applications.
- **Tailwind CSS**: Utility-first CSS framework for styling.
- **Vite**: Next-generation frontend tooling for fast development.
- **Node.js**: JavaScript runtime for server-side logic.
- **API Geocoding**: Reverse geocoding API for retrieving user addresses.

## How to Run

To run the Fast React Pizza Ordering System locally, follow these steps:

1. Clone the repository: `git clone https://github.com/itzharshitmavi/fast-react-pizza.git`
2. Navigate to the project directory: `cd FAST-REACT-PIZZA`
3. Install dependencies: `npm install`
4. Start the development server: `npm start`

## Future Improvements

- Implement user authentication and authorization for secure user accounts and order tracking.
- Enhance the user interface with additional features like sorting and filtering of menu items.
- Integrate payment processing for online orders.
- Implement real-time order tracking for users and restaurant staff.
- Improve error handling and validation for a smoother user experience.
