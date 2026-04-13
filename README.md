# Data-Processing-Challenge
This project demonstrates foundational data engineering skills by processing a complex user dataset using standard Python libraries only. The goal was to perform data extraction, cleaning, and transformation without the use of high-level data analysis libraries like pandas or seaborn.
To make your GitHub repository look professional, your README should clearly state the project's purpose, the specific constraints you worked under, and how to use the code.

## Project Overview
This project demonstrates foundational data engineering skills by processing a complex user dataset using **standard Python libraries only**. The goal was to perform data extraction, cleaning, and transformation without the use of high-level data analysis libraries like `pandas` or `seaborn`.

The project involves handling a CSV dataset (`acw_user_data.csv`) containing user information, employment details, and vehicle data.

## Key Features & Tasks
The notebook is structured into several tasks that reflect real-world data processing workflows:

* **Custom Data Extraction:** Reading and parsing CSV data into native Python data structures (lists of dictionaries).
* **Data Quality & Cleaning:** Identifying and fixing "problematic entries" in the dataset. Specifically, empty strings in the `Dependants` column were programmatically identified and replaced with "0" to ensure data integrity.
* **Schema Transformation:** Extracting specific nested information, such as vehicle details (Make, Model, Year, Type), and casting them into appropriate data types (e.g., converting years to integers).
* **Persistent Storage:** Saving cleaned datasets to new CSV files and exporting specific subsets to JSON format for downstream use.

## Constraints
As part of this challenge, the following rules were applied to the final logic:
* **No Pandas:** All data manipulation was done using the core `csv` and `json` modules.
* **Standard Library Only:** Used `os`, `sys`, and `time` for environment management and performance tracking.

## File Structure
* `Final Assesment.ipynb`: The main Jupyter Notebook containing the development process and final solutions.
* `acw_user_data.csv`: The raw input dataset.
* `AA_acw_user_data.csv`: The cleaned version of the dataset produced by the notebook.
* `VehicleDetails.json`: (Generated) A structured JSON export of vehicle-specific data.

## How to Use
1.  Ensure you have a standard Python 3 installation.
2.  Clone this repository.
3.  Open `Final Assesment.ipynb` in Jupyter Notebook or VS Code.
4.  Run the cells labeled **"FINAL ANSWER"** to execute the data processing pipeline.
