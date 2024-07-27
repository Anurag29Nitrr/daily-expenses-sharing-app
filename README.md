# Daily Expenses Sharing Application #Backend intern assignment

This is a simple backend application for managing daily expenses and generating balance sheets. It allows users to add expenses, view their own expenses, and download a balance sheet in PDF format.

## Getting Started

Follow these instructions to set up and run the project locally.

### Prerequisites

- [Node.js](https://nodejs.org/) (version 14 or higher)
- [MongoDB](https://www.mongodb.com/try/download/community) (running locally or using a cloud service)
- A `.env` file to store environment variables

### Setup

1. **Clone the Repository**

   ```bash
   git clone https://github.com/yourusername/daily-expenses-sharing-app.git
   cd daily-expenses-sharing-app
   ```

2. **Install Dependencies**

   Install the required Node.js packages using npm:

   ```bash
   npm install
   ```

3. **Create a `.env` File**

   Create a `.env` file in the root directory of the project and add your MongoDB connection URI:

   ```env
   MONGODB_URI=mongodb://localhost:27017/expenses_db
   PORT=3000
   ```

   Replace `mongodb://localhost:27017/expenses_db` with your MongoDB URI if you're using a different setup.

4. **Run the Application**

   Start the server with the following command:

   ```bash
   npm start or node app.js 
   ```

   The application will run on `http://localhost:3000`.

### API Endpoints

- **User Endpoints:**
  - `POST /api/users` - Create a new user.
  - `GET /api/users/:id` - Get details of a specific user.
  - `GET /api/users` - Get a list of all users.

- **Expense Endpoints:**
  - `POST /api/expenses` - Add a new expense.
  - `GET /api/expenses/user/:id` - Get expenses for a specific user.
  - `GET /api/expenses` - Get all expenses.
  - `GET /api/expenses/all` - Get all expenses (same as above).
  - `GET /api/expenses/balance-sheet` - Download the balance sheet as a PDF.
