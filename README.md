# ETL_Peer_Project
Project Name: Bank Market Data ETL

Description:

Bank Market Data ETL is a Python project designed to automate the process of extracting, transforming, and loading (ETL) financial market data from various sources. The project focuses on extracting data from JSON and CSV files, transforming the data by converting market capitalization to GBP (£), and loading the transformed data into a CSV file for further analysis.

Features:
Extracts financial market data from JSON and CSV files.
Transforms market capitalization data from USD to GBP.
Logs the progress of the ETL process with timestamps.
Provides a structured workflow for automating ETL tasks.


Dependencies:
Python 3.x
Pandas: A Python library for data manipulation and analysis.
Glob: A module for selecting files in a directory.
Xml.etree.ElementTree: A module for processing XML files.
Datetime: A module for working with dates and times.

UsageTips:
Ensure Python and the required dependencies are installed.
Run the script in your Python environment to perform ETL operations on bank market data.


Functions:
extract_json_file(file_to_extract): Extracts data from a JSON file and returns a Pandas DataFrame.
extract_files(): Extracts data from JSON files in the directory and returns a combined Pandas DataFrame.
extract_csv_file(file_to_extract): Extracts data from a CSV file and returns a Pandas DataFrame.
transform_marketcap(df): Transforms market capitalization data from USD to GBP and updates the DataFrame accordingly.
load(dataframe, target_file): Writes the DataFrame to a CSV file.
log_now(message): Logs a message with a timestamp to a log file.


Sample Output:
After running the script, the transformed data will be saved in a CSV file named "transformed_data.csv". Log messages will be recorded in "logfile.txt" indicating the progress of the ETL process.
