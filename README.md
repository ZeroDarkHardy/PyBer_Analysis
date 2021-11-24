# PyBer (Ride-Sharing Data Analysis)

## Project Overview
Given a wealth of data regarding the ride-sharing company PyBer's customer and driver data, our goal is to analyze and explore potential correlation between market factors in specific types of cities and the total fare revenue generated in those areas.  Visualizations were created to help illustrate the disparities between types of cities, be they Rural, Suburban, or Urban.

---
## Resources
**Source Files:** [city_data.csv](https://github.com/ZeroDarkHardy/PyBer_Analysis/blob/main/Resources/city_data.csv), [ride_data.csv](https://github.com/ZeroDarkHardy/PyBer_Analysis/blob/main/Resources/ride_data.csv)

**Python Code (via Jupyter Notebook):** [PyBer_Challenge.ipynb](https://github.com/ZeroDarkHardy/PyBer_Analysis/blob/main/PyBer_Challenge.ipynb)

**Software:** Python 3.7.10, Anaconda, Pandas, Matplotlib.pyplot, Jupyter Notebook, Visual Studio Code 1.62.1

---
## Results
### Summary of rides, drivers and fares by city type:
![PyBer_Summary_DF](https://github.com/ZeroDarkHardy/PyBer_Analysis/blob/main/analysis/pyber_summary_df.png)
- The data, once aggregated, shows an inverse relationship between the average fare (both per ride and per driver) and the total number of rides, when you compare the various city types.  In rural areas, where we see only 125 total rides, we see an average fare per driver of $55.49, as opposed to urban areas where the average fare per driver was only $16.57 (and there were 1,625 total rides).
- A direct correlation is observed between the number of drivers and the total rides/fares.
- It's worth noting that, in urban areas, there are far more drivers than there were total rides.  This suggests that almost 800 drivers never had a single fare, during the data sample time period.  This also suggests that the average fare per driver in those areas may be a bit skewed, since many drivers would never have made anything from fares and thusly present null values, weighing our averages.  In the other two areas, rural and suburban, there are fewer drivers than there are total rides, and we can see that the average fare per driver (rural: $55.49, suburban: $39.50) are higher than the average fare per ride (rural: $34.62, suburban: $30.97), yet in urban areas the average fare per ride is $24.53 while the average fare per urban driver is only $16.57.
---
### Total fares by city type, from 1-1-2019 through 4-28-2019
![total_fares_by_city_type_linechart](https://github.com/ZeroDarkHardy/PyBer_Analysis/blob/main/analysis/total_fares_by_city_type_linechart.png)
- Visualizing the longitudinal data for total fares by city type tells us only a few things:
    - The disparities in fare revenues between city types remain pretty constant throughout our sample period.
    - There seemed to be a mutual spike in fares in all city types during the 3rd and 4th week of February.  More research into the cause of this spike is recommended.
    - Since there are currently more drivers than there are customers in urban areas, we're likely seeing the maximum amount of total fares for those areas.  Marketing and discount promotions, however, may produce changes in rural and suburban areas.
---
## Summary
Even though there seems to be a directly inverse relationship between the average fare per rides and the total rides that took place, it's unclear how much the price of the fare actually incentivizes or dissuades the customers from utilizing the service.  My business recommendations to PyBer are as follows:
- Temporarily reduce the costs to consumers in rural areas, to see whether this incentivizes more people to use the ride-sharing service.  Immediate risks include a fall in revenue (though the risk is mitigated by the much smaller customer base in rural areas), and a potential impact to the number of participating drivers.  If this theory proves successful, it should resolve the other risks as well.
- Reduce workforce in urban areas.  This is an obvious move, since there are clearly more drivers than there are customers.  Performing additional analysis after a period with reduced workforce should provide more accurate revenue information.
- Investigate market forces driving the spike in fares seen in all areas in late February of 2019.  Perhaps there are factors that can be replicated, to the benefit of PyBer and all drivers.
