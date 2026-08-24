# Assignment 2: Data Wrangling and Exploratory Analysis

## 1. Question Explored

This analysis explored the relationship between penguin physical characteristics, particularly flipper length and body mass. I also compared the average body mass and flipper length across different penguin species.

The Palmer Penguins dataset was selected because it contains more than 200 observations and includes both numerical and categorical variables, making it suitable for practicing data cleaning, GroupBy aggregation, merging, NumPy computation, and visualization.

## 2. Data Cleaning and Analysis

The dataset was inspected for its shape, column names, data types, missing values, and unique values. Missing observations were removed because only a relatively small number of rows contained missing values, leaving enough observations for analysis. Duplicate rows were also checked and removed where necessary.

For feature engineering, I grouped the data by penguin species and calculated the average body mass and average flipper length for each species. These summary statistics were then merged back into the cleaned dataset.

I also used NumPy to standardize the body mass values. The standardized values were calculated using a vectorized operation without an explicit Python loop and were added to the dataframe as a new feature.

## 3. Findings

The analysis shows a positive relationship between flipper length and body mass. In general, penguins with longer flippers tend to have greater body mass. This relationship is shown in **Figure 1**, saved as `a2_chart1.png`.

The comparison by species also shows differences in average body mass. The species-level aggregation makes it possible to compare the typical body mass of the different penguin species. This finding is shown in **Figure 2**, saved as `a2_chart2.png`.

The GroupBy and merge operations were useful because they allowed species-level statistics to be calculated and then attached to each individual penguin record for further analysis.

## 4. Limitation

One limitation of this analysis is that the dataset contains measurements from a limited number of penguin species and locations. Therefore, the findings should not automatically be generalized to all penguin populations. In addition, removing rows with missing values may have reduced the amount of available data.

## 5. Reflection

### Which transform took the longest to get right, and why?

The merge operation took the longest to get right because it required understanding how the GroupBy results were structured and how the `species` column could be used as the key to join the summary information back to the main dataframe. Checking the dataframe shape before and after the merge helped confirm that the transformation worked correctly.

### What would you do differently with another dataset?

With another dataset, I would spend more time understanding the variables before starting the transformations. I would also compare different approaches to handling missing values instead of immediately removing rows. Finally, I would choose visualizations based more directly on the research question and the types of variables available in the dataset.
