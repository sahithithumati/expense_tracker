# Expense Tracker (CLI)

A tiny, single-file Python project to **log expenses** and **summarize spending** by category or month.
Perfect for a simple GitHub portfolio project.

## Features
- Add expenses (date, amount, category, note)
- List all expenses
- Summarize by category or by month
- Uses a simple CSV file for storage (no external dependencies)

## Quick Start
```bash
# 1) Ensure you have Python 3.8+
python --version

# 2) Clone or download the repo, then run:
python expense_tracker.py add --amount 12.5 --category Food --note "Lunch"
python expense_tracker.py list
python expense_tracker.py summary --by category
python expense_tracker.py summary --by month
```

The data file `expenses.csv` will be created in the same folder automatically.

## Example
```bash
python expense_tracker.py add --amount 1800 --category Rent --date 2025-10-01
python expense_tracker.py add --amount 45.20 --category Groceries --note "Market"
python expense_tracker.py add --amount 12 --category Transport --note "Bus"
python expense_tracker.py summary --by category
python expense_tracker.py summary --by month
```

## Project Structure
```
expense-tracker-cli/
├── expense_tracker.py
├── expenses.csv           # created automatically after first 'add'
├── README.md
├── .gitignore
└── LICENSE
```

## Why this project?
- Clean, readable code with docstrings and type hints
- Shows basic file I/O, CLI design with `argparse`, and simple reporting
- No external libs → easy to run anywhere

## License
MIT
