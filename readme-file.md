# Highridge Construction Company - Worker Payment System

This repository contains a payment processing system for Highridge Construction Company to facilitate weekly payments to workers. The system is implemented in both Python and R.

## Features

- Dynamically generates data for 400 workers with realistic attributes
- Processes weekly payments and generates individual payment slips
- Implements conditional logic for employee level assignment:
  - If salary > $10,000 and < $20,000, employee level is "A1"
  - If salary > $7,500 and < $30,000 and employee is female, level is "A5-F"
- Includes exception handling for error management
- Provides implementations in both Python and R
- Generates summary reports of worker data
- Displays a list of workers with their names, salaries, and employee levels

## Requirements

### Python Version
- Python 3.6+
- Required packages: 
  - pandas
  - datetime
  - random
  - os

### R Version
- R 3.5+
- Required packages:
  - dplyr
  - lubridate

## Installation

1. Clone this repository or download the ZIP file
2. Extract the contents to your desired location
3. Install the required dependencies:

For Python:
```bash
pip install pandas
```

For R:
```R
install.packages(c("dplyr", "lubridate"))
```

## Usage

### Python Implementation

To run the Python version:

1. Open a terminal/command prompt
2. Navigate to the repository directory
3. Run the script:

```bash
python payment_system.py
```

This will:
- Generate data for 400 workers
- Process payments and determine employee levels
- Generate individual payment slips in the "payment_slips" directory
- Save worker data to "payment_slips/worker_data.csv"
- Display a summary report in the console
- Show a list of top 20 workers sorted by salary

### R Implementation

To run the R version:

1. Open R or RStudio
2. Set the working directory to the repository location
3. Source the script:

```R
source("payment_system.R")
```

or run:

```bash
Rscript payment_system.R
```

This will:
- Generate data for 400 workers
- Process payments and determine employee levels
- Generate individual payment slips in the "payment_slips_r" directory
- Save worker data to "payment_slips_r/worker_data.csv"
- Display a summary report in the console
- Show a list of top 20 workers sorted by salary

## Output

Both implementations will create:

1. A directory containing individual text files for each worker's payment slip
2. A CSV file with all worker data including employee levels
3. Console output showing:
   - Processing progress
   - Summary statistics with employee level distribution
   - A formatted list of workers with names, salaries, and employee levels

## Code Structure

### Python Version

- `generate_workers()`: Creates a list of worker dictionaries with random data
- `determine_employee_level()`: Applies conditional logic to determine employee level
- `generate_payment_slip()`: Formats payment information into a readable slip
- `process_payments()`: Main function that orchestrates the payment process
- Custom exception class for salary validation

### R Version

- `generate_workers()`: Creates a data frame of workers with random data
- `determine_employee_level()`: Applies conditional logic to determine employee level
- `generate_payment_slip()`: Formats payment information into a readable slip
- `process_payments()`: Main function that orchestrates the payment process
- `handle_error()`: Custom error handling function

## Author

Developed by ROWLAND M BERNARD for Highridge Construction Company

## License

This project is licensed under the MIT License - see the LICENSE file for details