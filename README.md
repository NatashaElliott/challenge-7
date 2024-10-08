# Project 1: Amrit, Soheil, Natasha, Iaroslav

**Datasets:**

Ambulance data - https://data.gov.au/dataset/ds-vic-05533eeb-870b-4427-afb1-a5d06faa0366/details?q=ambulance

Census data 2018 - https://www.abs.gov.au/statistics/people/population/regional-population-age-and-sex/2018

Census data 2019 - https://www.abs.gov.au/statistics/people/population/regional-population-age-and-sex/2019#data-downloads

Traffic data - https://vicdata.vicroads.vic.gov.au/metadata/Traffic_Count_Locations%20-%20Open%20Data.html

**Analysis of Ambulance Victoria response times for 2018 & 2019**

The following report is an analysis of Ambulance Victoria's performance over the years 2018 and 2019. We aimed to investigate whether Ambulance Victoria is meeting their self-stated goals and if they aren't, what factors may be contributing to this. We have identified 2 major factors which we have investigated, which are traffic density and local population. The data from Ambulance Victoria includes both Code 1 incidents, which are defined as “urgent, requiring a lights and sirens response” and Code 2 incidents, which are “not time critical and do not require a lights and sirens response”. The data is divided up into both Local Government Area (LGA) and Urban Centres and Localities (UCL). We have chosen to focus on UCLs because it allowed us to line up the Ambulance data from Ambulance Victoria, census data from the Australian Bureau of Statistics, and traffic data from VicRoads. 

We have raised the following questions regarding these datasets:

What is the comparison between Code 1 and Code 2 incidents in terms of average response time and number of incidents?

Which UCLs consistently meet or fail to meet the 85% or 90% response time targets for Code 1 incidents?

Does population density of a UCL affect Ambulance response time?

Does traffic density affect the response time?


**What is the comparison between Code 1 and Code 2 incidents in terms of average response time and number of incidents? (Amrit)**

For Code 1 

