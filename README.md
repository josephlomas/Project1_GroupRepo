# Project1_GroupRepo

This analysis pulls in Zillow datasets that give insight on the US residential housing market. At the beginning of the code, we bring in dependencies and we import six csv files that come directly from Zillow. Most of the code is cleaning the datasets by taking out rows that have N/As and organizing the data into usable DataFrames. For some graphs and calculations, we only wanted to look at the last five years of data so we filtered the datasets to start the data at January 2018. Also, the data is organized by regions within a state. For many of the graphs, we aggregated up to the state level by taking the average. 

The basic questions that we are interested in are where are the most and least expensive housing markets at the state level. To answer this questions we created a heatmap that looks at the average median sale price and the average rental prices across the US. This gave us an idea of where home sales and rents were highest and lowest. Also, we created bar graphs that show the top and bottom 25 regions and 10 states in the US. We used these graphics to quickly summarize the data and understand the headline of what is the most and least expensive market.

Hawaii, Coloarado, and California are ranked in the top 5 for both home sales and rent. While the West Cost dominates in home sales, the rental market is somewhat split between the both coasts. Also, the average rental rate in the US falls in the top 10 when compared to all the states individually. This indicates that the rent prices from the top states are pulling the average higher than rents from bottom states. The top 5 states consisting on Hawaii, Colorado, Vermont, California, and Massachussets are driving the higher national rent price.

The second part of our analysis looks to answer more complicated questions related to the state of the housing market. The two main questions are:
1) Is it better to be a renter vs a owner?
2) Is it better to be a buyer vs a seller?

To answer our first question, we looked at the relationship between median home sales and monthly rent. We plotted these two datasets as a scatter plot and found that as median sale prices rise so does monthly rent. The correltion between the two variables is 87%. On the scatter plot, the closer you get to red trend line the more closely this relationship holds. If a region falls above the trend line the advantage goes to the renter. If the region falls below the trend line the advantage goes to the buyer. We determined because the relationship between the two variables are so close, it is hard to say for the entire US housing market whether it is better to be a renter or a buyer.

To answer the second question, we leveraged datasets that forecast home value and analyzed the relationship between average days to close a home sale and percent of homes sold above listing price. When highlighting specific states, we also included statistics on median sale price and rental price to support the argument.

We graphed the Forecasted Change in Home Value by percent and numerical growth. To calculate the numerical growth, we did the following calculation:
Change in Value = Average Home Value * (1 + Percent Value Change)

This calculation was important because numerical growth in home value by state varies differently than percentage growth. A state that is starting at a low base might have the same percent increase as a another state but a greater numerical increase. This is reflected in differing top and bottom 5 for forecasted home value. 

Then, we graphed as a scatter plot Average Days to Close vs. Percent Home Sold Above List at the state level. The scatter plot was split into four quandrents that shows how the relationship between the two variables impact whether it is better to be a buyer or a seller. We determined the cutoff for each quadrent by calculating the median of each variable.

Finally, we selected New Jersey, Flordia, and Arizona as states you want to be a buyer and Wisconsin, Florida, and Kansas as states you want to be a seller. Also, we saw New Hampshire as market that is friendly to both buyers and sellers. We back up these recommendations using summary statisitcs from the median sale price, rental price, home value forecast, and its quadrent position in the relationship between homes sold above list and average days to close. We also include desk research that highlights market conditions in each state.