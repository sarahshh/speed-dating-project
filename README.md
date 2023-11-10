# speed-dating-project

# Problem statement

Tinder's marketing team needs help on a new project. They are experiencing a decrease in the number of matches, and they are trying to find a way to understand what makes people interested into each other. 
They are asking us to use the dataset "Speed-Dating-Data.csv" in order to provide them with recommendations to increase matches.
This dataset was compiled by Columbia Business School professors Ray Fisman and Sheena Iyengar for their paper Gender Differences in Mate Selection: Evidence From a Speed Dating Experiment. It is publicly available on Kaggle.
Data was gathered from participants in experimental speed dating events from 2002-2004. All participants are from Columbia University. They had to fill in information about themselves, their interests, preferences and rate partners they meet during the speed date.

## Installation Instructions

The project is executed using Python and requires the installation of the following packages :

- pandas
- numpy
- matplotlib
- seaborn
- plotly

These packages can be installed using pip :

```
pip install pandas numpy matplotlib seaborn plotly
```

## How to Use the Dataset

The dataset is a CSV file named 'Speed+Dating+Data.csv'. It can be loaded in Python using the pandas library :

```python
import pandas as pd

df = pd.read_csv('Speed+Dating+Data.csv', encoding= 'ISO-8859-1"')
```

# Methodology 

We leveraged the dataset provided in order to determine which factors influenced matches and which factors didn't influence match decisions.
We used Jupiter Notebook in order to do the Exploratory Data Analysis (EDA).
We also relied on the following data exploration ideas provided on Kaggle:
- What are the least desirable attributes in a male partner? Does this differ for female partners?
- How important do people think attractiveness is in potential mate selection vs. its real impact?
- Are shared interests more important than a shared racial background?
- Can people accurately predict their own perceived value in the dating market?
- In terms of getting a second date, is it better to be someone's first speed date of the night or their last?

# Results & Conclusion

Based on the results obtained throughout the data analysis process, we can provide the following recommendations:

- Highlight attractiveness : it seems that attractiveness plays an important role in potential mate selection for both men ans women, although it seems more important for men compared to women. The dating app could encourage users to upload several pictures of themselves (min. number required), enable filters so users can improve their pictures and therefore increase their attractiveness.
- Broaden the audience : the analysis shows that differences in race, age, field of study or career goal don't influence the participant's decision to see again the partner. Hence, the dating app could suggest a large diversity of profiles to users so they have more choice.
- Leverage shared interests : the results show that shared interests is highly correlated to the partner's decision to see again the partner. Hence, the dating app could ask users to input their interests in a specific section on their profiles and use this information in their algorithm to suggest profiles with similar interests.
- Promote fun : the "fun" attribute appears as decisive for particpants. Therefore, the dating app could showcase the fun traits of users through fun-related prompts (e.g. "Share a funny story about yourself."). They could also allow the upload of videos or voice messages where users could show their fun personalities.
- Display profiles in order of relevance : participants in the study were more likely to say "yes" to their first date than their last date. If we were to translate this finding for a recommendation for the dating app, we could encourage the app to display most compatible profiles as soon as the user opens the app so they have more chances to like it.

Conclusion & Next steps: The analysis of the dataset enabled to provide recommendations to the dating app for an increase in matches and user engagement. However, it's important to note that these findings are specific to this dataset and may not be applicable to other populations or cultures. The dataset contains numerous variables (195) and this analysis only focused on few variables of interest. Next steps could include the analysis of the other variables, and also the use of machine learning techniques to predict decision / matches. 


