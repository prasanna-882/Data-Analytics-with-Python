# Netflix Dataset Analysis

## Project Overview

This project analyzes Netflix's content library to uncover trends in Movies and TV Shows available on the platform. The analysis focuses on data cleaning, exploratory data analysis (EDA), feature engineering, and visualization to identify patterns related to content type, genre, country, ratings, and content growth over time.

## Business Problem

Netflix offers thousands of Movies and TV Shows from different countries and genres. Understanding content distribution and trends can help stakeholders answer questions such as:

- Which countries contribute the most content?
- What genres are most popular?
- Does Netflix have more Movies or TV Shows?
- How has content availability changed over time?
- What audience ratings dominate the platform?

The goal of this project is to transform raw Netflix data into meaningful insights that support data-driven decision-making.

---

## Dataset Information

The dataset contains information about Netflix Movies and TV Shows.

### Key Columns

| Column Name | Description |
|------------|-------------|
| show_id | Unique content identifier |
| type | Movie or TV Show |
| title | Content title |
| director | Director name |
| cast | Cast members |
| country | Country of origin |
| date_added | Date added to Netflix |
| release_year | Original release year |
| rating | Audience rating |
| duration | Movie duration or TV Show seasons |
| listed_in | Genre/Category |
| description | Content description |

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Data Cleaning

The dataset contained several data quality issues that required preprocessing before analysis.

### Missing Values

The following columns contained missing values:

- Director
- Cast
- Country
- Rating

### Data Cleaning Steps

- Removed duplicate records
- Handled missing values using appropriate techniques
- Converted `date_added` to datetime format
- Standardized text fields
- Checked and corrected data types
- Validated data consistency across columns

---

## Feature Engineering

To improve analysis and generate deeper insights, additional features were created.

### added_year

Extracted the year from the `date_added` column to analyze content growth trends.

### added_month

Extracted the month from the `date_added` column to identify seasonal content addition patterns.

### duration_num

Converted movie durations from text format into numeric values for quantitative analysis.

### genre_count

Calculated the number of genres associated with each title.

### content_age

Created a new feature to determine how old a title is:

```python
content_age = Current_Year - release_year
```

---

## Exploratory Data Analysis (EDA)

### Movies vs TV Shows

Analyzed the distribution of Movies and TV Shows available on Netflix.

### Country-wise Analysis

Identified countries contributing the highest amount of content.

### Genre Analysis

Explored the most common genres available on Netflix.

### Rating Distribution

Analyzed audience ratings to understand target demographics.

### Content Growth Trend

Studied how Netflix content additions changed over the years.

### Release Year Analysis

Examined whether Netflix focuses more on recent or older content.

---

## Visualizations Created

- Movies vs TV Shows Count Plot
- Top 10 Countries by Content
- Top Genres Distribution
- Content Added by Year Trend
- Ratings Distribution
- Release Year Distribution

---

## Key Insights

### Content Type

Movies represent the majority of Netflix content compared to TV Shows.

### Top Countries

The United States contributes the highest amount of content, followed by India and the United Kingdom.

### Popular Genres

Drama, International Movies, and Comedy are among the most common genres.

### Platform Growth

Netflix experienced significant content growth between 2015 and 2019, indicating rapid expansion of its content library.

### Audience Targeting

TV-MA is the most common rating, indicating a strong focus on mature audiences.

### Recent Content Preference

Most content was released after 2010, suggesting a preference for newer titles.

---

## Challenges Faced

### Missing Data

Several important columns contained null values that required handling before analysis.

### Date Conversion

The `date_added` column was stored as text and required conversion into datetime format.

### Multiple Countries in One Record

Many titles were associated with multiple countries, making country-level analysis more complex.

### Mixed Duration Formats

Movies were measured in minutes, while TV Shows were measured in seasons, requiring separate processing.

---

## Project Workflow

1. Data Collection
2. Data Understanding
3. Data Cleaning
4. Feature Engineering
5. Exploratory Data Analysis (EDA)
6. Data Visualization
7. Business Insights Generation

---

## Learning Outcomes

Through this project, I gained practical experience in:

- Data Cleaning
- Data Transformation
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Data Visualization
- Business Insight Generation
- Python for Data Analytics
- Pandas and NumPy Operations
- Matplotlib and Seaborn Visualizations

---

## Conclusion

This project demonstrates how raw data can be transformed into actionable insights through data cleaning, feature engineering, exploratory analysis, and visualization. The findings highlight Netflix's content strategy, audience preferences, and content growth trends, showcasing how data analytics can support business decision-making.
