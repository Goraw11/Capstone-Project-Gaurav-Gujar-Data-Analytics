# Final Capstone Project - Gaurav Gujar

# Project Objective: Find the G.O.A.T - GreatestCricketer of All Time
Welcome to project, where I tried to answer the question: "Who is the G.O.A.T - Greatest Cricketer of All Time"!
In this project, I have conducted a deep dive into the fascinating world of cricket (and of course cricket stats) to identify and analyze data to determine who can be rightfully crowned as the greatest cricketer of all time. Cricket, a sport deeply ingrained in the cultural fabric of many nations and enjoyed by billions of people, has seen legendary players, leaving a rich and lasting impact on the game's history.

Using my comprehensive data analysis skills, I explored various performance metrics, historical records, and impactful moments in cricketing history. After this, I leveraged many data visualization techniques, statistical modeling, and insightful interpretations, to seek the answer to this question. I must admit, that for some metrics, it was a bit of a challenge to single out 1 player, however, for the metrics that have meaning, and the popular metrics, I did come across one player who's the best of them all.

Below, I will take you through how I achieved this, and answer the timeless question: Who is the G.O.A.T - Greatest of All Time Cricketer?

# Data Collection (Data gathering)
The first challenge was to acquire a dataset - an accurate, meaningful, relatively clean data set.
I researched using various options, and finally landed on a reliable dataset - that of ESPN.
I like the ESPN Dataset for several reasons: 
Reliable (Is a big name in sports stats)
Comprehensive
Rich Data Attributes and variables
Formatted upto a certain degree
Accessible and Open

# Data Cleaning and Wrangling
After finalizing which dataset I was going to use for my project, I started with some cleaning and wrangling type activities:
Initial review
Checking for missing data fields, null values, etc.
Reviewing outliers
Standardizing data
Quality review

I then import loaded the cleaned dataset in Python:
```python
cricket_data = pd.read_csv('SuperCleaned.csv', low_memory=False)
```

# Exploratory Data Analysis (EDA)
After I loaded the dataset in Python, I started on EDA. My goal was to understand the data, its structure, patterns, and relationships. I also used basic data visualizations, and exploratory techniques to find insights and identify interesting trends (And some anomalies). My EDA helped in formulating my hypotheses.
I will provide a very concise snippet of the first couple of steps:

```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
```

```python
# Display the first few rows of the dataset
print("First 5 rows of the dataset:")
print(cricket_data.head())
```

```python
# Display column names
print("\nColumn names:")
print(cricket_data.columns)
```

Again, this is very concise view of my initial steps.

# Further analysis (with a view to cement my hypothesis)
As I was doing further analysis, I also created visualizations within Python to ensure that I am on the right track, and also to ensure that I am making progress to prove my hypothesis. Below, is a code snippet of one of my plots:

```python
# Histogram of batting averages
plt.figure(figsize=(8, 6))
sns.histplot(cricket_data['BATTING_ODIs_Ave'], bins=20, kde=True)
plt.title('Distribution of Batting Averages')
plt.xlabel('Batting Average')
plt.ylabel('Frequency')
plt.show()
```

# Interpretation of Results
After I had found the player who is the Greatest Cricketer of All Time using various metrics on Python, my next task was to translate these, using interesting, clean, and clear visualizations on Tableu.
I loaded the cleaned dataset on to Tableau, and started building a story, with a goal of making it:
1. Clean and clear (And not 'busy')
2. Easy to understand (even for folks who do not understand cricket)
3. To tell the entire story using Tableau Story
4. To make it interactive and immersive, to keep in interesting.

I have shown 1 image, as an illustration, from my final presentation.
![image](https://github.com/Goraw11/Capstone/assets/157068568/4988ea94-bba0-465c-8e3e-7dbcaca02858)

# Tools Used
1. CSV
2. Python
3. Tableau

# Author
Gaurav Gujar, March-April 2024
