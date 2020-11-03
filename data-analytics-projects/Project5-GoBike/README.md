# Exploration on Ford  GoBike System Data
## by Junghoon Suk


## Dataset

> Ford GoBike System Data discovers individual trip information of a bike-sharing system 
in the Greater Sanfrancisco Bay Area, that is publicly available on https://www.lyft.com/bikes/bay-wheels/system-data. 

> The dataset chosen for this exploration covers the period of June 2020 only. 

> The dataset was cleaned to include features of interest, and saved as 'bike_cleaned' dataframe. 
The process covered the following:   

- all geographcial data were deleted 
- datetime features were added
- the key variable of interest is created and named as 'duration_min.' 
It numerically represents duration of bike rental measured by minute.

> Some outliers were investigated in the key variable 'duration_min' and data with the following conditions are excluded.

- Trip duration less than 1 minute
- Trip duration more than 1 day (1440 minutes)


## Summary of Findings

> After exploring the data, key findings are summarized as following:

1. The median trip duration is around 14 minutes, with over 75% of the rentals last 24 minutes.

2. The ridership shows a constant increase from 6am till it peaks at around 17-18 pm. 
A fair level of demand last until 21pm, and usage becomes down to the lowest level through the night time.

3. There is no noticeable difference in trip duration between casual users and members (customer type). 
It is rather casual users more likely to ride longer than members although difference is trivial. 

4. Trip durations is slightly higher on weekends than weekdays.

4. Of the two available bike types, electric bikes were rented more than docked bikes. 

5. However, it looks that trip duration of electric bikes are shorter than docked bikes. 
All users didn't rent elctric bikes more than 500 minutes level (approximately 8 hours).


## Key Insights for Presentation

> Note that no changes in design is made from your exploration step.

> The recent pricing policy says "single rides start at $2 for the first 30 minutes, then $2 per additional 15 minutes." 
(source from: https://www.lyft.com/bikes/bay-wheels/pricing).

Trip duration in general is mostly below the first quota level (30 minutes), not producing additional charges per every 15 minutes. 
It suggests that users prefer renting bikes from Ford Gobike (now as Bay Wheels) for a quick ride only.

On the other hand, electric bikes are more demanded, assuming the similiar level of availability. 
However, trip duration is not as high as docked bikes, which suggests further investigation to improve the operation of electric bikes.









