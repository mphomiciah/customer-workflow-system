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

1. **Clone the repository:**
   ```bash
   git clone https://github.com/mphomiciah/customer-workflow-system.git
   cd customer-workflow-system
2. Verify Python installation by opening a command prompt (CMD) and typing `python --version`.
3. If you don't have python, Install Python from [python.org](https://www.python.org/downloads/).
4. Create and activate a virtual environment (python -m venv venv, source venv/bin/activate).It's optional, you cn skip this step if you want.
5. Install `pip`, the Python package installer, by following the [pip installation guide](https://pip.pypa.io/en/stable/installation/).
6. Once `pip` is installed, navigate to the project directory in CMD.
7. Install the required dependencies using the command: `pip install -r requirements.txt`.
8. Run the application:
   ```bash
   python app.py
   ```
   Open `http://localhost:5000` in your web browser.

## Assumptions

- The uploaded Excel file should have the format: month, income, expense (in the first three columns).

## Usage

1. **Upload File:**
    - Navigate to `http://localhost:5000`.
    - Fill in the form with first name, last name, and date of birth.
    - Upload an Excel file containing monthly financial data.

2. **View Graph:**
    - After uploading, the system redirects to a page displaying the generated bar graph.
    - The graph is saved in the `static` folder with a unique filename.

## Technologies Used

- **Flask:** Web framework for Python.
- **SQLite:** Lightweight relational database management system.
- **matplotlib:** Data visualization library in Python.
- **openpyxl:** Library to read/write Excel files.
- **Bootstrap**: Frontend framework for styling HTML templates.