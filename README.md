# EXPENSE-TRACKER

Expense Tracker Application

Overview:
This is an Expense Tracker web application built using React for the frontend and a backend that manages transactions (incomes and expenses). It allows users to view and track their financial records, showing their income, expenses, and balance, while sorting the transactions by date. The app also displays graphical insights with the help of a chart.

The app fetches income and expense data from the backend, calculates totals, and organizes transactions into Income and Expense sections. The backend API handles CRUD operations for the transactions.

Features:
    -> Dashboard View: Displays a summary of total income, total expenses, and total balance.
    -> Transaction List: View detailed income and expense records, sorted by date.
    -> Chart Visualization: Graphical representation of income vs. expense data.
    -> Min/Max Calculation: View the minimum and maximum income/expense values.


Technologies Used

Backend:

    Node.js
    Express.js
    MongoDB
    API for fetching and managing incomes and expenses

Frontend:

    React
    Styled Components
    Chart.js (for data visualization)
    React Context API (for global state management)
    React Router (for routing)
    Axios (for API calls)

Styling:

    CSS (with Styled Components for custom styling)


Setup and Installation:

Prerequisites:
    Node.js (v14 or above)
    MongoDB or any other database
    Git

Frontend Setup:

    Clone this repository to your local machine:
    git clone https://github.com/Nishaanth-44/EXPENSE-TRACKER.git
    cd expense-tracker

    Install the required dependencies:
    npm install

    Start the development server:
    npm start

    Visit the application in your browser at http://localhost:3000.


Backend Setup:

    Navigate to the backend directory:
    cd backend

    Install the backend dependencies:
    npm install

    Start the backend server:
    npm start

    The API should be running on http://localhost:5001 (or http://localhost:5000).





How the Application Works

Dashboard:
    -> The dashboard shows the total income, total expenses, and the balance (income - expenses).
    -> The data is fetched from the backend via API calls when the component mounts.
    -> The total income, total expense, and balance are calculated from the fetched data.

Incomes and Expenses Sections:
    -> The app provides two sections: one for Income and one for Expense.
    -> Both sections are sorted by date, with the most recent transactions appearing first.
    -> Each transaction displays its date and amount.

Chart:
    -> A chart is rendered using Chart.js to visualize the comparison between total income and total expenses.

Min/Max Values:
    -> The minimum and maximum values for income and expense are calculated and displayed.





API Endpoints:

Incomes
-> GET /api/incomes
    Fetches all the income records.
    Returns an array of income objects with amount, date, etc.

-> POST /api/incomes
    Adds a new income record.
    Request body should include amount and date fields.

-> PUT /api/incomes/:id
    Updates an existing income record by ID.
    Request body should include updated amount and date fields.

-> DELETE /api/incomes/:id
    Deletes an income record by ID.
    
Expenses
-> GET /api/expenses
    Fetches all the expense records.
    Returns an array of expense objects with amount, date, etc.

-> POST /api/expenses
    Adds a new expense record.
    Request body should include amount and date fields.

-> PUT /api/expenses/:id
    Updates an existing expense record by ID.
    Request body should include updated amount and date fields.

-> DELETE /api/expenses/:id
    Deletes an expense record by ID.
