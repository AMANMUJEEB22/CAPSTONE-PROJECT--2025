# **Analyzing and Visualizing UNESCO Education Statistics**
The UNESCO Institute for Statistics (UIS) is the authoritative source for globally comparable data on education, science, culture, and communication. As UNESCO’s official statistical agency and custodian of Sustainable Development Goal 4 (Quality Education), UIS provides critical data to guide policies and investments that shape the future of education worldwide.This project utilizes the UIS dataset to carry out thorough data cleaning, preprocessing, and visualization. The focus is on extracting meaningful insights and trends in education statistics, particularly regarding Information and Communication Technology (ICT) graduates across various countries and years.By removing irrelevant metadata and handling missing or duplicate data, the project refines the raw dataset into a clear, analyzable form. Renaming columns and organizing data prepares it for effective visualization and further analysis.
# Data Cleaning and Visualization of UNESCO Education Data
Step 1: Dataset Loading
We began by importing the UNESCO UIS dataset (CSV format) into a Pandas DataFrame using Python. This step reads the raw data into memory so it can be processed and analyzed.
Step 2: Data Cleaning – Removing Unnecessary Columns
The original dataset contained many metadata columns that were not useful for analysis (e.g., STRUCTURE, FREQ, UNIT_TYPE, etc.). These were dropped to simplify the dataset and improve focus.
Step 3: Checking for Missing and Duplicate Values
To ensure data quality, we checked for:
Null (missing) values using isnull().sum()
Duplicate rows using duplicated().sum()
These checks help ensure the integrity of the dataset before visualization.
Step 4: Renaming Columns for Clarity
Several column names were long or unclear. We renamed key columns for readability and easier analysis. For example, REF_AREA_LABEL was renamed to Country, and OBS_VALUE to Value.
Step 5: Data Visualization
Using matplotlib and seaborn, we visualized trends in ICT-related education statistics. For example, we plotted the total number of ICT graduates by year to identify growth patterns and country-level trends.
# Model Building & Performance Evaluation (Visualization) 
In this stage of the project, five regression models were built: Linear Regression, Lasso Regression, Support Vector Regressor (SVR), Random Forest, and XGBoost. The models were trained using the cleaned and preprocessed dataset. Each model was evaluated using performance metrics such as Root Mean Squared Error (RMSE) and R² score. These metrics helped assess how accurately the models predicted the target variable. A comparison of all model performances was visualized using bar charts, providing a clear view of their effectiveness. Among the models, the one with the highest R² score and lowest RMSE was selected as the best-performing model. Additionally, feature importance was analyzed for tree-based models like Random Forest and XGBoost. This helped identify the most significant factors influencing the model's predictions. The evaluation process ensured that the final model chosen was both accurate and reliable. These results formed the basis for the final insights and conclusions of the project.
#  Project Summary
This project involved analyzing and visualizing education-related data from the UNESCO UIS dataset. The data was first cleaned by removing unnecessary metadata columns and renaming the relevant ones for clarity. Missing values and duplicates were checked to ensure data quality. Exploratory data analysis and visualizations were used to uncover trends in indicators, particularly focusing on ICT-related metrics across different countries and years. Multiple regression models such as Linear Regression, Random Forest, XGBoost, Lasso, and SVR were trained to predict educational indicators. Their performances were evaluated using RMSE and R² scores and visualized for comparison.
# Conclusion
The machine learning models developed provided valuable insights into the trends and patterns in global education data. Among the models, [Insert Best Model] showed the best performance based on R² and RMSE values. The analysis highlighted the influence of various features in predicting education outcomes, especially in the context of ICT development. Overall, this project demonstrated how data science and machine learning can be effectively applied to understand and predict educational trends, supporting data-driven decision-making for policy and development. Future improvements could include using more recent data, additional indicators, or interactive dashboards for better presentation.








