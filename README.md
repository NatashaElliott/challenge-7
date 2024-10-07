# Project 1
Amrit, Soheil, Natasha, Iaroslav

**Datasets:**
Ambulance data - https://data.gov.au/dataset/ds-vic-05533eeb-870b-4427-afb1-a5d06faa0366/details?q=ambulance
Census data 2018 - https://www.abs.gov.au/statistics/people/population/regional-population-age-and-sex/2018
Census data 2019 - https://www.abs.gov.au/statistics/people/population/regional-population-age-and-sex/2019#data-downloads
Traffic data - https://vicdata.vicroads.vic.gov.au/metadata/Traffic_Count_Locations%20-%20Open%20Data.html

**Analysis of Ambulance Victoria response times for 2018 & 2019**
The following report is an analysis of Ambulance Victoria's performance over the years 2018 and 2019. We aimed to investigate whether Ambulance Victoria is meeting their self-stated goals and if they aren't, what factors may be contributing to this. We have identified 2 major factors which we have investigated, which are traffic density and local population. Ambulance Victoria data is divided up into both Local Government Area (LGA) and Urban Centres and Localities (UCL). We have chosen to focus on UCLs because it allowed us to line up the Ambulance data from Ambulance Victoria, census data from the Australian Bureau of Statistics, and traffic data from VicRoads. We have raised the following questions regarding these datasets:

    What is the comparison between Code 1 and Code 2 incidents in terms of average response time and number of incidents?
    Which UCLs consistently meet or fail to meet the 85% or 90% response time targets for Code 1 incidents?
    Does population density of a UCL affect Ambulance response time?
    Does traffic density affect the response time?

**What is the comparison between Code 1 and Code 2 incidents in terms of average response time and number of incidents? (Amrit)**
-Analysis goes here

**Which UCLs consistently meet or fail to meet the 85% or 90% response time targets for Code 1 incidents? (Soheil)**
-Analysis goes here

**Does population density of a UCL affect Ambulance response time? (Natasha)**
One of the factors we think could affect the response time of any given area is the population of that area. Our assumption is that with a higher population density there will be an increase in ambulance response times due to a number of reasons such as higher incident rates, higher number of calls, and ambulance staffing limitations. In order to investigate the above, data was sourced from Ambulance Victoria and merged with Census data from the Australian Bureau of Statistics. UCLs that appeared in both datasets were then matched and used for this analysis. As seen in “Total Persons vs Average Response Time (s) - 2018 & 2019”, the total population per UCL (“Total Persons”) was measured against the average response times (“AVG RT – Seconds”) for both 2018 in blue and 2019 in red as a scatter plot with added linear regression. The linear regression shows a slight negative correlation, especially for 2019. This indicates that contrary to the assumption, an increase in population does not exactly impact the response time in any particular area. The statistical analysis may in fact indicate that response times increase in areas with a lower population.
In addition to higher population in a densely populated area, we can assume that this will cause an increase in the number of calls to Ambulance Victoria services. As seen in “Total Number of Calls vs Average Response Time (s) - 2018 & 2019”, the total number of calls was measured against the average response times for again, both 2018 in blue and 2019 in red as a scatter plot with added linear regression. Additionally for the purposes of linear regression, the outlier of Melbourne for 2018 was removed as the total calls for Melbourne significantly altered the statistical analysis due to being so far out of the range of the rest of the UCLs. The linear regression still shows a slight negative correlation, however it is a stronger correlation than the previous plot. This could indicate that a greater number of calls will have a strong chance of increasing the average response time. The stronger correlation suggests that an increase in the number of calls may impact response times more significantly than a larger population does.
Based on these visualisations, population does not seem to have a significant impact on the response times of Ambulance Victoria and almost indicates that lower populated areas have higher response times. As previously mentioned, Ambulance Victoria’s staffing limitations could still be a factor causing increased response times as there may be larger staffing issues in lower populated areas. Additionally lower populated areas can often be more spread out, leading to greater travel distances. Based on this data, we can safely assume that Ambulance Victoria is still improving their response times from 2018 to 2019.

**Does traffic density affect the response time? (Iaroslav)**
-Analysis goes here

**Conclusion:**
Conclusion goes here
