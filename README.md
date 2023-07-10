# Lede Program 2023

This is a classwork assignment for [The Lede Program at Columbia's Graduate School of Journalism](https://ledeprogram.com), Summer 2023

## Topic

Intro To Pandas & Matplotlib

## DBackground

I was given two .csv files **continent_facts** and **countries**. These .csv files contained global information on the life expectancy, population, and GDP of each country on every continent. I used pandas to analyze the data and create new dataframes and matplotlib to visualize the data.


## Data Analysis Exports

**Calculating GDP Per Capita** = I created a new data frame with GDP per capita using the calculation of GDP divided by population `df.gdp/df.population` . To add this new column into the header I used `df['gdp_per_capita'] = df.gdp / df.population
df.head()` and then saved it as a new file entitled **cont_total.csv** using `df.to_csv("cont_total.csv", index=False)`

**Merging Datasets** = I created new dataframes in the **countries.csv** file to analyze the data. I then pulled in **continent_facts.csv** to convert the series into a new dataframe to include overlapping data in both documents. The result is the **merged_datasets.csv**

**Calculating Life Expectancy, By Continent** = To find the average life expectancy by continent: `df.groupby(by='continent')life_expectancy.median()` . I then rounded it with `df.groupby(by='continent').life_expectancy.median().round()` and sorted it in descending order `df.groupby(by='continent').life_expectancy.median().sort_values(ascending=False)`

**MatplotLib** I made a scatter plot with of the countries with the X-Axis as GDP Per Capita and the Y-Axis as Life Expectancy and a bar graph of continents with the Y-Axis as the continent and the X-Axis as the median life expectancy.

## Contact

Student: Amanda Cohen
Program Director: Jonathan Soma, Columbia University
