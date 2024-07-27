# Daily Expenses Sharing Application

## Setup and Installation

1. Clone the repository:
   ```bash
   git clone <repository_url>
   cd daily-expenses-sharing-app

Install dependencies: npm install

Create a .env file in the root directory and add your MongoDB connection string: MONGODB_URI=your_mongodb_connection_string

Start the server: npm start


API Endpoints
User Endpoints
Create User: POST /users
Retrieve User Details: GET /users/:id

Expense Endpoints
Add Expense: POST /expenses
Retrieve Individual User Expenses: GET /expenses/user/:id
Retrieve Overall Expenses: GET /expenses


Validation
Ensure percentages in the percentage split method add up to 100%.