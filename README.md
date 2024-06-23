# Course-Recommending-Course-
We aim to design and evaluate recommendation systems tailored for an online learning platform to enhance user experience through personalised course recommendations. Use methodologies and algorithms to improve user engagement and satisfaction on educational platforms.


This code performs exploratory data analysis (EDA) on a simulated dataset. Here’s a breakdown of what each section does:

1. **Data Creation**: 
   - Generates a synthetic dataset `df` with 10,000 rows and the following columns:
     - `user_id`: Sequential IDs from 1 to 10000.
     - `course_id`: Random integers between 1 and 5000.
     - `course_rating`: Random integers between 1 and 5.
     - `course_duration`: Random integers between 1 and 100.
     - `user_interaction_count`: Random integers between 1 and 50.

2. **Key Statistics**:
   - Prints out descriptive statistics of the dataset using `df.describe()`, which includes count, mean, standard deviation, minimum, 25th percentile (Q1), median (50th percentile or Q2), 75th percentile (Q3), and maximum values for numerical columns (`course_id`, `course_rating`, `course_duration`, `user_interaction_count`).

3. **Data Distributions**:
   - Plots a histogram of the `course_rating` column using `sns.histplot()` from Seaborn. This visualization shows the distribution of course ratings across five bins, with a kernel density estimation (kde) overlay. It helps understand the distribution and concentration of course ratings.

4. **Correlation Analysis**:
   - Creates a scatter plot using `sns.scatterplot()` to explore the relationship between `course_duration` (on the x-axis) and `user_interaction_count` (on the y-axis). This plot visually examines if there is any correlation between the duration of courses and the number of user interactions. 

5. **Outlier Detection**:
   - Displays a boxplot using `sns.boxplot()` of the `user_interaction_count` column. Boxplots are useful for identifying potential outliers in the data distribution. The boxplot summarizes the distribution's central tendency, spread, and highlights any potential outliers.

### Summary:
This code snippet is designed to perform an initial exploration and analysis of the synthetic dataset `df`. It covers:
- Descriptive statistics to understand the basic characteristics of the dataset.
- Visualization of data distributions (`course_rating` histogram).
- Examination of relationships between variables (`course_duration` vs `user_interaction_count` scatter plot).
- Identification of potential outliers (`user_interaction_count` boxplot).

These steps are crucial in understanding the dataset's structure, identifying patterns, correlations, and outliers, which are foundational in any data analysis workflow.
