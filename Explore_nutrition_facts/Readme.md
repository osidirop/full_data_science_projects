In this project an analysis is performed on the [Open Food Facts](https://www.kaggle.com/openfoodfacts/world-food-facts) dataset from Kaggle available under the [Open Database License (ODbL)](https://opendatacommons.org/licenses/odbl/1-0/) after cleaning and exploring the dataset. The project is separated in the following tasks:

**A. Data import, exploratory data analysis (EDA) and cleaning**

**B. In-depth analysis to answer the following:**

1. Are the number of additives correlated with the nutrition score?
2. How the products are classified according to their risk?
3. Are there countries with more or less risky additives?
4. Which product categories have more risky additives?
5. Which product category is most prone to have many additives?

**C. Text normalization in order to find:**

The 5 most common ingredients in the dataset.

**D. Time-series analysis:** 

1. Analyze the mean time difference between the created_datetime and last_modified_datetime. 
2. Analyze the total number of items created each month over the full timeline of the data. 

**E. Build a database**

Build an sqlite3 database with two tables restricted the data to 1000 entries

**F. Finding correlations within the tables:**

Identify the variables which most affect the nutritional score and provide some insight into which factors cause both a low or a high nutritional score. 


Note:
-----
The modified version incorporates the following:
1. (Task C): Commas separate most ingredients. Split the ingredients on the commas and then count them to find the most common ones.
2. (Task F): Quantify the strength of the relationship between the nutrition score and the other macro-nutrients. Numerical ordering of all correlations of the nutrition score with the other features.
3. Cell 19 (Tip) Transposing the output of the describe method improves readability: df_selected.describe().T
4. Cell 28: (Tip for scatterplots): Adapt the transparency of data points with the alpha keyword for overlapping data points.
