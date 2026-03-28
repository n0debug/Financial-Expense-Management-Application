# Financial-Expense-Management-Application
Managing personal finances manually is often confusing and unorganized. People forget where their money goes and struggle to monitor income, expenses, and savings effectively. This application helps users record, categorize, and analyse their income and expenses to improve financial planning.

Finance Mnagement App (Java)
A lightweight, console-based Java application designed to help users manage their personal finances. This tool allows for the tracking of income and expenses with persistent storage, ensuring your financial data is saved even after the program closes.

Project Overview :
    This application serves as a digital ledger. It captures four key data points for every entry: Date, Type (Income/Expense), Category, and Amount. By storing data in a local text file, it provides a simple yet effective way to monitor your remaining balance and spending habits without needing a complex database.

Features :
Full CRUD Operations: Add, View, Update, and Delete financial records.

Automatic Date Stamping: Uses java.time.LocalDate to automatically tag entries with the current date.

Persistent Storage: Saves all records to a data.txt file automatically after every change.

Financial Summaries: * Totals: Instant calculation of Total Income, Total Expense, and Remaining Balance.

Category Analysis: Grouped summaries showing how much you've spent or earned per category (e.g., Salary, Food, Travel).

Error Handling: Robust validation for numeric inputs to prevent program crashes.

Technical Stack :

Language: Java 8+

Storage: Flat-file System (data.txt)

Core Logic: ArrayList for in-memory processing and HashMap for category-based aggregation.

Getting Started
Prerequisites
Java Development Kit (JDK) installed on your machine.

A terminal or command prompt.

Installation & Running
Clone or Copy the Code: Save the code into a file named FinanceApp.java.

Compile the Program:

Bash
javac FinanceApp.java
Run the Application:

Bash
java FinanceApp

How to Use
Main Menu: Upon launching, choose an option from 1 to 8.

Adding Records: When adding income or expenses, the app will ask for a category and an amount. The date is handled automatically.

Updating/Deleting: View your records first (Option 3) to find the index number of the entry you wish to modify or remove.

Data Storage: A file named data.txt will be created in the same directory. You can open this file to see your raw data, but do not manually edit its format to avoid loading errors.

Project Structure :
Plaintext

FinanceApp.java    # Main source code containing all logic
FinanceApp.class   # Compiled bytecode (generated after javac)
data.txt           # Persistent storage file (generated at runtime)

Important Note on Data Format
The application expects the data.txt file to follow this specific comma-separated format:
YYYY-MM-DD, Type, Category, Amount

Example: 2026-03-25, Income, salary, 5000.0
