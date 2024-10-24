# pionex_Alpha
This code cleans and processes a Pionex user database. It handles missing values, standardizes formats, and validates email addresses. The output is two CSV files: 'cleanPionex.csv' with validated data, and 'garbagePionex.csv' containing invalid records.

# Pionex User Data Cleaning

This project cleans and processes a CSV file containing user data from Pionex, a cryptocurrency trading platform. It addresses issues like missing values, inconsistent formatting, and invalid email addresses to produce a clean and usable dataset.

## Process

The code performs the following steps:

1. **Data Loading and Initial Cleaning:** Loads the CSV into a Pandas DataFrame, identifies missing values, and removes unnecessary columns.
2. **Data Formatting:** Standardizes the format of 'RegistrationDate', 'First Name', 'Last Name', and 'Phone' columns.
3. **Handling Missing Values:** Replaces empty fields with the word 'Void'.
4. **Renaming Columns:** Renames columns to a more consistent and readable format.
5. **Column Reordering:** Arranges columns in a specific order for easier data analysis.
6. **Data Validation and Separation:** Extracts invalid data, including rows with missing values and invalid email addresses, into a separate file.
7. **Further Validation:** Checks NaN values and validates emails using regex.


## Input

- `241k-Singapore-pionex.com-Crypto-Trading-Bots-UsersDB-csv-2023.csv`: The original CSV file containing the raw Pionex user data.

## Output

- `cleanPionex.csv`: Contains the cleaned and validated user data.
- `garbagePionex.csv`: Contains rows with missing values or invalid email addresses.

## Dependencies

- Python 3.x
- Pandas library

## Usage

1. Make sure you have Python 3.x and the Pandas library installed. You can install Pandas using pip:


bash pip install pandas



2. Place the `241k-Singapore-pionex.com-Crypto-Trading-Bots-UsersDB-csv-2023.csv` file in the same directory as the Python script.
3. Execute the Python script.
