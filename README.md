# -5-Modeling-and-Analysis-of-Electricity-Data-Using-the-R-Programming-Language

This project deals with electricity usage data for 241 households in New Zealand collected in 2009. The data is for a single 24-hour period and has been sampled every 30 minutes. Hence there are 48 measures per household. The first entry is at 12:30am, the second at 1am, and so on.

Run the supplied R script power.R, which loads the electricity data and produces a boxplot which aggregates the 241 households over time and an example plot for one household. Note that the data is a data.frame (each row is labelled with each household identifier associated with this data), and that to plot an individual example we turned the individual 48 data points into a numeric vector (as.numeric).

Examine the boxplot and briefly discuss the aggregated pattern of electricity usage.

The electricity company is interested in understanding some general patterns of usage so that they can identify different types of users and therefore target them with specific pricing structures. One task is to identify 6 (SIX) overall patterns of usage.

This problem is basically one of clustering – but to solve the problem we will first want to construct explanatory variables that characterise the pattern of usage for each household. Note that some patterns will want to be related to how the electricity usage varies over the day, as well as summary statistics such as the mean/variance/etc. electricity usage.

Construct a table of explanatory variables, where each row is a household, and each column is an explanatory variable that I have constructed from the original usage data. Describe the functions that I have constructed to create these explanatory variables, and in particular discuss how I have described (represented) the temporal structure of usage.

Apply kmeans clustering with 6 centers to my final explanatory datatable. Produce two figures: one with boxplots showing the final clustering patterns of usage for each of the six clusters, the second as 6 line plots showing the mean usage pattern for each timestep for each cluster. 
