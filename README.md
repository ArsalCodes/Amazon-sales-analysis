# 📊 Amazon Sales Data Analysis

## 📌 Project Overview

This project analyzes an Amazon product dataset using Python and data analysis techniques. The project focuses on transforming raw data into an analysis-ready dataset, exploring product characteristics and customer feedback, and identifying meaningful patterns that can support data-driven decision-making.

The analysis covers data cleaning, exploratory data analysis, feature engineering, statistical analysis, visualization, and sentiment analysis.

---

## 🎯 Project Objectives

The main objectives of this project were to:

* Clean and prepare raw Amazon product data for analysis.
* Handle missing values and validate the dataset.
* Convert price, discount, rating, and review-related fields into appropriate data types.
* Explore product prices, discounts, ratings, and customer engagement.
* Identify relationships between discounts, ratings, and review activity.
* Analyze customer review sentiment.
* Generate insights from the data using statistical analysis and visualizations.

---

## 📊 Dataset

The original dataset contained **1,465 records and 16 columns**.

After data cleaning and preparation, the working dataset contained **1,463 records and 28 columns**, including engineered features used for further analysis.

The dataset includes information such as:

* Product ID
* Product name
* Product category
* Discounted price
* Actual price
* Discount percentage
* Product rating
* Rating count
* Product description
* Customer reviews
* Review titles
* Product and image links

---

## 🛠️ Tools and Technologies

* **Python**
* **Pandas**
* **NumPy**
* **Matplotlib**
* **Seaborn**
* **TextBlob**
* **Jupyter Notebook**

---

## 🧹 Data Cleaning and Preparation

The raw dataset required significant preprocessing before analysis.

Key data preparation steps included:

* Examining the dataset structure using `head()`, `info()`, and descriptive statistics.
* Checking for missing values.
* Removing records with missing values in key fields.
* Checking for duplicate records.
* Removing currency symbols and commas from price fields.
* Converting price columns to numeric data types.
* Converting discount percentages from text format to numeric values.
* Converting product ratings to numeric format.
* Preparing rating counts for numerical analysis.
* Validating the cleaned dataset.

Examples of the transformations performed include:

```python
pd.to_numeric()
```

and text cleaning techniques to remove:

* `₹` currency symbols
* Commas from numeric values
* `%` symbols from discount percentages

---

## 🔧 Feature Engineering

Additional features were created to support deeper analysis.

These included features related to:

* Cleaned price values
* Numeric discount percentages
* Product price characteristics
* Review length
* Review word count
* Sentiment scores
* Customer sentiment classification

The final working dataset contained **28 columns**.

---

## 🔍 Exploratory Data Analysis

The analysis explored several important questions, including:

### ⭐ Are most products highly rated?

The distribution of product ratings was analyzed to understand overall customer satisfaction.

The results showed that ratings were generally concentrated at relatively high values, suggesting that many products in the dataset received positive customer evaluations.

---

### 💰 Do larger discounts lead to higher ratings?

A scatter plot was used to explore the relationship between discount percentage and product ratings.

The analysis suggested that **larger discounts do not necessarily lead to higher product ratings**. Customer ratings appear to depend on factors beyond the discount offered.

---

### 📈 Do popular products tend to have better ratings?

The relationship between rating count and product rating was examined.

The analysis indicated that products with greater customer engagement may also maintain relatively strong ratings, although popularity alone should not be interpreted as the only factor influencing customer satisfaction.

---

## 😊 Sentiment Analysis

Customer review content was analyzed using **TextBlob** to calculate sentiment polarity.

Reviews were classified as:

* Positive
* Negative
* Neutral

### Sentiment Results

The analysis produced:

* **Positive:** 1,436 reviews
* **Negative:** 26 reviews
* **Neutral:** 1 review

The dataset was therefore dominated by positive sentiment, suggesting generally favorable customer opinions within the analyzed reviews.

---

## 📈 Key Insights

### 1. Most products received relatively positive ratings

Product ratings were generally concentrated around higher values, indicating positive customer evaluations across much of the dataset.

### 2. Larger discounts do not guarantee higher ratings

The relationship between discount percentage and rating did not demonstrate that heavily discounted products automatically receive better customer ratings.

### 3. Customer engagement and ratings can be related

Products with greater numbers of reviews may demonstrate stronger customer engagement and can maintain positive ratings.

### 4. Customer sentiment was overwhelmingly positive

Sentiment analysis classified the majority of analyzed reviews as positive.

---

## 💡 Business Recommendations

Based on the analysis, several recommendations can be considered:

* **Focus on product quality and customer satisfaction rather than relying only on larger discounts.**
* **Use customer reviews and ratings as important signals for understanding product performance.**
* **Monitor highly reviewed products to identify characteristics associated with customer engagement.**
* **Analyze negative customer feedback to identify potential areas for product or service improvement.**
* **Combine quantitative analysis with customer sentiment analysis to gain a broader understanding of customer behavior.**

---

## 📁 Repository Structure

```text
amazon-sales-analysis/
│
├── README.md
│
├── notebooks/
│   └── amazon_sales_analysis.ipynb
│
└── images/
    └── project visualizations
```

---

## 📊 Project Visualizations

Selected visualizations from the analysis will be added to the `images/` directory.

The visualizations include analysis of:

* Product rating distribution
* Discount percentage versus product rating
* Rating count versus product rating
* Customer sentiment distribution

---

## 🚀 Future Improvements

Potential future improvements to this project include:

* Developing an interactive dashboard.
* Performing more advanced statistical analysis.
* Applying machine learning techniques for prediction.
* Conducting deeper natural language processing on customer reviews.
* Comparing product categories in greater detail.

---

## 👤 Author

**Muhammad Ar Salan Khan**

Aspiring Data Analyst focused on:

**Python | Pandas | SQL | Data Cleaning | Exploratory Data Analysis | Data Visualization**

---

⭐ If you found this project interesting, feel free to explore the notebook and connect with me.



![Freq visualization of review](./Images/wordcloud.png)
![Product ratings dist](./Images/product_ratings_dist.png)
![Discount vs Ratings](./Images/discountvsrating.png)

