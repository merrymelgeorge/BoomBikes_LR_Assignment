# BoomBikes_LR_Assignment

## Problem Statement
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled wherein the user enters the payment information, and the system unlocks it. This bike can then be returned to another dock belonging to the same system.

A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state.

In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.

They have contracted a consulting company to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market. The company wants to know:

Which variables are significant in predicting the demand for shared bikes.
How well those variables describe the bike demands
Based on various meteorological surveys and people's styles, the service provider firm has gathered a large dataset on daily bike demands across the American market based on some factors.

## Business Goal
You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.

## Data Dictionary
The data, day.csv, has the following attributes :

instant: record index
dteday : date
season : season (1:spring, 2:summer, 3:fall, 4:winter)
yr : year (0: 2018, 1:2019)
mnth : month ( 1 to 12)
holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
weekday : day of the week
workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
weathersit :
1: Clear, Few clouds, Partly cloudy, Partly cloudy
2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
temp : temperature in Celsius
atemp: feeling temperature in Celsius
hum: humidity
windspeed: wind speed
casual: count of casual users
registered: count of registered users
cnt: count of total rental bikes including both casual and registered


### Technologies Used
* IPython - Version 7.29.0
* Pandas - Version 1.3.4
* NumPy - Version 1.20.3
* Jupyter Notebooks - Version 6.4.5
* Seaborn - Version 0.11.2
* Matplotlib - Version 3.4.3
* Scikit - Version 0.24.2
* StatsModel Api - Version 0.12.2


## Observations and Conclusions

* Temperature is the most positively contributing feature to the target variable. Summer season also has a positive relation. Hence, the company should make sure of the availability of bikes during these periods due to high demands
* Saturdays and Working days have a positive influence on the number of bookings. Also, holidays have a negative impact. Hence, the company should come up with some strategy to attract the users on Working weekdays as well as holidays.
* Weather conditions like Mist, clouds, Light Snow, Light rain etc have a negative contribution. The spring season and windy condition also can be considered as an extension to this. As such, company should come up with better or complmentary strategies to tackle this issue.
* Though the entire winter is a good contributing factor, the September month alone stands out as more contributing factor.
* There is an increase in bookings from 2018 to 2019, with an organic growth of 23%.
* Temperature with the highest positive coefficient
* Weather Situation = 3 (Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds) has the next highest coefficient in magnitude. But the sign is negative
* Year has the third-highest effect, and it is positive
