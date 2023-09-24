# Pharmaceutical Treatment Testing using Pandas and Matplotlib

In this project for the UCI Data Analytics Bootcamp, I used Python to analyze pharmaceutical testing treatment data. The purpose of this study was to compare the performance of an anti-cancer medication, Capomulin, against the other treatment regimens. 

# Prepare Data

To prepare the data, I merged the mouse_metadata and study_results DataFrames into a single DataFrame.

# Summary Statistics 

To begin the analysis, I created two identical summary statistics DataFrames. For the first DataFrame, I used the groupby method to generate the mean, median, variance, standard deviation, and SEM of the tumor volume for each drug regimen. For the second DataFrame, I used the aggregate method to produce the same summary statistics table. 

<img width="477" alt="Screen Shot 2023-09-24 at 6 27 52 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/6bda4cf5-489c-4a8c-b0ea-6bb15e238bc9">

# Bar Charts 

I generated two bar charts showing the total number of time points for all mice tested for each drug regimen throughout the study. 

The first bar chart uses the Pandas built-in plotting function. 

<img width="566" alt="Screen Shot 2023-09-24 at 6 12 53 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/37976de0-b31d-46ac-bfcb-5d079f8ee394">

The second bar chart uses Matplotlib methods.

<img width="615" alt="Screen Shot 2023-09-24 at 6 13 15 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/44857588-d3ac-4793-bead-e5f4bc7756cf">

# Pie Charts

I generated two pie charts showing the distribution of female versus male mice in the study.

The first pie chart uses the Pandas built-in plotting function. 

<img width="444" alt="Screen Shot 2023-09-24 at 6 13 33 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/2e2e90e1-a38b-4efe-9526-e634f9fcd0cd">

The second pie chart uses Matplotlib methods.

<img width="444" alt="Screen Shot 2023-09-24 at 6 13 58 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/34285d4a-bdc2-4e12-86f9-662d044fbbe0">

# Quartiles, Outliers, and Box Plot

I calculated the final tumor volume of each mouse across four of the treatment regimens: Capomulin, Ramicane, Infubinol, and Ceftamin. Then, I calculated the quartiles and IQR, and I determined if there were any potential outliers.

To do so, I created a grouped DataFrame that shows the last (greatest) time point for each mouse and merged this grouped DataFrame with the original cleaned DataFrame. Then, I created a list that holds the treatment names as well as a second, empty list to hold the tumor volume data. I used a for loop to iterate through each drug in the treatment list, locate the rows in the merged DataFrame that correspond to each treatment, and extract the tumor volume data for each of the treatments. I also determine outliers by using the upper and lower bounds. 

Here is the code used for the for loop: 

<img width="821" alt="Screen Shot 2023-09-24 at 6 19 09 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/df131a73-b605-4a42-8782-b6fcc31d550f">


To visualize the quartiles, I generate a box plot of the final tumor volume for all four treatment regimens. 

<img width="603" alt="Screen Shot 2023-09-24 at 6 19 49 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/5444d19b-b466-4262-bff5-39779072c66f">


# Line Plot

I selected a mouse that was treated with Capomulin and I generated a line plot of 'Tumor volume' versus 'Time point' for that mouse.

<img width="613" alt="Screen Shot 2023-09-24 at 6 20 34 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/b74c10d8-162c-4b54-8ed9-1fd0eee4c130">


# Scatter Plot 

I generated a scatter plot of 'Tumor Volume' versus 'Weight' for the Capomulin treatment regimen.

<img width="605" alt="Screen Shot 2023-09-24 at 6 20 54 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/e2dd1266-5fa5-4ecb-9425-f49cdbb469dc">

# Correlation

The correlation coefficient between 'Weight' and 'Tumor Volume' is 0.82. This indicates a strong positive relationship between the two factors. 

<img width="845" alt="Screen Shot 2023-09-24 at 6 22 11 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/f9efc988-fd86-44ff-be5b-b89c29887984">


# Regression 

I calculated linear regression and plotted the linear regression model on top of the previous scatter plot.

The linear regression equation is y = 0.95x + 21.55. This means there is a strong positive relationship between 'Weight' and 'Tumor Volume', with 'Weight' as the independent variable and 'Tumor Volume' as the dependent variable. 

<img width="604" alt="Screen Shot 2023-09-24 at 6 23 57 PM" src="https://github.com/kaylajgranados/Pharmaceutical-Treatment-Testing/assets/83734241/60517eb4-df61-4a35-846f-30786bc6e864">


# Conclusions 

1. From the bar charts, I can conclude that Capomulin and Ramicane are the most promising drug regimens.
2. From the pie charts, I can note that there are slightly more males than females in this study.
3. From the box plots, I can see that Capomulin and Ramicane have lower median tumor volumes, lower IQRs, and potential outliers with lower values than Infubinol and Ceftamin. Capomulin and Ramicane have lower tumor volumes and less variability.
4. From the positive correlation coefficient between 'Weight' and 'Tumor Volume', I can conclude that when the value of one variable increases in a mouse treated with the Capomulin drug regimen, we'd expect the other variable to increase. This is visualized in the linear regression model.



