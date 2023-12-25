# Identification of Global Workout Trends for Discovery of Sought-After Training Programs


## Table of Contents

- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)
  

### Project Overview
---

This data analysis project is intended to conduct a market analysis **in Python** to assist a fitness studio based in Philippines with:

- Ident


<p align="center">
  <img src=""
 alt="Alfred Nobel">
</p>



### Data Sources

There were four fundamental datasets leveraged for this analysis as follows:

- workout.csv
- three_keywords.csv
- workout_global.csv
- geo_three_keywords.csv


### Tools

- [Anaconda Navigator: ](https://www.anaconda.com/download)
  - To access the Jupyter Notebook for **Python**


### Data Preparation

- Found in the *Datasets* folder, all datasets were first inspected and then loaded into various Pandas DataFrames in the appropriate sections of the code.
- During inspection, duplicated, corrupt and missing aspects of the data were identified.
- Before loading any file into DataFrames, the code was written to pre-emptively handle all problematic parts in the datasets.


### Exploratory Data Analysis

Depending upon Google Trends and also YouTube keyword searches in niche instances, EDA aimed at answering some key questions, such as:

1.  How does the trend of global demand for workout appear for the timeframe between mid-March 2018 and mid-March 2023?
  - During this period, in which month-year was this demand also highest on average?

2.  Which of these three keywords - *gym workout*, *home workout* and *home gym*, generated most interest in 2020 and also during 2022-2023 separately? 
3.  What are the top 20 countries with the highest interest in workout, which hinges on this keyword search?
4.  What is the breakdown of the three workout keywords for certain Middle Eastern and South Asian countries (aka. MESA), including Philippines and Singapore?
5.  Based on YouTube keyword searches, which workout type (e.g., yoga, weight lifting) generated highest interest in Philippines during the timeframe at hand?


### Data Analysis

```python

```

### Findings

The critical analysis results are summarised as follows:

1. Interest in workouts tends to be rather seasonal, spiking at the beginning of each year, presumably due to people's part of New Year resolutions.
  - However, there is an anomaly observed in year 2020, with another but more powerful spike in global interest in workouts, shortly following the COVID announcement - in **April 2020**.

<p align="center">
<img src="https://github.com/OzzyGoylusun/Data-Driven-Product-Management-for-Global-Workout/blob/main/Visuals/Global%20Interest%20in%20Workouts.png" alt="Global Interest in Workouts">
</p>
 
2. During the **peak COVID 2020** period, **the home workouts** had stood out most as the most popular workout trend, whereas there was subsequently a global shift in trend towards **the gym workouts** from 2022 onwards.

<p align="center">
<img src="https://github.com/OzzyGoylusun/Data-Driven-Product-Management-for-Global-Workout/blob/main/Visuals/Interest%20in%20Type%20of%20Global%20Workouts.png" alt="Global Interest in Type of Workouts">
</p>

3. **United States** in relative terms showed the highest interest in workouts, and **Philippines** globally ranked **the 7th spot**, while almost half of the top 20 countries turned out to be based in Middle East or South Asia (MESA).

<p align="center">
<img src="https://github.com/OzzyGoylusun/Data-Driven-Product-Management-for-Global-Workout/blob/main/Visuals/Interest%20in%20Workout%20by%20Country.png" alt="Interest in Workout by Country">
</p>

4. It was fairly interesting to note that, among the other prominent MESA countries in rankings, Philippines came out on top for the population's interest in **home workout**. Nevertheless, the same country ranked the last spot when comes to interest in **home gym**.


### Recommendations



### Limitations



### References

1. [DataCamp: Project Source](https://app.datacamp.com/)
2. [Python-Pandas: Use of Stack() Function](https://sparkbyexamples.com/pandas/pandas-stack-function/)
4. [Python-Pandas: DateTime Conversion](https://stackoverflow.com/questions/30405413/pandas-extract-year-from-datetime-dfyear-dfdate-year-is-not-working)
5. [Python-Pandas: Manipulation of DateTime into Desired String](https://stackoverflow.com/questions/50188123/remove-days-from-pandas-datetimeindex)
6. [Python-Pandas: Resampling Method](https://stackoverflow.com/questions/71802964/difference-between-pandas-resample-m-and-ms)
7. [Seaborn Library: Setting Background Theme for Graphs](https://seaborn.pydata.org/generated/seaborn.set_style.html)
8. [Seaborn Library: Setting Colour Palette for Graphs](https://seaborn.pydata.org/generated/seaborn.color_palette.html)
