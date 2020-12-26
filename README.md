# NYC Citibike Analysis

##Analyze NYC Citi Bike data during the month of August that has been released to the public and identify if the relevant data will be able to apply to bike-sharing company in Des Moines.  

- Deliverable 1: Change Trip Duration to a Datetime Format:
	- Using Python and Pandas to convert the "tripduration" column from an interger to a datetime datatype to get the time in hours, minutes, and seconds.Then, export the DataFrame as a csv file to use for Deliverable 2. 
	- use ```pandas pd.to_datetime() function``` 

- Deliverable 2: Create Visualizations for the Trip Analysis 
	- How long bikes are checked out for all riders and genders.
	- How many trips are taken by the hour for each day of the week, for all riders and genders.
	- A breakdown of what days of the week a user might be more likely to check out a bike, by type of user and gender.

###Resources

- Data Source: 
	- 201908-citibike-tripdata.csv

- Software: 
	- Jupyter Notebook 6.1.4
	- Tableau Public 2020.4.0

##Results:

- Dashboard: 
![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/dash.PNG "Dashboard")
It shows the total number of bike rides/trips in the month of August (2,344,224), gender breakdown (male: 1,530,272 / female: 588,431 / unknown: 225,521), as well as average trip duration by age (birth year).

- Checkout Times for Users:
![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/checkout_times_for_users.PNG "Checkout Times for Users")
It shows the number of bikes (y axis) being used per tripduration (x axis). The bikes are commonly used for 4-6th hours with the peak at 5 hours and 15 minutes.

- Checkout Times by Gender:
![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/checkout_times_for_gender.PNG "Checkout Times by Gender")
It is the same graph as "Checkout Times for Users" but the number of bikes are based on gender (male/female/unknown).

- August Peak Hours:
![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/august_peak_hour.PNG "August Peak Hours")
It shows the peak usage hours for the month August (y axis shows the hours and x ticks shows the number of bikes used). There are two prime times throughout a day, 8-9am in the morning and 5-7pm in the afternoon. 

- Trips by Weekday for Each Hour:

![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/trips_by_weekday_each_hour.PNG "Trips by Weekday for Each Hour")

This is breakdown of "August Peak Hours" by day of week. y axis shows the hours and x axis shows the day of week. The heatmap indicates the number of bikes. The darker the color, more bikes being used. The large number of bikes are used during peak hours (8-9 am and 5-7pm) from "August Peak Hours" on weekday (Mon - Fri). However, more bikes are used b/w 9am - 9pm inversely on weekend (Sat/Sun).

- Trips by Gender Weekday per Hour:
![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/trips_by_gender_weekday_per_hour.PNG "Trips by Gender Weekday per Hour")
This is the same graph but split into three parts based on gender (female/male/unknown). Although the bike counts is higher with male users, the trip patterns (hours/weekday) are identical. 

- Trips by Gender by Weekday:

![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/trips_by_gender_weekday.PNG "Trips by Gender by Weekday")

This heatmap shows the count of bikes used by weekday and gender. The darker the blue, the higher the count.

- Top Starting/Ending Locations:
![alt text](https://github.com/Yunaka1269/bikesharing/blob/main/pic/top_starting_ending_locations.PNG "Top Starting/Ending Locations")
The size and the color of circle indicate the bike counts (bigger/darker the circle, the higher in bike counts). Two maps show the top starting locations and endfing locations. Noticebly, these top locations are almost the same. They may be popular tourist sites/landmarks and or near business/financial district.  


##Summary:

Even though our bike-sharing company is in Des Moines, we can expect the same weekday/hours bike ride pattern and gender ratio from NYC result. It is crucial to determine the station locations that are close to major tourist sites/landmarks and also close to business district to attact both the leisure travelers and the local commuters. Bikes need to be maintained between 9pm and 6am next day and are to be allocated aproppriately depending on demands. Upon launching the bike sharing srevice, we may want to offer a promotion that's targeting on riders who were born 1990 and after since tripduration increases in NYC.  
