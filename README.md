# Food Ordering System - README

Welcome to the **Food Ordering System** built with Python! This system allows users to browse through menus, add food items to their cart, place orders, and complete payments. It also provides an administrative interface for managing restaurants, orders, and users.

## Features

### User Features
- **Browse Menus:** View restaurants and their menus.
- **Add Items to Cart:** Add desired food items to your shopping cart.
- **Place Orders:** Review the cart and place an order.
- **Track Orders:** Monitor the status of your order.
- **Payment Processing:** Integration with payment gateways like Stripe or PayPal.
- **Order History:** View previous orders for quick reordering.

### Admin Features
- **Restaurant Management:** Admin can manage restaurant profiles, including adding, editing, or deleting restaurants.
- **Menu Management:** Admin can manage menus by adding or removing food items.
- **Order Management:** Admin can view and manage customer orders.
- **User Management:** Admin can manage user accounts, including activation or deactivation.

## Prerequisites

To run the Food Ordering System, you will need the following:

- **Python 3.x**
- **Flask** (for the backend)
- **SQLite** or **MySQL** (for database)
- **Stripe** or **PayPal API** for payment processing (optional)
- **Flask-SQLAlchemy** for ORM
- **Flask-Login** for user authentication
- **Requests** (for API calls)

### Install dependencies:
You can install all the required dependencies using pip:

```bash
pip install -r requirements.txt
```

## Installation

### Step 1: Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/yourusername/food-ordering-system-python.git
cd food-ordering-system-python
```

### Step 2: Setup the Database

1. Install SQLite or MySQL for the database (SQLite is used for simplicity in this example).
2. Create the database by running:

```bash
python create_db.py
```

This will create the necessary tables (users, orders, menus, etc.) in your database.

### Step 3: Configure Environment Variables

Create a `.env` file in the root directory of the project and add the following variables:

```
SECRET_KEY=your_secret_key
DATABASE_URL=sqlite:///food_ordering.db  # or your MySQL database connection string
STRIPE_API_KEY=your_stripe_api_key  # if using Stripe
PAYPAL_CLIENT_ID=your_paypal_client_id  # if using PayPal
```

### Step 4: Run the Application

To start the development server, run:

```bash
python app.py
```

By default, the application will be available at `http://127.0.0.1:5000`.

### Step 5: Access the Frontend

The frontend will be served through the Flask backend. You can access the application in your web browser by navigating to:

- **Frontend:** `http://localhost:5000`
- **Backend (API):** The backend routes are integrated directly into the Flask app.

## Usage

Once the system is running, you can:

- **Register and Log In** as a user to place orders.
- **Browse restaurants** and add food items to the cart.
- **Place and track orders** after confirming the payment.

### User Workflow:
1. Register/Login: Create a new user or log in to your existing account.
2. Browse Menus: Select a restaurant and view its menu.
3. Add to Cart: Add food items to your shopping cart.
4. Checkout: Review the cart, provide delivery details, and complete the payment.
5. Track Order: Check the status of your order in real time.

### Admin Workflow:
1. Log in with admin credentials.
2. Manage restaurants: Add/edit/remove restaurant listings.
3. Manage menu items: Edit or remove menu items.
4. View and manage orders: Track user orders and update their status.

## Technologies Used

- **Backend Framework:** Flask (Python)
- **Database:** SQLite or MySQL (SQLAlchemy ORM)
- **User Authentication:** Flask-Login
- **Payment Gateway:** Stripe / PayPal (depending on configuration)
- **Frontend:** HTML, CSS, JavaScript (optional integration with frontend frameworks like React)
- **Deployment:** Can be deployed on any server (Heroku, AWS, etc.)

## Contributing

We welcome contributions to improve the Food Ordering System! If you want to contribute, fork the repository, make your changes, and submit a pull request.

Ensure your changes are well-documented and follow the coding standards.

## License

This project is licensed under the MIT License.

---

**Food Ordering System** built with Python - A complete solution for online food ordering.

For support or inquiries, contact us at: proind32@gmail.com
