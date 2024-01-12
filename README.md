# Life_expectancy_analysis

## Task #2 - Regression

- If you submit the assignment after the first deadline but before the final deadline, you will receive a penalty of -12 points. Late submissions will not receive any points.

In this task, you will deal with a regression problem, various types of features, and missing values.

- Before building a predictive model, you need to somehow convert the features into a numerical representation.

The tasks are designed to allow for creativity. Figuring out how to solve them precisely is an essential part of the assignment, and originality and creativity will also be evaluated!

- Use Markdown cells to explain your approach. Points will be deducted for unclear explanations.

**Data Source**

We will predict life expectancy in different countries and years. You have training data in the file `data.csv` and evaluation data in the file `evaluation.csv`.

**List of features:**

- Year - Year
- Status - Developed or developing country
- Life expectancy - Life expectancy in years - the target variable you will predict
- Adult Mortality - Adult mortality rate (probability that individuals aged 15 will die before reaching age 60, per 1,000 individuals)
- Infant deaths - Number of infant deaths per 1,000 population
- Alcohol - Alcohol consumption per capita (age 15+) (in liters of pure alcohol)
- Percentage expenditure - Expenditure on health as a percentage of gross domestic product per capita (%)
- Hepatitis B - Hepatitis B vaccination coverage among 1-year-olds (%)
- Measles - Measles cases reported per 1,000 population
- BMI - Average Body Mass Index of the entire population
- Under-five deaths - Number of under-five deaths per 1,000 population
- Polio - Polio vaccination coverage among 1-year-olds (%)
- Total expenditure - Government expenditure on health as a percentage of total government expenditure (%)
- Diphtheria - Diphtheria, tetanus, and pertussis (DTP3) vaccination coverage among 1-year-olds (%)
- HIV/AIDS - Number of deaths of children aged 0-4 due to HIV/AIDS (per 1,000 live births)
- GDP - Gross domestic product per capita (in USD)
- Population - Population of the country
- Thinness 1-19 years - Percentage of children aged 10-19 with BMI less than two standard deviations below the median (%)
- Thinness 5-9 years - Percentage of children aged 5-9 with BMI less than two standard deviations below the median (%)
- Income composition of resources - Human Development Index in terms of income composition of resources (index ranging from 0 to 1)
- Schooling - Number of years of schooling (years)

**Instructions for Completion**

1. Load the data from the `data.csv` file in the notebook. Divide the data into subsets suitable for training (training), model comparison (validation), and predicting the performance of the final model (testing).

2. Perform basic data preprocessing:
   - Go through each feature and transform it into a suitable form for use in the selected regression model.
   - Deal with missing values in some way. Be cautious about methodological errors!
   - You can use visualizations as well. Comment briefly but sufficiently on everything.

3. Create your own implementation of a random forest. Use the prepared skeleton below for this purpose.

4. Apply your previous implementation of the random forest model to the prepared data, as well as one of the linear regression or ridge regression models, and at least one other model of your choice. For each of these models, do the following:
   - Comment on the suitability of the model for the given task.
   - Experiment with normalization (standardization/min-max) if you expect a favorable impact on the model.
   - Choose the main hyperparameters to tune and find their best values (in terms of RMSE).
   - For the model with the best hyperparameter values, calculate its error using RMSE and MAE. Be careful about methodological errors!

5. From all the options you've tried in the previous step, select the final model and estimate the error (RMSE) you can expect on new data that you haven't had access to so far. Be careful about methodological errors!

6. Finally, load the evaluation data from the `evaluation.csv` file. Use the final model to calculate predictions for this data. Create a `results.csv` file in which you store the obtained predictions using three columns: Country, Year, and Life expectancy. Submit this file as well (save it in the repository next to the notebook).

**Sample of the first rows of the `results.csv` file:**

Country,Year,Life expectancy
Peru,2012,71.4
Peru,2013,72.6

