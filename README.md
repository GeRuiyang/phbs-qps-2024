# phbs-qps-2024

## Project Overview
This project provides functionality for fetching CPI data from the Federal Reserve Economic Data (FRED) and calculating inflation rates over the last four quarters. It aims to help users analyze economic trends and understand key inflation metrics.

## GitHub Repository URL
[phbs-qps-2024 GitHub Repository](https://github.com/GeRuiyang/phbs-qps-2024)

---

## Setup and Running Instructions

### 1. Clone the Repository

Clone the repository to your local machine using the following command:

git clone https://github.com/GeRuiyang/phbs-qps-2024.git

### 2. Navigate to the Project Folder

Change into the directory where the repository was cloned:

    cd phbs-qps-2024

### 3. Set Up the Python Environment

Make sure you have Python 3.8+ installed. Then, install the necessary dependencies by running:

    pip install -r src/requirements.txt

This will install all required packages listed in the requirements.txt file.

### 4. Run the Script to Fetch CPI Data and Calculate Inflation

Once the environment is set up, you can run the script that fetches CPI data and calculates the inflation:

    python scripts/fetch_cpi_data.py

This will download the CPI data from FRED, resample it to quarterly averages, and calculate the inflation rate as the percentage change over the past 4 quarters.

### 5. Output

The script will display the last 4 quarters of inflation data, including:

- CPI values for the last 4 quarters
- Inflation rate (in percentage) based on the percentage change in CPI over the past 4 quarters

## Script Overview

The primary script fetch_cpi_data.py does the following:

- Fetches CPI data from the Federal Reserve Economic Data (FRED) for the specified date range.
- Resamples the data to a quarterly frequency and calculates the quarterly average.
- Computes the inflation rate as the percentage change over the past 4 quarters.
- Outputs the most recent 4 quarters of inflation data.

## Script Workflow

- The script fetches CPI data from FRED using the pandas_datareader library.
- It then resamples the data to get the quarterly average of CPI values.
- It calculates the inflation rate based on the percentage change in CPI over the last 4 quarters.
- Finally, the script prints the last 4 quarters of inflation data to the console.

## Troubleshooting

If you encounter any issues during installation or while running the script, here are some things to check:

- Missing Dependencies: Ensure all dependencies are installed by checking the requirements.txt file.
- Internet Connection: The script fetches data from FRED, so a working internet connection is required.
- Python Version: Make sure you are using Python 3.8+.

For further assistance, please open an issue on the GitHub repository.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
