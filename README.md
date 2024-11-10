# COTECH-Task1
**CO-TECH INTERNSHIP – TASK 1** 
**EXPLORATION EXPLORATORY DATA ANALYSIS (EDA)**

NAME: SAYEEDA MISBAH ILYAS 
COMPANY: COTECH IT SOLUTIONS
ID: CT08DS9133
DOMAIN: DATA SCIENCE
DURATION: OCT - NOV 2024
MENTOR: 
  
**1. PROJECT OVERVIEW** 

- This project performs Exploratory Data Analysis (EDA) on the Iris Dataset to gain insights into the relationships between different features of the iris flowers. The primary objective is to explore the dataset's characteristics, visualize distributions, correlations, and outliers, and analyze the relationships between numerical and categorical variables. The Iris Dataset contains measurements of sepal length, sepal width, petal length, and petal width for three species of iris flowers. This analysis helps in understanding the dataset before applying machine learning algorithms.

**2. Dataset Description**

- The **Iris Dataset** contains 150 observations of iris flowers, with 50 samples from each of the three species:
- Iris setosa, Iris versicolor, and Iris virginica. The dataset includes the following attributes:
•	*Sepal Length (cm)*: Continuous variable representing the length of the sepal.
•	*Sepal Width* (cm): Continuous variable representing the width of the sepal.
•	*Petal Length* (cm): Continuous variable representing the length of the petal.
•	*Petal Width* (cm): Continuous variable representing the width of the petal.
•	*Species*: Categorical variable representing the species of the iris flower, with values: 'Iris setosa', 'Iris versicolor', and 'Iris virginica'.

**STEP 1 - SET UP THE ENVIROMENT**

**Libraries Used**
1. pandas: For data manipulation and analysis (loading, cleaning, transforming data).
2. numpy: For numerical operations and handling arrays.	
3. matplotlib: For creating static, animated, and interactive visualizations.
4. seaborn: For statistical data visualization, including plots like heatmaps, pair plots, and boxplots. 

**1. Data Loading:**
     Load the Iris dataset into a pandas DataFrame from a CSV file.
     
**Step - 2 : Data Exploration:**
             a) df.info -  Provides information on the dataset, such as the number of entries, column names, data types, and null values.
             b) df.dtypes -  Provides Lists the data types for each column
             c) df.head - To read the head the and the first row of the dataset
             d) df.columns - It shows the names of all columns
             e) df.describe - Generates descriptive statistics for each numerical column, including mean, standard deviation, and percentiles.

**Step - 3 : Visual Analysis**
The visual analysis phase involves examining the distributions, relationships, and patterns in the dataset through various types of plots:

**a) Histograms for Feature Distributions:**

*Purpose:* To understand the distribution of each numerical feature (sepal length, sepal width, petal length, and petal width).   
*Insight:* Histograms help reveal whether features are normally distributed, skewed, or bimodal. They also provide a quick overview of ranges and potential variations within each feature. For instance, petal width and petal length typically show more variation across species than sepal measurements.



**b) Pair Plot :**

*Purpose:* To visualize distributions and relationships between all pairs of features simultaneously.
*Insight:* Pair plots provide a grid of scatter plots and histograms for quick, comprehensive insights. In the Iris dataset, pair plots can reveal natural groupings by species and help distinguish which features are the most informative for species classification.

**c) Boxplots for Outlier Detection:**

*Purpose:* To identify potential outliers and the spread of each feature.
*Insight:* Boxplots allow us to observe how data is distributed around the median, revealing skewness, the interquartile range, and outliers. For example, petal width and length often have a greater spread and visible outliers, especially when comparing across species.

 A *correlation matrix* is a table showing the correlation coefficients between pairs of features. Each coefficient ranges from -1 to 1, where:

 1 indicates a perfect positive correlation: as one feature increases, the other does as well.
-1 indicates a perfect negative correlation: as one feature increases, the other decreases.
0 means no correlation: there’s no linear relationship between the features.

In this matrix, the diagonal values are always 1 because each feature is perfectly correlated with itself

This *Heapmap** visually shows the strength and direction of relationships between the features in the Iris dataset. 
- Each cell in the heatmap represents the correlation value between two features, ranging from -1 (strong negative correlation) to +1 (strong positive correlation). 
- Positive values indicate that as one feature increases, the other also tends to increase
- Negative values indicate an inverse relationship. 

This analysis helps identify which features may be more closely related, which is useful for selecting features or understanding patterns in the data.

**INSIGHTS**

***Insights from the Iris Dataset:***
**1. Setosa species has the smallest petal length and width, which is significantly different from Versicolor and Virginica.**
**2.  Virginica species generally has larger sepal and petal dimensions compared to Setosa and Versicolor**  
**4.   There is a strong positive correlation between petal length and petal width, indicating that as petal length increases, petal width also increases**
**5.   Sepal width shows a weak correlation with other features, suggesting it might not be a strong predictor of species on its own.**

**Expected Output**

1. Histograms: Visual representations of the distributions of the numerical features.
2. Boxplots: Visualizations showing the spread of data and potential outliers.
3. Scatter Plots: Charts showing the relationships between pairs of features.
4. Correlation Heatmap: A heatmap illustrating the strength of the relationships between numerical features.
5. Bar Plots and Boxplots for Categorical Data: Visualizations displaying the distribution of species and how numerical features vary across them.

**CONCLUSION**

The **Iris Dataset** offers valuable insights into the characteristics of iris flowers, providing a clear example of how data science techniques can be applied to explore and visualize data. Through EDA, we identified the distribution of features, correlations between them, and visualized outliers. This analysis provides a deeper understanding of the dataset, which is essential for building machine learning models for classification or clustering tasks.

The findings of this EDA can also serve as a foundation for further analysis or modeling, such as applying classification algorithms to predict species based on the flower's attributes.
