# MIST4610-Project2

# 21479_8 Members
- [Emma Dolson](https://github.com/eld49325/EmmaDolson_MIST4610GroupProject2)
- [Hannah Kelly](https://github.com/hannahkelly98765/MIST-4610-Tableau)
- [Shir Kochi](https://github.com/shirkorchi/MIST4610-Project2)
- [Donovan Vanderpool](https://github.com/donovanv2/MIST4610Project2)
- [Kaden Williams](https://github.com/kadenwilliams1/MIST4610Project2)

# Data Set
This data was pulled from the US Energy Administration and joined together for an easier analysis. It is a collection of major factors that play into C02 emissions, from the Production and Consumption of each type of major energy source for each country to its pollution rating each year. It also includes each countries GDP, Population, Energy intensity per capita (person), and Energy intensity per GDP (per person GDP). All the data spans all the way from the 1980's through 2019.

Feature Descriptions and Data Types:

Country: Country in question (String)
Energy_type: Type of energy source (String)
Year: Year the data was recorded (DATE)
Energy_consumption: Amount of Consumption for the specific energy source, measured (quad Btu = 10¹⁵ British thermal unit) (Decimal)
Energy_production: Amount of Production for the specific energy source, measured (quad Btu) (Decimal)
GDP: Countries GDP at purchasing power parities, measured (Billion 2015$ PPP) (Decimal)
Population: Population of specific Country, measured (Mperson) (Decimal)
Energy_intensity_per_capita: Energy intensity is a measure of the energy inefficiency of an economy (MMBtu/person) (Decimal)
Energy_intensity_by_GDP: Energy intensity is a measure of the energy inefficiency of an economy (1000 Btu/2015$ GDP PPP) (Decimal)
CO2_emission: The amount of C02 emitted, measured (MMtonnes CO2) (Decimal)

# Question 1
People have employed several approaches to curbing CO2 emissions, ranging from policy changes and regulations to technological advancements and behavioral changes. In 2019, Prince Harry and Meghan Markle announced they would limit their family size to two children, citing environmental reasons. This led people to question if family planning is an effective solution to reducing CO2 emissions. Population growth has been linked to increased CO2 emisssions as increased demand for resources, including energy, food, and transportation, which all contribute to greenhouse gas emissions. However, it is important to note that the correlation between population and CO2 emissions is not straightforward, as other factors such as economic development contribute to CO2 emissions. Economic growth is often accompanied by increased energy demand for transportation, manufacturing, construction, and other sectors, resulting in increased CO2 emissions. This prompted us to ask the question:

Is there a stronger correlation between CO2 emissions and GDP or CO2 emissions and population?

# Question 1 Analysis and Report
![image](https://user-images.githubusercontent.com/128431687/234630675-b5529859-0cf6-4263-9242-9cd57e9bc065.png)

For the top two graphs, we examined the top five countries with the highest CO2 emissions overall (China, US, India, Russia, and Japan). In doing so, the data points are more visible and eliminate less significant countries that could possibly skew the data.
For the top two graphs, we examined the top five countries with the highest CO2 emissions overall (China, US, India, Russia, and Japan). In doing so, the data points are more visible and eliminate less significant countries that could possibly skew the data.

Looking at the visualization between Energy Intensity by GDP vs Energy Intensity per capita, we observed both measures following similar trends year to year with the exception of China. After 2013, China's Energy Intensity by GDP decreases while its Energy Intensity per capita continues to increase. Upon further research, we found this was a result of China's energy restructuring to increase production from its statewide power generators and reduce its reliance on coal. With the other countries' Energy Intensity by GDP and Energy Intensity per capita following parallel trends, the graph reaffirms our hypothesis that GDP and population are contributing factors towards CO2 emissions.

The visualization between Population and GDP shows us there may not be a strong correlation between population and GDP themselves. Looking at the United States, it has the highest GDP in the world yet it has a significantly smaller population compared to China and India. From this graph, we can assume these disparaties will lead to a difference in the correlation between CO2 emissions and population and the correlation between CO2 emissions and GDP.

In the bottom two graphs, we ran a linear regression on the correlation between CO2 emissions and population and the correlation between CO2 emissions and GDP. For both population and GDP, the p-values were less than 0.0001 and reaffirmed our hypothesis that they were statistically significant in contributing to CO2 emissions. The R-squared for CO2 emissions and GDP was 0.8693, which was higher than the R-squared between CO2 emissions and population of 0.6276. This answers our question as the CO2 emissions and GDP has a stronger correlation than the correlation between CO2 emissions and population. The implication of our findings suggests economic policies may have a stronger effect on reducing CO2 emissions than population control.

# Question 2
The Paris Climate Agreement is a global treaty that was adopted in 2015 by 196 countries with the goal of limiting global warming to well below 2°C above pre-industrial levels and pursuing efforts to limit it to 1.5°C. The agreement requires each country to set its own targets for reducing greenhouse gas emissions and regularly report on their progress. While many countries have made efforts to reduce their greenhouse gas emissions, some countries' commitments fall short of the global warming goal and other countries have withdrawn from the agreement or not yet ratified it. In 2017, the U.S. was one country that withdrew from the Paris Climate Agreement only to rejoin it in five years later. With the controversy surrounding its' validity, we used our datset to answer the question:

How effective has the Paris Climate Agreement been in reducing CO2 emissions?

# Question 2 Analysis and Report
![image](https://user-images.githubusercontent.com/128431687/234630624-6cda92e5-d9de-40b3-b7ee-7d0ae8f60b25.png)

Visualizing CO2 emissions worldwide, CO2 levels did decline in the two years after the agreement's inception from 2015 to 2017. However, CO2 emissions reached a record high after 2017 and from the dataset we can see they continue to increase through 2019. The International Energy Agency (IEA) accounted two-thirds of the global emissions increase to Asian countries, particularly China.
Visualizing CO2 emissions worldwide, CO2 levels did decline in the two years after the agreement's inception from 2015 to 2017. However, CO2 emissions reached a record high after 2017 and from the dataset we can see they continue to increase through 2019. The International Energy Agency (IEA) accounted two-thirds of the global emissions increase to Asian countries, particularly China.

A Climate Action Tracker (CAT) report found that all G20 countries were failing to meet the commitment made in the Paris Agreement and several countries' pledges were highly insufficient in reducing CO2 emissions at a significant level. Four G20 countries (Britain, United States, Mexico and Japan) did experience declines in their CO2 emissions during 2017 but they are far outweighed by the increases in emissions from China and Russia.

By focusing on the CO2 emissions of Asian countries, we can see the top three emitters (China, India, and Russia) all increased their emissions after 2017. It is also important to note those three are also a part of the Paris Climate Agreement. In terms of Asian countries that have not ratified the agreement, major oil producers Iran and Iraq also saw an increase in CO2 emissions.

In an attempt to answer our question, the Paris Climate Agreement is a loose commitment to reducing CO2 emissions. Without a regulatory body, countries are not held accountable for their pledges or their actions taken to honor them. For countries like the US who made sufficient commitments to the agreement, they saw a reduction in CO2 emissions. However, if other countries like China and Russia, are allowed to continue increasing their CO2 emissions without consequence, the progress made by others becomes mute. The implication of this is dangerous as it could lead to the prisoner's dilemma in which case all countries favor their own benefits of not reducing CO2 emissions over the mutual benefit of reduced CO2 emissions worldwide.

# Manipulations
No manipulations or calculations were performed on the data set. For relevance, we filtered our time period to the decade of 2009-2019 to reduce outliers and to exclude countries that no longer exist (e.g. USSR, West and East Germany).

# Sources
Chestney, N. (2018, March 22). Global carbon emissions hit record high in 2017. Reuters. Retrieved April 26, 2023, from https://www.reuters.com/article/us-energy-carbon-iea/global-carbon-emissions-hit-record-high-in-2017-idUSKBN1GY0RB

Guo, X., Xiao, B., & Song, L. (2022, July 29). What cause the decline of energy intensity in China's cities? A comprehensive panel-data analysis. ScienceDirect. Retrieved April 26, 2023, from https://www.sciencedirect.com/science/article/pii/S095965261932030X#sec4

Lai, O. (2021, September 17). Every G20 Country Is Failing to Meet Paris Agreement On Climate Change. Earth.Org. Retrieved April 26, 2023, from https://earth.org/every-g20-country-is-failing-to-meet-paris-agreement-on-climate-change/
