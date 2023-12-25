# Data-Driven-Product-Management-for-Global-Workout

# Python- Identifying Hidden Patterns and Visualising All Nobel Prize Winners

## Table of Contents

- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Findings](#findings)

### Project Overview
---

This data analysis project conducted via **Python** is intended to identify undiscovered patterns by exploring some intriguing Nobel Prize winner data. 

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

EDA involved exploring XXX data to answer key questions, such as:

1.  
2.  
3.  
4.  


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

1. X
2. XX
3. [Seaborn: Setting Background Theme for Graphs](https://seaborn.pydata.org/generated/seaborn.set_style.html)
4. [Seaborn: Setting Colour Palette for Graphs](https://seaborn.pydata.org/generated/seaborn.color_palette.html)
