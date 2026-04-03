# Scikit-Learn-x-Matplotlib-Kaggle-data-observations
3 observations of Kaggle and sklearn visualized with Matplotlib

Analysis of the loan visualization
Based on the visual analysis of the provided loan dataset, several key trends emerge. First, the histogram of loan amounts reveals that most borrowers request relatively small sums, with the majority of loans falling under £10,000, despite significant outliers at the higher end. Second, the bar chart of income versus home ownership indicates a strong financial correlation: individuals with mortgages or high property ownership status consistently report higher average annual incomes (£81,000+) compared to renters (£55,000). Finally, the pie chart of loan intentions shows that "Education" and "Medical" costs are the leading drivers of loan requests, suggesting that life necessities are more common reasons for debt than luxury ventures or personal home improvements. These conclusions were derived by comparing the central tendencies and categorical distributions across the cleaned dataset.


Project Purpose
The purpose of this project is to perform exploratory data analysis (EDA) using Python and Matplotlib. By visualizing both biological (Iris) and financial (Loan) datasets, we can identify patterns, distinguish species traits, and understand the socioeconomic trends driving loan applications.

Class Design and Implementation
The project is implemented using the DataVisualizer class to encapsulate all data-related operations.

Attributes:

loan_csv_path: A string representing the path to the CSV data.

loan_df: A Pandas DataFrame holding the processed loan data.

iris_df: A Pandas DataFrame holding the Iris dataset.

Methods:

__init__(path): Initializes class parameters.

load_data(): Orchestrates the loading of multiple data sources.

clean_loan_data(): Performs critical data cleaning, such as removing currency symbols from loan_amnt and handling extreme outliers in employment_duration.

plot_iris_visuals(): Generates scatter and box plots to differentiate between Setosa, Versicolor, and Virginica species.

plot_loan_visuals(): Creates a histogram, bar chart, and pie chart to analyze loan characteristics.

Limitations:

The script assumes the input CSV follows a specific naming convention for columns.

The employment_duration cleaning method uses a hard limit (60 years) to filter out unrealistic data entries (e.g., 123 years).

Generative AI Disclosure
This project was developed with the assistance of a large language model. The chat logs documenting the design process and troubleshooting steps are included in this repository as part of the submission requirements.


Created using AI, chat link: https://gemini.google.com/share/97a4b0219b73
