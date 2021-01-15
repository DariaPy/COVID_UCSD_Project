# Government response to COVID-19 pandemic: indicators visualisation and correlation analysis

In this project I create the tool to conduct automated monitoring of both COVID statistics and government measures to understand situation and government reaction in different countries on the threats of 2020. I explore the correlation between COVID spread statistics and government response to it.

I used 3 datasets in order to gather pandemic statistics (JHU CSSE COVID-19 Dataset), structured this data by country, region, income level (WDI Dataset) and date since January 1st 2020 till today, and then combined resulting dataset with government response index (Oxford Covid-19 Government Response Tracker) to calculate correlations and get insights on different countries reaction to this threat.

I mostly use pandas built-in methods to work with tabular data, along with several visualization techniques to present the research results.


# Datasets

## Dataset #1:
Name: JHU CSSE COVID-19 Dataset.
Source: https://github.com/CSSEGISandData/

## Dataset #2:
Name: Oxford Covid-19 Government Response Tracker
Source: https://github.com/OxCGRT/

## Dataset #3 (supplementary):
Name: World Development Indicators Dataset (WDI)
Source: http://api.worldbank.org/v2/country/all/indicator/

# Motivation

I decided to explore what new indicators could reveal summary on governments respond to COVID-19 pandemic. Being a municipal servant myself I would like to have the tool to monitor this activity to understand reaction in different countries on the threats of 2020. 

My goal was to write the code that would let me update the information on the fly daily to prepare summary of situation monitoring automatically.
I consider government policies indicators and pandemic statistics to be one of the most interesting datasets to research in mid 2020. I specifically use visualization technics that are different from JHU approach to their famous dashboard and suggest supplementary visual solutions. 

I believe the ideas of this project could be valuable for many people like me who is concerned with pandemic issues or try to compare different governments approaches to this problem.


# Data preparation and cleaning

I described my approach to cleaning and preparation of the data in special paragraphs of each chapter of this project. Particular steps are always related to the structure and completeness degree of the data, as well as my goals in terms of using data: for calculating, for creating animated map, for plotting interactive line graphs, bubble graphs or sunbursts.

The problems I have encountered with the dataset were the following: lack of values for particular countries or dates, excessive values that can not be plotted on map or can not be visible there even if plotted (for example, COVID cases on cruise ships "Diamond Princess and "MS Zaandam“, or in Vatican), wrong ISO-3 codes for the countries, outdated choropleth maps (for example, Kosovo could not be plotted, even though the shape is there, and I cleaned the dataset, and I fixed the ISO-3 codes).

# Research Questions

I have formulated 3 research questions to answer with this project:

- is there a significant correlation between cumulative cases of COVID-19 and cumulative deaths related to it?
- is there a significant correlation between maximum government response index and government healthcare expenditure in previous years?
- is there strong positive correlation between confirmed COVID-19 cases and government response index over time?

# Hypothesis to check

- yes, there is significant positive correlation between cases of COVID-19 and deaths;

- no, strict response to COVID-19 in 2020 and better funding healthcare systems in 2019 are not significantly correlated;

- no, correlation between confirmed cases and government response over time is strong.

### Note: I explore indicators using Russia, Canada, USA, China and Brazil to describe and compare trends. I also plotted world’s average data to provide additional context to comparisons.
