# A2: U.S. COVID Trends

## Overview
In many ways, we have come to understand the gravity and trends in the COVID-19 pandemic through quantitative means. Regardless of media source, people are consuming more epidemiological information than ever, primarily through reported figures, charts, and maps.

This assignment is your opportunity to work directly with the same data used by the New York Times. While the analysis is guided through a series of questions, it is your opportunity to use programming skills to ask more detailed questions about the pandemic.

You'll load the data directly from the [New York Times GitHub page](https://github.com/nytimes/covid-19-data/), and you should make sure to read through their documentation to understand the meaning of the datasets.

Note, this is a long assignment, meant to be completed over the two weeks when we'll be learning data wrangling skills. I strongly suggest that you **start early**, and approach it with patience. We're asking real questions of real data, and there is inherent trickiness involved.

## Getting Started
You should start this assignment by opening up the `analysis.R` script. The script will guide you through an initial analysis of the data.

* **Coding prompts.** Complete the coding prompts in `analysis.R`.  Your goal is correct code that is understanable.
* **Reflection prompts.** Throughout the script, there are prompts labeled `REFLECTION`. Please write 1 - 3 sentences for each of these prompts below.
As appropriate, provide evidence (e.g., facts from the datasets), give justification for your opinions, or genuinely reflect on your views.  Please strive for concise, clear, and interesting wrirting.

## Reflection Prompts

**R1:** Loading Data
* **R1.a (a)** The county level data differs because there are many more observations, since there is data collected from each county within each state. In addition, the county and state data sets both have a fips column which is not included in the national data set. The county data set gives us the most information on where exactly Covid cases are occuring.
* **R1.a (b)** The similar aspects of each of the data sets are that they all contain a date, cases, and deaths column. Each data set is tracking the number of Covid-19 deaths and cases in the United States, but they are measuring them in different locations.
* **R1.a (c)** Fips stands for Federal Information Processing Standards. These are standards annonced by the National Institue of Standards and Technology to be used in computer system. Fips has specific county and state codes, and those are the numbers observed in the county and state data bases.

**R2**: Exploratory Analysis
* **R2.a (a)** I learned that American Samoa was counted as a state because it was returned at the state with the lowest number of cases. This tells me that the data set includes more than just the 50 states and Washington DC.
* **R2.a (b)** This teaches me that making assumptions about a data set can be dangerous, because before finding this answer I would have just assumed that the locations were only in the 50 states and Washington DC. However, I would have been wrong, so it is always good to test your assumptions and make sure you are working with the same data you assume you are.
* **R2.b** No, because the location with the highest number of cases is Los Angeles county in California whereas the highest number of deaths is in New York City, New York. There could be many reasons why the two locations are different. I remember when the pandemic was just starting, there were a lot of deaths associated with nursing homes in New York, and the elderly have a higher chance of dying from Covid 19. The population in New York City might be more vulnerable, so the proportion of cases who die would be higher.
* **R2.c** Looking at the plots gives you a good sense of at what date Covid cases and deaths spiked, it is also very easy to see the local minimum and maximums. It is interesting to look at the different moving averages and compare them to what was happening at that time.

**R3**: Grouped Analysis
* **R3.a** While you might expect the number of observations to be around fifty, it makes sense that it would be higher. First of all as shown previously, this data set is including more than just the fifty states with because American Samoa is included. Additionally, a few states have multiple counties where there have been no Covid-19 deaths, in this case there is a tie within the state for the location with the lowest number of deaths.

**R4:**: Joins
* **R4.a (a)** When checking the differences in cases between the national, state, and county datasets, I found that there was no difference in cases between the national and state datasets. However I did find differences between the country and state data sets, this leads me to believe that the inconsistency would arise from within the county data.
* **R4.a (b)** The next step for finding where the inconsistency arises would be to determine which states differ from their total sum of cases based on the cases reported in the total of their counties. Finding the location of where the case numbers differ would be the next step, and that would be important in finding out if there is an error.

**R6**: Your Learning
* **R6.a** Something that made me curious while working with this data was getting to create many different data frames which wrangled the data in different ways. For example, it was interesting to find the different locations which still have 0 Covid deaths in the United States. Something that surprised me was how many questions I was able to answer using only three data sets. There seemed like a lot of different analysis that I was able to perform on the data. Something that I would do the same would be to try and debug like I did this time. I can't think of much that I would have done differently for this project.
