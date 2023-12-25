# Data-Driven-Product-Management-for-Global-Workout


## Table of Contents

- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)
- [Recommendations](#recommendations)
  

### Project Overview
---

This data analysis project is intended to conduct a market analysis **in Python** to assist a fitness studio based in Philippines with:

- Ident


<p align="center">
  <img src="https://github.com/OzzyGoylusun/Python.-Identifying-and-Visualising-Nobel-Prize-Winners/blob/main/Nobel_Prize.png"
 alt="Alfred Nobel">
</p>



### Data Sources

The dataset used for this analysis is the *"nobel_dataset.csv"* file, containing detailed information about each award winner up to date ever since the Prize was established.


### Tools

- [Anaconda Navigator: ](https://www.anaconda.com/download)
  - To access the Jupyter Notebook for **Python**


### Data Preparation

Only *the nobel_dataset.csv* dataset was first inspected and then imported into a Pandas DataFrame to begin conducting the exploratory data analysis work:


### Exploratory Data Analysis

Depending upon Google Trends and also YouTube keyword searches in niche instances, EDA aimed at answering some key questions, such as:

1.  How does the trend of global demand for workout appear for the timeframe between mid-March 2018 and mid-March 2023?
  - During this period, in which month-year was this demand highest on average?

2.  
3.  
4.  XX
5.  


### Data Analysis

The following code helped me consolidate my knowledge in subsetting, filtering and then grouping the resulting subset by two separate categories for a count-type aggregate operation:

```python
female_winners = nobel_winners_df[nobel_winners_df['sex'] == 'Female'].groupby(['decade',
                                                                                'category']).agg({"prize":"count"})
```

In addition, the code below helped me clear out the blurry lines between a Pandas Series and DataFrames where each one of those have a different set of functions and methods.

By resorting to an integer-based indexing on my Pandas DataFrame below, I was able to fetch what I required and assigned it to a variable:

```python
top_birth_country = nobel_winners_df["birth_country"].value_counts().reset_index().iloc[0,0]
```

### Findings

The critical analysis results are summarised as follows:

1. 
   
2. 
<p align="center">
<img src="https://github.com/OzzyGoylusun/Python.-Identifying-Hidden-Patterns-and-Visualising-Nobel-Prize-Winners/blob/main/Trend%20of%20US-born%20Winners%20per%20Decade.png" alt="Trend of US-born Winners per Decade">
</p>
  
3. 

4. 


### Recommendations



### Limitations



### References

1. [DataCamp](https://app.datacamp.com/)
2. [Python-Pandas: Use of Stack() Function](https://sparkbyexamples.com/pandas/pandas-stack-function/)
4. [Python-Pandas: DateTime Conversion](https://stackoverflow.com/questions/30405413/pandas-extract-year-from-datetime-dfyear-dfdate-year-is-not-working)
5. [Python-Pandas: Manipulation of DateTime into Desired String](https://stackoverflow.com/questions/50188123/remove-days-from-pandas-datetimeindex)
6. [Python-Pandas: Resampling Method](https://stackoverflow.com/questions/71802964/difference-between-pandas-resample-m-and-ms)
7. [Seaborn Library: Setting Background Theme for Graphs](https://seaborn.pydata.org/generated/seaborn.set_style.html)
8. [Seaborn Library: Setting Colour Palette for Graphs](https://seaborn.pydata.org/generated/seaborn.color_palette.html)
