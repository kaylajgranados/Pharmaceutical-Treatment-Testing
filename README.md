# Pharmaceutical Treatment Testing using Pandas and Matplotlib

In this project for the UCI Data Analytics Bootcamp, I used Python to analyze pharmaceutical testing treatment data. The purpose of this study was to compare the performance of an anti-cancer medication, Capomulin, against the other treatment regimens. 

# Merge data 

Prepare the Data 
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

![image](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/c8d5bf2c-b64e-4fa9-b910-4e02191d40c1)


Create the second bar chart with Matplotlib's pyplot methods.

![bar_chart2](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/a32eda25-c976-43f4-b989-9d5f400da595)

# Pie Charts

Generate two pie charts. Both charts should be identical and show the distribution of female versus male mice in the study.

Create the first pie chart with the Pandas DataFrame.plot() method.

![pie_chart1](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/f22dafcc-3443-427d-814b-da39b5f96071)


Create the second pie chart with Matplotlib's pyplot methods.

![pie_chart2](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/7c8c9246-5f64-488e-b8ac-c11f68d72219)

# Quartiles, Outliers, and Box Plot

Calculate the final tumor volume of each mouse across four of the most promising treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, calculate the quartiles and IQR, and determine if there are any potential outliers across all four treatment regimens. Use the following substeps:
1. Create a grouped DataFrame that shows the last (greatest) time point for each mouse. Merge this grouped DataFrame with the original cleaned DataFrame.
2. Create a list that holds the treatment names as well as a second, empty list to hold the tumor volume data.
3. Loop through each drug in the treatment list, locating the rows in the merged DataFrame that correspond to each treatment. Append the resulting final tumor volumes for each drug to the empty list.
4. Determine outliers by using the upper and lower bounds, and then print the results.

Using Matplotlib, generate a box plot of the final tumor volume for all four treatment regimens. Highlight any potential outliers in the plot by changing their color and style.

![boxplot](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/e36ee97d-c260-4543-a569-bb8ff80d7691)


# Line Plot

Select a mouse that was treated with Capomulin, and generate a line plot of tumor volume versus time point for that mouse.

![lineplot](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/a7e9f2c7-dbd9-42b5-8705-e8c8411a7108)


# Scatter Plot 

Generate a scatter plot of tumor volume versus mouse weight for the Capomulin treatment regimen.

![scatterplot](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/0f2f081e-975e-4c36-a2ef-c75d558594de)


# Correlation

Calculate the correlation coefficient and linear regression model between mouse weight and average tumor volume for the Capomulin treatment.

# Regression 

Plot the linear regression model on top of the previous scatter plot.

![linear_regression](https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/d98d614b-8c25-4dbc-94aa-ab8e21e4f383)


# Summary



