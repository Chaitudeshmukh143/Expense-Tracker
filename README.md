# Expense-Tracker
A Java-based web app to track income and expenses using JSP, Servlets, JDBC, and Oracle DB. Users can add, view, and analyze transactions with totals and net balance. Simple UI, MVC structure, and deployed on Apache Tomcat. Ideal for personal finance management and learning Java web dev.  


# Expense Tracker Web Application

A simple Java-based web application to manage and track your income and expenses.

## 🧾 Features

- Add and store income and expense transactions
- View all transactions in a table format
- Summarize total income, total expenses, and net balance
- Filter transactions by type (income/expense)
- Clean and responsive JSP UI
- Built using MVC architecture

## 🛠️ Technologies Used

- Java (JSP, Servlets)
- Oracle Database
- JDBC (Java Database Connectivity)
- HTML/CSS
- Apache Tomcat

## 💡 Project Structure

- `transactionForm.jsp`: Add transaction form
- `viewTransactions.jsp`: Displays all transactions
- `SummaryServlet.java`: Computes totals and balance
- `TransactionDAO.java`: Handles DB operations

## 📦 How to Run

1. Import the project in your IDE (like Eclipse or IntelliJ)
2. Configure Oracle DB credentials in `TransactionDAO.java`
3. Deploy on Apache Tomcat server
4. Open in browser: `http://localhost:8080/ExpenseTracker/`

## 📁 Database Setup

```sql
CREATE TABLE transactions (
    id NUMBER PRIMARY KEY,
    type VARCHAR2(20),
    category VARCHAR2(50),
    amount NUMBER(10,2),
    transaction_date DATE
);
