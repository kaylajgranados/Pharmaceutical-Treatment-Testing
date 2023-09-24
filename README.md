# Pharmaceutical Treatment Testing using Pandas and Matplotlib

In this project for the UCI Data Analytics Bootcamp, I used Python to analyze pharmaceutical testing treatment data. The purpose of this study was to compare the performance of an anti-cancer medication, Capomulin, against the other treatment regimens. 

# Merge data 

Merged the mouse_metadata and study_results DataFrames into a single DataFrame.

# Summary Statistics 

I created two summary statistics DataFrames. For the first DataFrame, I used the groupby method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. 

<img width="707" alt="Screen Shot 2023-09-24 at 6 09 29 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/09ad1b99-3d1d-4351-8fd3-e0d76dc61724">

For the second DataFrame, I used the agg method to produce the same summary statistics table by using a single line of code.

<img width="1139" alt="Screen Shot 2023-09-24 at 6 09 57 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/e0266c3e-36e2-4bd4-ac07-1b586999a639">


# Bar Charts 

I generated two bar charts showing the total number of time points for all mice tested for each drug regimen throughout the study. 

The first bar chart uses the Pandas built-in plotting function. 

<img width="566" alt="Screen Shot 2023-09-24 at 6 12 53 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/37976de0-b31d-46ac-bfcb-5d079f8ee394">

The second bar chart with Matplotlib methods.

<img width="615" alt="Screen Shot 2023-09-24 at 6 13 15 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/44857588-d3ac-4793-bead-e5f4bc7756cf">


# Pie Charts

I generated two pie charts showing the distribution of female versus male mice in the study.

The first pie chart uses the Pandas built-in plotting function. 

<img width="444" alt="Screen Shot 2023-09-24 at 6 13 33 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/2e2e90e1-a38b-4efe-9526-e634f9fcd0cd">

The second pie chart with Matplotlib methods.

<img width="444" alt="Screen Shot 2023-09-24 at 6 13 58 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/34285d4a-bdc2-4e12-86f9-662d044fbbe0">

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



