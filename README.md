**Lighthouse Labs Data Science - Midterm Project**

**Task 4**:  How taxi times changing during the day? Does higher traffic lead to bigger taxi times?

After first plotting the number of departures during the day to get an idea of the peak hours, I plotted the taxi-out and taxi-in times to find outliers. Right off the bat, there are a few obvious ones that I removed. However, upon plotting the average taxi-out/taxi-in times against the hour of the day, there is not an obvious trend.
***
**Task 5**: What is the average percentage of delays that is already created before departure? (aka are arrival delays caused by departure delays?) Are airlines able to lower the delay during the flights?

This was a bit confusing for me, but essentially, I counted the number of flights that had both a departure delay and arrival delay, then calculated the percentage of those situations from the total number of flights. For the second part of the question, I calculated the average difference between the delay times (arrival_delay - departure_delay) which would tell me if the delay was reduced during flight.
***
**Task 6**: How many states cover 50% of US air traffic?

Pretty straight-forward.
***
**Task 7**: Test the hypothesis whether planes fly faster when there is the departure delay? 

After cleaning up the data, I wondered if the distance would have a more significant effect on plane speed. So, first of all, I calculated the plane's speed by dividing the distance by the elapsed time (in hours) to get a miles-per-hour value. After normalizing the data by converting time into hours, I first plotted the distance by the speed. Per the figure, we can see that with a farther destination, the plane will travel faster...makes sense.
The second figure is the effect of delay times on plane speed, which does not give a very clear interpretation since it fluctuates so much. So, I kind of made a hybrid of the two figures. For the third figure, I split the flights into long, medium, and short hauls (based on task 8), then compared the delay times to average plane speeds. So from this, we still don't really see a trend.
***
**Task 8:** When (which hour) do most 'LONG', 'SHORT', 'MEDIUM' haul flights take off?

First, clean up data (missing values) then standardizing the time to hours, then binning them. I read that short haul flights are less than 3 hours long, medium hauls are between 3 and 6 hours, and long haul flights are over 6 hours. So after splitting them up, I plotted them. We can see that short and medium haults are most popular throughout the day, with a break for medium hauls around lunch time, but long haul flights are very specific to mornings.
