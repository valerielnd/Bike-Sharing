# Bikesharing Analysis

## Project Overview
This project aims to see if a bike-sharing business in Des Moines can be as successful as "Citi Bike" in New York City. 
To do this, we'll first study how bike-sharing works in NYC and then propose how it could work in Des Moines to attract investors.

We have performed the following analysis using Tableau:

* Gender Breakdown
* Customer Type
* Checkout times for users
* Checkout times by gender
* Bike utilization
* Bike repairs
* Average Trip duration by Age
* Trips by weekday for each hour
* Trips by gender (weekday per hour)
* Trips by gender by weekday
 
All of these visualizations have been integrated into a Tableau story, accessible via the following link:
 
 [NYC Story](https://public.tableau.com/views/NYC_Story_16550826332950/NYCCitibikeanalysis?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)


## Ressources
We used the Citi Bike data released to the public to perform the analysis for this project.

We downloaded the CSV file that contains the data for August 2019 because there is likely more traffic during 
the summer months.

We used Tableau Public to create the visualizations for the business proposal, Python Panda library, 
and Jupyter Notebook to transform to data before working with it.

## Results

### Gender Breakdown

We initially sought to explore the gender distribution among users of the bike-sharing service using a Tableau visualization. 
With 2,344,224 trips recorded for August, we analyzed the number of rides by gender. Understanding this breakdown can provide insights into the potential customer demographics in Des Moines.

![gender_breakdown_pic](https://github.com/valerielnd/Bike-Sharing/blob/main/gender_breakdown.png)

[Gender Breakdown Tableau Link](https://public.tableau.com/views/NYC_Story_16550826332950/NYCCitibikeanalysis?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

There are 588431 female riders and 1530272 male riders. So the percentage of male riders might be more significant 
than female riders in De Moines.

### Customer Types

To further understand our potential customers, we decided to identify the count of short-term and annual subscribers in New York. 
This analysis will assist us in anticipating the customer types for a bike-sharing service in Des Moines.


![customer_proportion](https://github.com/valerielnd/Bike-Sharing/blob/main/customer_type.png)

[Customer Types Tableau Link](https://public.tableau.com/shared/ND59Z5376?:display_count=n&:origin=viz_share_link)

With 1,900,359 subscribers and 443,865 short-term customers, the ratio of subscribers to short-term customers is 4.28. 
Consequently, we anticipate more subscribers than short-term customers in Des Moines.

### Checkout times for users

Having gained insights into the genders and types of customers, we determined the duration they check out bikes.

![checkout_times_for_users](https://github.com/valerielnd/Bike-Sharing/blob/main/checkout_time_users.png)

[Checkout times for users Tableau Link](https://public.tableau.com/shared/48GPWJKMR?:display_count=n&:origin=viz_share_link)

The peak checkout time for users is 5 minutes, with approximately 146,752 bikes utilized for trips that duration. 
Beyond this peak, as the checkout time surpasses 48 minutes, the number of bikes used for trips of that length or longer diminishes, 
stabilizing between 0 and 5,000 bikes. This suggests that riders generally utilize bikes for trips lasting between 0 and 40 minutes.

### Checkout times by gender

As we have an idea of users' typical trip duration, we decided to find out what type of users have the most extended trip durations.

![checkout_time_gender](https://github.com/valerielnd/Bike-Sharing/blob/main/checkout_time_gender.png)

[Checkout times by gender Tableau Link](https://public.tableau.com/shared/JKQMP9MP7?:display_count=n&:origin=viz_share_link)

Male customers have a peak checkout time of 5 minutes, while female customers have a peak checkout time of 6 minutes. 
Therefore, although male customers are more inclined to use the bike-sharing service, there isn't a significant difference between genders regarding their highest checkout time.

### Bike utilization


Now that we understand the demographics of ride-sharing users and their typical trip durations, 
we explored bike utilization data in New York. This will provide additional insights into the demand for a bike-sharing service in Des Moines.

![bike_utilization](https://github.com/valerielnd/Bike-Sharing/blob/main/bike_utilization.png)

[Bike Utilization Tableau Link](https://public.tableau.com/shared/Y3MTSHYPX?:display_count=n&:origin=viz_share_link)

The highest level of utilization is 3838476 seconds (around 1066 hours). The bike with the highest utilization level was used for 34 trips.
This means this bike was not used on average for short trips and might need more attention than others. So, this analysis
can help us find bikes that need more attention than others.

### Bike repairs

The bike with the highest utilization level was used for 3,838,476 seconds, equivalent to approximately 1,066 hours. 
This bike was utilized for 34 trips, indicating that it was not typically used for short trips. As a result, 
it may require more maintenance and attention compared to other bikes. Analyzing this data helps identify bikes that may need additional maintenance.

![bike_repairs](https://github.com/valerielnd/Bike-Sharing/blob/main/bike_repairs.png)

[Bike Repairs Tableau Link](https://public.tableau.com/shared/3FHJY6D6T?:display_count=n&:origin=viz_share_link)

The bike with ID 38124 was used for the highest number of trips: 479. We can use this visualization and filter, for example, the ten bikes
with the highest number of trips to schedule their maintenance.

### Average Trip Duration by Age

Having collected data about both customers and bikes, we shifted our focus to analyzing the trips taken with the bikes. 
Our initial step was calculating the average trip duration based on age groups.

![trip_duration_age](https://github.com/valerielnd/Bike-Sharing/blob/main/trip_duration_age.png)

[Average Trip Duration by Age Tableau Link](https://public.tableau.com/shared/24N42NG7M?:display_count=n&:origin=viz_share_link)

In general, younger riders tend to use the bikes for longer periods.

### Trips by weekday for each hour

Subsequently, we opted to tally the bike trips per hour for each day of the week to discern the anticipated peak hours and busiest days in Des Moines. 
This analysis aids in estimating the daily bike requirements and determining optimal maintenance schedules.

![trips_weekday_hours](https://github.com/valerielnd/Bike-Sharing/blob/main/trip_wkday_hour.png)

[Trips by weekday for each hour Tableau Link](https://public.tableau.com/shared/W2NB9XZZC?:display_count=n&:origin=viz_share_link)

The peak hours are 8 AM, probably when people go to their daily activities, and 5 to 7 PM, when they 
head home. The busiest days are Monday, Tuesday, and Thursday. So, on those days,
we need to provide the greatest number of bikes and ensure they all work properly. However,
we can schedule maintenance on the bikes between 2 to 5 AM each morning.

### Trips by gender (weekday per hour)

To confirm our findings regarding who uses the service the most and also to get an idea of when specifically, we 
created another visualization similar to the previous one but broken down by gender.

![trips_by_gender_hour](https://github.com/valerielnd/Bike-Sharing/blob/main/trip_gender_wkday_hour.png)

[Trips by gender \(weekday per hour\) Tableau Link](https://public.tableau.com/shared/5QZR29RCJ?:display_count=n&:origin=viz_share_link)

This confirms that male customers used the bike-sharing business more than female customers, and their peak hours 
of usage are 8 AM and 5 to 7 PM.

### Trips by gender by weekday

And finally, we decided to find out what type of customers, in addition to their gender, tend to have the greatest number
of trips and on what specific day of the week.

![trips_gender_type](https://github.com/valerielnd/Bike-Sharing/blob/main/trips_gender_type.png)

[Trips by gender by weekday Tableau Link](https://public.tableau.com/shared/YN87TTDQN?:display_count=n&:origin=viz_share_link)

Male subscribers tend to use the bike-sharing business more, especially on Thursdays.

## Summary

Following the results of the analyses run on the data of the ride-sharing company Citi Bike in NY, we can expect to have
a sufficient number of trips to Des Moines in the summer months.

We will probably have more male riders than female riders and a more significant number of subscribers than short-term customers.

Riders will typically use the bikes for trip durations of 5-6 minutes, and the number of bikes used for trip durations over Forty minutes 
is less than 5000.

Younger riders tend to use the bikes for more extended periods.

Regarding bike maintenance and cost of upkeep, we will need to pay special attention to bikes with the highest utilization
levels that mean used for long trips and bikes used for the greatest number of trips.

As for peak hours and busy days, we might need to make available the greatest number of bikes at 8 AM and between
5-7 PM on Mondays, Tuesdays, and Thursdays. So, we can schedule maintenance around 2-5 AM.

Two other analyses we could do is to find the top starting trip stations and top ending trip stations to get an idea of how to distribute
our bikes among the different stations.



