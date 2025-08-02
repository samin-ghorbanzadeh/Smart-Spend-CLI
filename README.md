# Smart-Spend-CLI
Phase 2 of the Personal Expense Tracker project — includes modular code, data visualization with Matplotlib, and advanced CLI functionality

# Personal Expense Tracker CLI

This project is a command-line interface (CLI) tool for managing personal expenses. It was built as part of a Python training exercise to practice OOP, file handling, data visualization, and CLI development.

## Features

- **Add Expenses**: Add new expense entries with validation for amount, date, and category.
- **View Expenses**: View expenses with filters such as recent entries, category, and date range.
- **Summary Report**: Generate a summary including total expenses, category-wise sums, and daily averages.
- **Visualization**: Plot bar and line charts showing spending by category and daily spending trends.
- **Data Persistence**: All expense data is saved and loaded from a CSV file ('expenses.csv').

## Installation

1. Make sure you have Python 3.7+ installed.
2. Install required packages:

   pip install matplotlib

## Usage

The main entry point is 'main.py'. It supports the following commands:

* **Add an expense**

  python main.py add --amount 40 --date 2025-07-12 --category groceries --description "Weekly shopping"

* **View expenses**
  Show last 10 expenses by default:

  python main.py view
 
  Filter by category:

  python main.py view --category food

  Filter by date range:

  python main.py view --from 2025-07-01 --to 2025-07-15

* **Summary report**

  python main.py summary

* **Visualize expenses**

  python main.py visualize

## Project Structure

expense_tracker/
├── data/
│   ├── expenses.csv
│   └── reports/
│       ├── category_spending_bar.png
│       └── daily_expense_line.png
├── main.py
├── expense.py
├── expense_manager.py
├── report.py
├── visualize.py
├── utils.py
└── README.md

