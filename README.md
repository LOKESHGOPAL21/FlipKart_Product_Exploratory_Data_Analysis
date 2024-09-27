# Project Documentation: Exploratory Data Analysis on Flipkart Product Dataset

# 1. Project Overview
This project focuses on performing Exploratory Data Analysis (EDA) on a dataset scraped from Flipkart, a popular e-commerce platform. The dataset contains various features about products, such as their categories, ratings, prices, seller information, and descriptions. The goal of this analysis was to clean the dataset, handle missing values, and derive insights using univariate and bivariate analysis, represented through various visualizations.

# 2. Dataset Description
The dataset consists of the following features:

Category1, Category2, Category3: Specify the division (primary, secondary, and tertiary categories) to which each product belongs.<br>
Title: Title of the product listed on Flipkart.<br>
Product Rating: Customer-based rating for the product.<br>
Selling Price: The price at which the product was sold at the time of data scraping.<br>
MRP: Maximum Retail Price (MRP) of the product.<br>
Seller Name: Name of the business or individual selling the product.<br>
Seller Rating: Customer-based rating for the seller.<br>
Description: Product description (if available).<br>
Highlights: Key highlights of the product (if available).<br>
Image Links: URLs for images of the products.<br>
3. Steps Followed in the Project
3.1 Importing Required Libraries
I started by importing the necessary Python libraries such as:

#pandas for data manipulation and analysis,
#matplotlib and seaborn for creating visualizations.
#3.2 Reading the Dataset
The dataset was loaded into a Pandas DataFrame using the .read_csv() function for further analysis:

# 3.3 Dropping Unrequired Columns
Certain columns that were irrelevant to the analysis were dropped using the .drop() function to streamline the dataset.

# 3.4 Retrieving Columns of the DataFrame
I retrieved all the columns of the dataset to understand the structure of the data using df.columns.

# 3.5 Getting Information About the Dataset
I used .info() to get a comprehensive understanding of the data types, column names, and the presence of null values.

# 3.6 Handling Missing Values
Missing values were identified in certain columns. I found that rows containing NaN values were not relevant, so they were replaced with suitable values depending on the data type of each column. For example:<br>

Numeric columns were filled with the median of the column.
Categorical columns were filled with the mode of the column.
3.7 Univariate Analysis
For univariate analysis, I focused on studying each column of the dataset individually to understand the distribution and characteristics of the data.

Key Steps:
Pie Chart for Category1: I represented the unique values of the Category1 column and their respective percentages using a pie chart.
Bar Plot for Category2: A bar plot was used to represent the 10 most frequent values in Category2, showing their occurrences.
Horizontal Bar Plot for Category3: A horizontal bar plot visualized the occurrences of the 10 most common values in the Category3 column.
Product Rating Visualization: A sample of 10 ratings from the Product Rating column was plotted to show their frequency. Additionally, I used a boxplot to represent the distribution of product ratings.
3.8 Bivariate Analysis
In bivariate analysis, I studied the relationships between two variables at a time.

Key Steps:
Boxplots for Various Columns: Boxplots were created to understand the distribution of various columns such as Product Rating and Selling Price.
Selling Price vs Product: A graph was plotted to represent 10 randomly selected products and their corresponding selling prices.

# 4. Key Insights from the EDA
Product Categories: From the univariate analysis, I found that Category1 had a clear distribution with specific categories dominating the dataset.
Selling Prices: Selling prices showed significant variance, with some products being sold well below their MRP. A comparative analysis of Selling Price and MRP indicated that many products had substantial discounts.
Seller Rating Distribution: Similar to product ratings, most sellers had ratings 5, with few extreme values.

# 5. Visual Representations
Pie Chart for Category1: Showed the proportion of different categories.
Bar Plot for Category2 and Category3: Visualized the top 10 frequent values.
Boxplots for Product Rating and Selling Price: Helped in identifying the spread and outliers in the data.
Graph for Product Ratings: Demonstrated the frequency of ratings.

#6. Conclusion
This exploratory data analysis provided a comprehensive view of the Flipkart product dataset. The cleaning process ensured that missing values were appropriately handled, and both univariate and bivariate analyses provided useful insights into the relationships between product categories, prices, ratings, and sellers. Visualizing the data helped highlight trends, such as pricing strategies and customer feedback distribution, making the dataset easier to interpret and analyze.

#Tools and Libraries Used:
#Python Libraries:
Pandas, Matplotlib, Seaborn
#Methods: 
Univariate and Bivariate Analysis, Data Cleaning, Visualization (Pie charts, Bar plots, Boxplots)
