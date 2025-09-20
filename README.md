# Grocery Store Management System 👨🏻‍🔧

## Project Description: 👨‍🏫
- The "Grocery Store Management System" is a web-based application designed to automate and manage various aspects of a grocery store.
- This system allows store administrators to manage products and inventory efficiently, while customers can browse products, add items to their cart, and place orders online.
- The system provides a user-friendly interface for customers and a robust backend to ensure smooth operations.

## Project Architecture: 🛠
<img width="930" alt="Screenshot (3174)" src="https://github.com/user-attachments/assets/1b96ef8b-f77e-4418-b5d2-efe5b1270849">


## Database Schema: 
- User Login Table: Represents users with a unique user_id.
- Product Table: Represents products with a unique prod_id.
- Cart Table: Represents the shopping cart, linking user_id to prod_id with a quantity.
- Order Table: Represents orders made by users with a unique order_id, and links to user_id.

## E-R Diagram:
- The user_login table has a one-to-many relationship with the cart table via user_id.
- The product table has a one-to-many relationship with the cart table via prod_id.
- The user_login table has a one-to-many relationship with the order table via user_id.
![Screenshot (3175)](https://github.com/user-attachments/assets/4080cdc8-9f6f-429f-9090-660bd18f088c)

## Backend Modules:
- **mysqlConn.py:** makes connection between Python and MySQL.
- **product.py:** Contains functions such as add product , remove product and retrieve the list of products.
- **cart.py:** Contains functions such as add item into cart , remove item from the cart and view cart items.
- **order.py:** Contains functions such as create order details and view order details.
- **app.py:** This is the main Python file that triggers the entire Web-Application. This file contains flask app , routing url functions and  APIs to communicate between frontend and backend.


## Frontend templates folder:
- **login.html:** User login page.
- **register.html:** User registration page.
- **home.html:** Home page of grocery store.
- **products.html:** Products page where user sees available products.
- **orderDetails.html:** Order details page showing user's orders.
- **finalOrderDetail.html:** Detailed view of a specific order.
- **invoice.html:** Order invoice generation and display.


## Features:
**1. User Authentication & Session Management:**
- Implemented secure login and registration systems using Flask sessions, ensuring data integrity and user session management.
- Stored user credentials and information securely in the user table within the MySQL database.

**2. Product Management with Full CRUD Functionality:**
- Enabled administrators to perform CRUD operations (Create, Read, Update, Delete) on product data, allowing for easy management of the store’s inventory.
- Product details, including names, prices, and descriptions, are stored and managed in the product table.

**3. Shopping Cart with Real-Time Updates:**
- Developed a dynamic shopping cart system where users can add, update, or remove products, with changes reflected in real-time.
- The cart table in the database tracks all items added by each user, ensuring accurate order processing.

**4. Order Processing and Management:**
- Facilitated smooth order placement by integrating a comprehensive order management system, allowing users to review their cart items and finalize purchases.
- Implemented features to store and retrieve order details in the order table, with automatic total price calculation.

**5. Responsive and User-Centric Design:**
- Designed the frontend using Bootstrap to ensure the application is fully responsive and optimized for various devices, providing a consistent user experience across desktops, tablets, and smartphones.
- Created an intuitive user interface that enhances the shopping experience, making navigation and interaction effortless.

**6. Efficient Database Interaction with MySQL:**
- Connected the application to a MySQL database using a custom Python module (mysqlConn.py), enabling efficient data handling.
- Wrote optimized SQL queries to perform operations on the user, product, cart, and order tables, ensuring fast and reliable data processing.

**7. Seamless API Integration for Frontend-Backend Communication:**
- Built and integrated custom APIs to handle data requests and responses between the frontend and backend, enabling real-time data interaction and smooth user experiences.



## Tools and Technologies Used: 🛠

- **Frontend: HTML , CSS , Bootstrap**
- **Backend: Python**
- **Web Framework: Flask** - Used for backend logic, routing URLs, and integrating with the frontend.
- **Database: MySQL** - Stores user data securely.


## Installation Instructions 🛣

1. Clone the repository:
```bash
git clone <Paste repository link here>
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```
Required packages:
- mysql-connector-python
- flask
- flask-session

3. Set up MySQL:
- Download and install MySQL on your local system
- Update the MySQL connection details in `mysqlConn.py` with your credentials

4. Run the application:
```bash
python app.py
```

5. Access the application:
- Open your web browser and navigate to `http://localhost:5000`
- Register a new account or login with existing credentials
- Start exploring the grocery store management system




## Usage Instructions 🛣

1. Run the application:
```bash
  python app.py
```

2. Access the application:
- Open a web browser and go to http://localhost:5000 or http://127.0.0.1:5000.
- You will see the login page.

3. Login or Register:
- If you have an account, log in using your credentials to visit the Grocery Store.
- If you don't have an account, click on "Create Account" to register.
- After registration, you will be redirected to the login page.

<div class="text-center">
  <h1>😍THANK YOU !😍</h1>
</div>
