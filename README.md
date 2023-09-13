# Pharmaceutical Treatment Testing using Pandas and Matplotlib

In this project for the UCI Data Analytics Bootcamp, I used Python to analyze pharmaceutical testing treatment data. The purpose of this study was to compare the performance of an anti-cancer medication, Capomulin, against the other treatment regimens. 

# Data Cleaning

Prepare the Data - drop duplicates
Run the provided package dependency and data imports, and then merge the mouse_metadata and study_results DataFrames into a single DataFrame.

Display the number of unique mice IDs in the data, and then check for any mouse ID with duplicate time points. Display the data associated with that mouse ID, and then create a new DataFrame where this data is removed. Use this cleaned DataFrame for the remaining steps.

Display the updated number of unique mice IDs.

# Summary Statistics 

Create two summary statistics DataFrames:

For the first DataFrame, use the groupby method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. This should result in five unique Series objects. Combine these objects into a single summary statistics DataFrame.

For the second DataFrame, use the agg method to produce the same summary statistics table by using a single line of code.

# Bar Charts 

Generate two bar charts. Both charts should be identical and show the total number of time points for all mice tested for each drug regimen throughout the study.

Create the first bar chart with the Pandas DataFrame.plot() method.

<img width="621" alt="Screen Shot 2023-09-07 at 8 53 04 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/ba72555b-b7d6-4d59-b9f2-2402b390a631">

Create the second bar chart with Matplotlib's pyplot methods.

<img width="622" alt="Screen Shot 2023-09-07 at 8 52 33 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/dde28eeb-2524-43d1-8e39-82721e7f2bc0">

# Pie Charts

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

![pie_chart1](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/523b88ed-5efa-4bb1-827e-6a002f308f32)

Create the second pie chart with Matplotlib's pyplot methods.


![pie_chart2](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/e6f10172-66b7-47a5-94e5-34def351f412)


# Quartiles, Outliers, and Box Plot

Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
1. Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
2. Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
3. Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
4. Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot of the final tumor volume for all four treatment regimens. Highlight any potential outliers in the plot by changing their color and style.

# Line Plot

Select a mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

# Scatter Plot 

Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

# Correlation

Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

# Regression 

Plot the linear regression model on top of the previous scatter plot.

# Summary



