# speed-dating-project

# Problem statement

Netflix would like to know the current state of their catalogue and provided us with a csv file containing the shows released on their platform for streaming from January 2008 to September 2021. It contains 8807 rows/shows and 12 columns.
They would like us to answer the following questions:
- identify which genres are the most present on the platform
- identify in how many countries Netflix content is produced
- identify which country has the most shows
- identify dominant genre per country
- identify if there is seasonality in their catalogue release

## Installation Instructions

The project is executed using Python and requires the installation of the following packages :

- pandas
- numpy
- plotly

These packages can be installed using pip :

```
pip install pandas numpy plotly
```

## How to Use the Dataset

The dataset is a CSV file named 'netflix_titles.csv'. It can be loaded in Python using the pandas library :

```python
import pandas as pd

netflix = pd.read_csv('netflix_titles.csv')
```

# Methodology 

We used Jupiter Notebook in order to perform Exploratory Data Analysis (EDA) of the csv file.
For each question, we started with data cleaning and data processing, then we performed data visualization using plotly.
Indeed, the columns don't have necessarily the right type when importing the csv file and need conversion to be able to manipulate them properly. Also, some columns (such as "country" and "listed_in"/genre) contained multiple values and needed to be broken down into individual values in order to perform analysis.
We also had to pay attention to NA values for the interpretation of the results.


# Results & Conclusion

Based on the results obtained throughout the data analysis process, we can provide the following observations:

- Dominant genres : A recurrent genre was "International Movies" which mean non-US movies, along with "Dramas" and "Comedy". It shows that Netflix is striving to provide relevant content for their non-US customer base.
- Top production countries : US comes as the first production country among Netflix content, followed by India. These 2 countries are top movie producers in the world which explains their top positions in the Netflix catalogue too. 
- Dominant genre per country: by looking at dominant genre per country, we could identify country-specific genres such as "British shows" for the UK, "Anime" for Japan or even "K Dramas" for South Korea. Note that this represents the dominant genre per production country and not the dominant genre among watchers in the country. This could be interesting to get this information to know which genres are most famous in each country.
- Catalogue seasonanility : Looking at 4 types of seasonality (per year, per month, per day of month and per day or week), we can notice that the number of shows added to the platform declined from 2020 mostly due to the covid crisis when it was more difficult to shoot new movies/shows. Also, Netflix has an habbit to add the majority of new shows to the platform on the 1st of the month, and also on Fridays. This way, it can create a sense of anticipation among the customer base and allow people to watch new content during the week-end.

Conclusion & Next steps: The analysis of the dataset enabled to obtain some insights about the Netflix catalogue. Next steps could be to look at the other columns not studied in this project such as "director", "cast", "rating" and "description". Especially the "description" column could be used as part of a NLP project to identify which key words are the most common in shows's descriptions. Also, we noticed that Netflix has a high number of genres on the platform (42) and a next step could be to look at how to regroup some of these genres together to decrease the number of genres, making the analysis easier.


