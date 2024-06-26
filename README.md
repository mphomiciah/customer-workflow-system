# customer-workflow-system

## Introduction

This project is a web-based workflow system that allows users to input customer information via an HTML form and upload an Excel file containing the customer's financial income and expenses for the last 12 months. The system processes the uploaded file, stores the data in a database, and renders a temporal graph showing the customer's income and expenditure.

## Requirements

- Python
- Flask
- SQLite
- Pandas
- openpyxl

## Setup

1. Clone the repository.
2. Create a virtual environment: `python -m venv venv`
3. Activate the virtual environment:
    - On Windows: `venv\Scripts\activate`
    - On Unix or MacOS: `source venv/bin/activate`
4. Install the required dependencies: `pip install -r requirements.txt`
5. Start the Flask development server: `python app.py`
6. Open your browser and navigate to `http://localhost:5000`.
7. To view graph open your browser and navigate to`http://localhost:5000/graph`

## Assumptions

- The uploaded Excel file should have the format: month, income, expense (in the first three columns).
- The system is designed for a single user with no need for login or user management.

## Architectural Decisions

- **Flask**: Chosen for simplicity and ease of use.
- **SQLite**: Chosen for its simplicity and zero-configuration.
- **File Upload Handling**: Handled directly in Flask with the `openpyxl` library for processing Excel files.
- **Extensibility**: The solution is modular, making it easy to extend or modify.
