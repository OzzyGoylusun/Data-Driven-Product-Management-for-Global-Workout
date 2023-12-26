# Conducting Market Analysis of Global Workout Trends 

## Table of Contents

- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)
  

### Project Overview
---

This data analysis project in Python is intended to conduct a market analysis to assist a fitness studio based in Philippines with:

- Assessing global demand for workout for the timeframe between mid-March 2018 and mid-March 2023.
- Exploring top 3 fitness keywords searched that generated most interest for workout during various time periods.
- Gauging the split of interest in these three keywords by Philippines and its far/near neighbouring countries, including in Middle East.
- Identifying most popular workout types in Philippines and Singapore.

<p align="center">
  <img src="https://github.com/OzzyGoylusun/Python.-Conducting-Market-Analysis-of-Global-Workout-Trends/blob/main/Visuals/Yoga%20Workout.jpeg"
 alt="Various Workout Types">
</p>

The main goal of these activities is to enable the firm to create unique new digital products and services for its existing customers and potential users informed by a **data-driven product management strategy.**

### Data Sources

There were four fundamental datasets leveraged for this analysis:

- workout.csv
- three_keywords.csv
- workout_global.csv
- geo_three_keywords.csv


### Tools

- [Anaconda Navigator: ](https://www.anaconda.com/download)
  - To access the Jupyter Notebook for **Python**


### Data Preparation

- Found in the *Datasets* folder, all datasets were first inspected and then loaded into various Pandas DataFrames in the appropriate sections of the code.
- During inspection, various duplicated, corrupt and missing aspects of the data were identified.
- Before loading any file into DataFrames, the code was written to pre-emptively handle all problematic parts in the datasets.


### Exploratory Data Analysis

Depending upon Google Trends and also YouTube keyword searches in niche instances, EDA aimed at answering some key questions, such as:

1.  How does the trend of global demand for workout appear for the timeframe between mid-March 2018 and mid-March 2023?
2.  Which of these three keywords - *gym workout*, *home workout* and *home gym*, generated most interest in 2020 and during 2022-2023 separately? 
3.  What are the top 20 countries with the highest interest in workout?
4.  What is the breakdown of the three workout keywords for certain Middle Eastern and South Asian countries (aka. MESA), including Philippines and Singapore?
5.  Based on YouTube keyword searches, which workout type (e.g., yoga, weight lifting) generated highest interest in Philippines during the timeframe at hand?


### Data Analysis

While inspecting datasets that include multiple categorical variables, I realised that if I were to transpose those cat variables from columns into rows, it would help tremendously with my next steps for the exploratory data analysis work.

Hence, I decided to resort to a function, called **stack()**, to achieve this task:

```python
df = file.set_index('Week').stack().reset_index()
```

Prior to that, I had needed to set the index to our 'Week' column so that I would be able to also group each of these three keywords by the datetime parameter without forfeiting it.

### Findings

The critical analysis results are summarised as follows:

1. Interest in workouts tends to be rather seasonal, spiking at the beginning of each year, presumably due to people's part of New Year resolutions.
  - However, there is an anomaly observed in year 2020, with another but more powerful spike in global interest in workouts, shortly following the COVID announcement - in **April 2020**.

<p align="center">
<img src="https://github.com/OzzyGoylusun/Data-Driven-Product-Management-for-Global-Workout/blob/main/Visuals/Global%20Interest%20in%20Workouts.png" alt="Global Interest in Workouts">
</p>
 
2. During the **peak COVID 2020** period, **the home workouts** had stood out as the most popular workout trend, whereas there was subsequently a global shift in trend towards **the gym workouts** from 2022 onwards.

<p align="center">
<img src="https://github.com/OzzyGoylusun/Data-Driven-Product-Management-for-Global-Workout/blob/main/Visuals/Interest%20in%20Type%20of%20Global%20Workouts.png" alt="Global Interest in Type of Workouts">
</p>

3. **United States** in relative terms showed the highest interest in workouts while **Philippines** globally ranked **the 7th spot** where the firm is based. In addition, almost half of the top 20 countries turned out to be based in Middle East or South Asia (MESA).

<p align="center">
<img src="https://github.com/OzzyGoylusun/Data-Driven-Product-Management-for-Global-Workout/blob/main/Visuals/Interest%20in%20Workout%20by%20Country.png" alt="Interest in Workout by Country">
</p>

4. It was fairly interesting to note that, among the other prominent MESA countries in rankings, Philippines came out on top for the population's interest in **home workout**. Nevertheless, the same country ranked the last spot when comes to interest in **home gym**.


### Recommendations

Based on the analysis, I recommend the following actions:

- Invest human and financial capital to devise a data-driven product management strategy.
- Launch marketing communications campaigns in the workout type of **Zumba** designed to alter potential users' behaviour towards visiting the firm's fitness studios.
- Develop products and services designed to interact with users, resistant to leave their homes, in their other areas of workout interest.
- Continue to undertake data researches of similar type every 6 months to stay abreast of new developments in the industry.

### Limitations

All this data analysis work hinges on the datasets made available by DataCamp. By consequence, the accuracy of the findings and proposed suggestions is inherently bound to the integrity of such data.

### References

1. [DataCamp: Project Source](https://app.datacamp.com/)
2. [Python-Pandas: Use of Stack() Function](https://sparkbyexamples.com/pandas/pandas-stack-function/)
4. [Python-Pandas: DateTime Conversion](https://stackoverflow.com/questions/30405413/pandas-extract-year-from-datetime-dfyear-dfdate-year-is-not-working)
5. [Python-Pandas: Manipulation of DateTime into Desired String](https://stackoverflow.com/questions/50188123/remove-days-from-pandas-datetimeindex)
6. [Python-Pandas: Resampling Method](https://stackoverflow.com/questions/71802964/difference-between-pandas-resample-m-and-ms)
7. [Seaborn Library: Setting Background Theme for Graphs](https://seaborn.pydata.org/generated/seaborn.set_style.html)
8. [Seaborn Library: Setting Colour Palette for Graphs](https://seaborn.pydata.org/generated/seaborn.color_palette.html)