![image](https://github.com/user-attachments/assets/4f180bed-5bc8-48f7-aa49-803d9e96b678)

R-squared value 0.0015 indicates that only 0.15% of the variability in average response time can be explained by the total number of calls. This suggests a very weak linear relationship, meaning that the number of calls does not significantly contribute to understanding the changes in response times.The extremely low R-squared value implies that there are likely other factors influencing response times that are not captured by this model. It indicates that the model is not very useful for predicting response times based on call volume.

Whereas, For Code 2

![image](https://github.com/user-attachments/assets/707441dd-65e6-429c-a65a-e8bb69268620)

R-squared value 0.0213 suggests that 2.13% of the variability in average response time can be explained by the total number of calls. Although this is slightly better than the R-squared for Code 1, it still reflects a weak relationship.While there is a marginally better fit compared to Code 1, it still indicates that the total number of calls has limited explanatory power regarding average response times. Other factors are likely more significant contributors to the variability in response times.

When compared side by side,

![image](https://github.com/user-attachments/assets/e9113535-7093-4b13-a83f-dc3369e8fd18)

Code 1 incidents, likely representing more critical and life threatening emergencies, receive faster response times (9 to 15 minutes), reflecting the system's focus on high-priority cases. In contrast, Code 2 incidents, possibly less urgent, experience significantly longer response times (19 to 32 minutes). This suggests that while resources are effectively directed towards urgent cases, there could be potential service capacity issues impacting the speed of lower-priority responses.<br><br/>

In summary, both models indicate that while there is some correlation between the total number of calls and the average response time, this correlation is weak. The low R-squared values suggest that other factors—such as operational efficiency, geographical location, or service quality—might have a more significant impact on response times. Therefore, further analysis considering additional variables would likely provide a more comprehensive understanding of the factors affecting average response times in ambulance services.

Considering the overall trend, 

![image](https://github.com/user-attachments/assets/6ec5cee2-8537-4616-a8fe-a587600df02c)

The bar graphs suggest

- Increase in Unique Areas: The growth in the number of unique areas served signifies an expansion of service coverage. This could be attributed to factors such as population growth or deliberate efforts to enhance accessibility for underserved regions. By reaching more areas, the service demonstrates a commitment to meeting community needs.

- Decrease in Average Number of Calls: The notable reduction in the average number of calls per area suggests positive developments in public health. This could indicate that improvements in lifestyle, health awareness, and preventive healthcare measures are contributing to fewer emergency situations. Additionally, it may reflect effective management strategies that successfully reduce the demand for emergency services, allowing resources to be better allocated.

- Increase in Code Types: The rise in the number of codes indicates a diversification of services offered, facilitating more specialized responses to different situations. This development can enhance the efficiency of call management, as dispatchers can allocate resources more effectively based on the specific nature of each call. It reflects an adaptive approach to emergency response that caters to varying community needs.

- Consistency in Average Response Time: The stability in average response times across both years demonstrates that, despite fluctuations in demand and service coverage, the quality of emergency service remains high. This consistency can be attributed to improved operational practices and resource management, ensuring that response times are effective even amid increased complexity in service delivery.

Overall, these trends suggest that emergency services are adapting well to changing community needs, with a focus on improving accessibility, efficiency, and quality of service. Continued monitoring and evaluation will be essential to sustain these positive developments and ensure that the system remains responsive to the demands of the population.


**Which UCLs consistently meet or fail to meet the 85% or 90% response time targets for Code 1 incidents? (Soheil)**

Based on the analysis of ambulance response times across different UCLs (Urban Centres and Localities), we identified key trends in meeting the 85% and 90% response time targets for Code 1 incidents. A significant number of UCLs fall into the "Between 85%-90%" category, indicating that while they are relatively close to meeting the 90% target, there is still room for improvement. UCLs that meet the 90% target show strong performance, with efficient emergency response systems likely due to better infrastructure or resource allocation. Conversely, UCLs that consistently fail to meet the 85% target likely face challenges such as traffic congestion, limited ambulance availability, or greater distances to travel, particularly in rural or less populated areas. 

**Does population density of a UCL affect Ambulance response time? (Natasha)**

One of the factors we think could affect the response time of any given area is the population of that area. Our assumption is that with a higher population density there will be an increase in ambulance response times due to a number of reasons such as higher incident rates, higher number of calls, and ambulance staffing limitations. In order to investigate the above, data was sourced from Ambulance Victoria and merged with Census data from the Australian Bureau of Statistics. UCLs that appeared in both datasets were then matched and used for this analysis. As seen in “Total Persons vs Average Response Time (s) - 2018 & 2019”, the total population per UCL (“Total Persons”) was measured against the average response times (“AVG RT – Seconds”) for both 2018 in blue and 2019 in red as a scatter plot with added linear regression. The linear regression shows a slight negative correlation, especially for 2019. This indicates that contrary to the assumption, an increase in population does not exactly impact the response time in any particular area. The statistical analysis may in fact indicate that response times increase in areas with a lower population.

![image](https://github.com/NatashaElliott/challenge-7/blob/main/Data/TotalPersons.png)

In addition to higher population in a densely populated area, we can assume that this will cause an increase in the number of calls to Ambulance Victoria services. As seen in “Total Number of Calls vs Average Response Time (s) - 2018 & 2019”, the total number of calls was measured against the average response times for again, both 2018 in blue and 2019 in red as a scatter plot with added linear regression. Additionally for the purposes of linear regression, the outlier of Melbourne for 2018 was removed as the total calls for Melbourne significantly altered the statistical analysis due to being so far out of the range of the rest of the UCLs. The linear regression still shows a slight negative correlation, however it is a stronger correlation than the previous plot. This could indicate that a greater number of calls will have a strong chance of decreasing the average response time. The stronger correlation suggests that an decrease in the number of calls may impact response times more significantly than a larger population does.

![image](https://github.com/NatashaElliott/challenge-7/blob/main/Data/TotalNumber.png)

Based on these visualisations, population does not seem to have a significant impact on the response times of Ambulance Victoria and almost indicates that lower populated areas have higher response times. As previously mentioned, Ambulance Victoria’s staffing limitations could still be a factor causing increased response times as there may be larger staffing issues in lower populated areas. Additionally lower populated areas can often be more spread out, leading to greater travel distances. Based on this data, we can safely assume that Ambulance Victoria is still improving their response times from 2018 to 2019.


**Does traffic density affect the response time? (Iaroslav)**

The dependency between traffic count vs ambulance response time was analyzed in Victoria.
The idea was to check if the response time depended on the traffic load.

For this pupose, the 

The biggest challenge was to match the traffic count dataset was used
 https://vicdata.vicroads.vic.gov.au/metadata/Traffic_Count_Locations%20-%20Open%20Data.html
 It had geo points in there, but unfortunately no locality names. 
 
 As a result, I resorted to a different dataset which contained various locality names accross Australia and I had to match 
 the geo points from the traffic dfataset to the locality names. That helped me obtain the common dataset with traffci count and the corresponding locality names.
 https://www.peter-johnson.com.au/AustraliaPlaces

The comon dataset had various locality/towns/suburb names and average traffic registered per year.

Than I compared the average traffic against ambulance records for 2019 and plotted scatter charts.

Based on the scatter plots, there is no strong dependency between the traffic count and the wait reaction to calls.
It could be because those topics are totally unrelated or because the service quality is spread rather equally based on the request density. 

There are outliers though. For the average response time, Colac & Drysdale performed the worst. I suppose it needs to be closer verified before making conclusion.
Gisborne hapened to be as another outlier with the best time for quick response.



**Conclusion:**

This analysis of ambulance response times reveals that the data leads to a weak relationship between traffic volume/population density and response times. This may suggest that other variables play a more significant role in shaping efficiencies in Ambulance Victoria meeting their time targets. While many UCLs are close to meeting the 90% response time for Code 1 incidents, and the overall improvement in response times between the years 2018 & 2019, there’s evident room for improvement. Additionally, some limitations to consider include the change in UCL names from 2018 to 2019 in the Ambulance data, and the other datasets (Census data and VicRoads data) where we were not able to match UCL name with the Ambulance data UCL name.
