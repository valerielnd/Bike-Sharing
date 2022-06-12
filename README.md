# Bikesharing Analysis

## Project overview
This project aims to perform several analyses to determine if a bike-sharing business 
in Des Moines will be as successful as "Citi Bike" in NY city. So, to find how to make
this work and convince potential investors, the first step is to figure out how the bike-share 
works in NY city and, from there, create a proposal on how it might work in Des Moines.

We have performed the following analysis:

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
 
 Tableau story link:
 
 [NYC Story](https://public.tableau.com/shared/9DBT2YKND?:display_count=n&:origin=viz_share_link)


## Ressources
To perform the analysis for this project, we used the Citi Bike data released to the public.

We downloaded the CSV file that contains the data for August 2019 because there is likely more traffic during 
the summer months.

We used Tableau public to create the visualization for the business proposal, Python Panda library, 
and Jupyter notebook to transform to data before working with it.

## Results

### Gender Breakdown

One of the first pieces of information we wanted to find with a Tableau visualization is regarding the gender of the riders using 
the bike-sharing business. 
As the total number of trips for August is 2,344,224, we decided to find the number of rides by gender. 
Knowing the gender breakdown can help us learn a little more about the customers we could have in Des Moines.

![gender_breakdown_pic](https://github.com/valerielnd/Bike-Sharing/blob/main/gender_breakdown.png)

[Gender Breakdown Tableau Link](https://public.tableau.com/shared/9DBT2YKND?:display_count=n&:origin=viz_share_link)

There are 588431 female riders and 1530272 male riders. So the percentage of male riders might be more significant 
than female riders in De Moines.

### Customer Types

To continue getting information about our potential customers, we decided to find the number of short-term customers and 
annual subscribers in NY. This will help us determine the types of customers we could expect for a bike-sharing 
company in Des Moines.


![customer_proportion](https://github.com/valerielnd/Bike-Sharing/blob/main/customer_type.png)

[Customer Types Tableau Link](https://public.tableau.com/shared/K73CR6SZ7?:display_count=n&:origin=viz_share_link)

Since there are 1900359 subscribers and 443865 short-term customers, which gives a proportion of 4.28 subscribers to short-term customers,
we expect a more significant number of subscribers than short-term customers in De Moines.

### Checkout times for users

Now that we have an idea about the customers' genders and types, we decided to find the length of time that bikes are checked out 
by them. 

![checkout_times_for_users](https://github.com/valerielnd/Bike-Sharing/blob/main/checkout_time_users.png)

[Checkout times for users Tableau Link](https://public.tableau.com/shared/C2S8B58HF?:display_count=n&:origin=viz_share_link)

The highest checkout time for the users is 5 minutes, where around 146752 bikes are used for trips of that duration.
Once this peak is reached, as the checkout time continues to increase and gets over 48 minutes, the number of bikes used 
for a trip of that duration and more, decreases and stays between 0 and 5000 bikes. That means riders typically use bikes
for a trip duration between 0 to 40 minutes.

### Checkout times by gender

As we have an idea of users' typical trip duration, we decided to find out what type of users have the most extended trip duration.

![checkout_time_gender](https://github.com/valerielnd/Bike-Sharing/blob/main/checkout_time_gender.png)

[Checkout times by gender Tableau Link](https://public.tableau.com/shared/BR43F6KYB?:display_count=n&:origin=viz_share_link)

The highest checkout time for male customers is 5 mins, and for female customers, 6 mins. So, regarding the highest checkout time, 
there is not a great difference between gender while male customers tend to use more the bike-sharing business.


### Bike utilization

Now that we have an idea about who uses the ride-sharing business and typically for how long, we decided
to find information about the bikes utilization in NY to further understand the need for a bike-sharing  
company in Des Moines.

![bike_utilization](https://github.com/valerielnd/Bike-Sharing/blob/main/bike_utilization.png)

[Bike Utilization Tableau Link](https://public.tableau.com/shared/2W57SSFJQ?:display_count=n&:origin=viz_share_link)

The highest level of utilization is 3838476 seconds (around 1066 hours). The bike with the highest utilization level was used for 34 trips.
This means this bike was not used on average for short trips and might need more attention than others. So, this analysis
can help us find bikes that need more attention than others.

### Bike repairs

Since we discovered that some bikes might need more attention which means most maintenance due to their utilization, 
we decided to determine which bikes have the highest number of rides since those also might need more care. 
Getting all those information will help us get an idea of the cost of bike upkeep.

![bike_repairs](https://github.com/valerielnd/Bike-Sharing/blob/main/bike_repairs.png)

[Bike Repairs Tableau Link](https://public.tableau.com/shared/T75BWP5WW?:display_count=n&:origin=viz_share_link)

The bike with ID 38124 was used for the highest number of trips: 479. We can use this visualization and filter, for example, the ten bikes
with the highest number of trips to schedule their maintenance.

### Average Trip duration by Age

After gathering information about the customers and the bikes, we decided to focus on the trips the bikes are used for.
We started by getting the average trip duration by age.

![trip_duration_age](https://github.com/valerielnd/Bike-Sharing/blob/main/trip_duration_age.png)

[Average Trip Duration by Age Tableau Link](https://public.tableau.com/shared/SD59C9HKR?:display_count=n&:origin=viz_share_link)

In general, younger riders tend to use the bikes for longer periods of time.

### Trips by weekday for each hour

Then, we decided to get the number of bike trips for each hour of each day of the week to get an idea of the expected 
peak hours and most busy days we will have in Des Moines. This can also help estimate the number of bikes needed each 
day and also when to do maintenance on the bikes.

![trips_weekday_hours](https://github.com/valerielnd/Bike-Sharing/blob/main/trip_wkday_hour.png)

[Trips by weekday for each hour Tableau Link](https://public.tableau.com/shared/Z5JS8FR76?:display_count=n&:origin=viz_share_link)

The peak hours are 8 AM, probably when people are going to their daily activities, and 5 to 7 PM, when they 
are done and heading homes. The busiest days are Monday, Tuesday, and Thursday. So, on those days,
we might need provide the greatest number of bikes and ensure that they are all working properly. However,
we can schedule maintenance on the bikes between 2 to 5 AM each morning.

### Trips by gender (weekday per hour)

To confirm our findings regarding who uses the service the most and also to get an idea of when specifically, we 
created another visualization similar to the previous one but broke down by gender.

![trips_by_gender_hour](https://github.com/valerielnd/Bike-Sharing/blob/main/trip_gender_wkday_hour.png)

[Trips by gender \(weekday per hour\ Tableau Link)](https://public.tableau.com/shared/SYYMR6ZXN?:display_count=n&:origin=viz_share_link)

This confirms that male customers used the bike-sharing business more than female customers, and their peak hours 
of usage are 8 AM and 5 to 7 PM.

### Trips by gender by weekday

And finally, we decided to find out what type of customers, in addition to their gender, tend to have the greatest number
of trips and at what specific day in the week.

![trips_gender_type](https://github.com/valerielnd/Bike-Sharing/blob/main/trips_gender_type.png)

[Trips by gender by weekday Tableau Link](https://public.tableau.com/shared/3R2ZXQTKJ?:display_count=n&:origin=viz_share_link)

Male subscribers used the bike-sharing business more on Thursdays.

## Summary

Following the results of the analyses run on the data of the ride-sharing company Citi Bike in NY, we can expect to have
a sufficient number of trips in the summer months in Des Moine.

We will probably have more male riders than female riders and a more significant number of subscribers than short-term customers.

Riders will typically use the bikes for trip durations of 5-6 mins, and the number of bikes used for trip durations over Forty minutes 
is less than 5000.

Younger riders tend to use the bikes for more extended periods of time.

Regarding bike maintenance and cost of upkeep, we will need to pay special attention to bikes with highest utilization
levels that mean used for long trips but also bikes used for the greatest number of trips.

As for peak hours and busy days, we might need to make available the greatest number of bikes at 8 AM and between
5-7 PM on Mondays, Tuesdays, and Thursdays. So, we can schedule maintenance around 2-5 AM in the mornings.

Another two analysis that we could do is to find what Bike stations are used more to get an idea of how to distribute
our bikes among them and 



