# MDC-Task
### Project Title

**Superstore Sales Analysis and Forecasting**

This project performs an exploratory data analysis (EDA) on the Superstore sales dataset and uses a linear regression model to forecast future sales.

### Files in this Repository

  * `MDC_task.ipynb`: Jupyter Notebook containing the complete code for data loading, cleaning, visualization, and forecasting.
  * `Sample - Superstore.csv`: The dataset used for the analysis.

### Overview

The project follows a standard data science workflow:

1.  **Data Loading and Inspection**: The `Sample - Superstore.csv` file is loaded into a pandas DataFrame. Initial checks are performed to understand the data types and identify any missing values. The notebook first unzips `archive.zip` to get the CSV file, and then loads it using `pandas.read_csv` with the `latin1` encoding. It also checks for data types and missing values.
2.  **Data Preprocessing**: The 'Order Date' and 'Ship Date' columns are converted from object type to datetime objects to enable time-series analysis.
3.  **Exploratory Data Analysis (EDA)**: A monthly sales trend is visualized using a line plot to understand sales patterns over time. The notebook aggregates sales by month and creates an interactive line plot using `plotly.express`.
4.  **Forecasting**: A simple linear regression model from scikit-learn is trained on the historical monthly sales data to predict the sales for the next month.

### How to Run the Notebook

1.  **Environment Setup**: Ensure you have Python and the necessary libraries installed. You can install the required libraries using pip:
    ```bash
    pip install pandas plotly scikit-learn numpy
    ```
2.  **Download the Data**: Download the `archive.zip` file containing the `Sample - Superstore.csv` dataset and place it in the same directory as the notebook. The notebook is set to unzip this file.
3.  **Run the Notebook**: Open and run the `MDC_task.ipynb` notebook in a Jupyter environment (like JupyterLab, Google Colab, or VS Code with the Jupyter extension).

### Results and Findings

The notebook successfully loads and processes the dataset, converting the date columns to the correct format. It then generates a line plot showing the monthly sales trend over several years. Finally, a linear regression model is used to predict the sales for the next month.

The predicted sales for the next month are displayed at the end of the notebook.

uploaded image file.<img width="1500" height="522" alt="Screenshot 2025-08-15 120024" src="https://github.com/user-attachments/assets/2f2921fe-83ee-464a-9800-fff8322439c6" />
