# PyBer_Analysis
Visualizing ride-share data using MatPlotLib

## Resources Used
- Data Source: city_data.csv, ride_data.csv
- Software: Python 3.9, Visual Studio Code, Jupyter Notebook

## Overview of the analysis: 
My boss has given me and Omar a brand-new assignment. Using our Python skills and knowledge of Pandas, we created a summary DataFrame of the ride-sharing data by city type. Then, using Pandas and Matplotlib, we created a multiple-line graph that shows the total weekly fares for each city type.

This new assignment consists of two technical analysis deliverables and a written report to present my results. I will submit the following:

  * Deliverable 1: A ride-sharing summary DataFrame by city type
  * Deliverable 2: A multiple-line chart of total fares for each city type
  * Deliverable 3: A written report for the PyBer analysis (README.md)

## Results: Using images from the summary DataFrame and multiple-line chart, describe the differences in ride-sharing data among the different city types.
![ride_share_dataframe.png](Resources/ride_share_dataframe.png)

We initially used the data from city_data.csv and ride_data.csv to create a new DataFrame with the data we wanted to visualize. We wanted to separate data by type of location (Rural, Suburban, and Urban) and get the Total Rides, Total Drivers, Total Fares, Average Fare per Ride, and Average Fare per Driver for each location. 

Once we had this new DataFrame set up, we wanted to create a pivot table with the date as the index so we could get the total fares for each type of city by the date. Next, we created a new DataFrame so we only had the data from January 1st, 2019 through April 29th, 2019. This is the time frame we want to analyze. Lastly, we resampled this DataFrame to get the sum of the fares by week, which allowed our data to be visualized in the line graph below.

![PyBer_fare_summary.png](analysis/PyBer_fare_summary.png)

## Summary: Based on the results, provide three business recommendations to the CEO for addressing any disparities among the city types.
Based on the results of our DataFrame and line graph, we can see the following trends:
 1. Total fares were by far the highest in Urban areas ($39,854.38) compared to Suburban ($19,356.33) and Rural ($4327.93) areas.
 2. While total fares were much higher in Urban areas, Average Fare per Driver was much lower. Urban drivers made $16.57 on average for every ride       they gave, while in Rural     areas, drivers made more than 3x as much ($55.49/ride). 
 3. As well as lower fares per driver, fares per ride are much different depending on the location of the trip. Rural rides are the most expensive, as they average $34.62/ride.       While Surburban ($30.97/ride) and Urban ($24.53/ride) areas were much cheaper. 
 
 If I were to make a recommendation to the CEO, I would recommend raising prices in Urban areas, as there are 15x as many rides taken compared to Rural areas and there is greater demand in those areas for quick and accessible transportation.
  
