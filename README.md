# Global Well-Being: Exploring the Relationship Between Mental Health, Economic Factors, and Happiness

## Project Overview

Mental health is an increasingly important component of overall well-being, yet it is influenced by many interconnected economic, social, and healthcare factors. This project combines data from global mental health and World Happiness datasets to explore how these factors relate to one another across 92 countries.

Using Python, Pandas, SQLite, and data visualization techniques, this analysis investigates the relationships between national happiness, mental health outcomes, healthcare resources, and socioeconomic indicators.

---

## Research Question

**Main Research Question**

> What factors are most strongly associated with national happiness and mental health outcomes across countries?

### Supporting Questions

1. Is there a relationship between GDP per capita and national happiness?
2. Does greater access to mental health care reduce treatment gaps?
3. Is social media use associated with higher rates of depression and anxiety?
4. Which regions experience the greatest mental health challenges?
5. Which factors appear to have the strongest relationship with national happiness?

---

## Hypothesis

Countries with stronger economies, better access to mental health care, and greater social support will generally report higher happiness scores and better mental health outcomes than countries with fewer healthcare resources and larger treatment gaps.

---

## Datasets

This project combines two publicly available datasets:

- Global Mental Health Crisis Index (2026)  
  https://www.kaggle.com/datasets/alitaqishah/global-mental-health-crisis-index-2026

- World Happiness Report (2019)  
  https://www.kaggle.com/datasets/obaidhere/world-happiness-report

The datasets were merged using each country's ISO3 country code to create a single dataset for analysis.

---

## AI Usage

ChatGPT (OpenAI) was used to assist with:
- brainstorming analysis questions, mainly by inputting my multitude of ideas and having it help me narrow down on them
- creating a page I could use to copy/paste the commonly used code lines, which I used in combination with copy/pasting from my other similar homework I have done previously
- Help with the markdown wordy bits, I told it what I wanted to say, then I pasted their version into notepad and rewrote what was there to be in my own words, and pasted that into the markdown

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SQLite3
- Jupyter Notebook
- Git & GitHub

---

## Project Structure

```
Capstone_Project/
│
├── data/
│   ├── raw/
│   └── cleaned/
│
├── database/
│   └── mental_health.db
│
├── images/
│   └── erd.png
│
├── notebooks/
│   └── capstone.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

---

## Data Preparation

The combined dataset was cleaned using Pandas.

Cleaning steps included:

- Handling missing values
- Inspecting data types
- Renaming columns for consistency
- Verifying duplicate records
- Creating derived variables for analysis

---

## Exploratory Data Analysis

Exploratory data analysis included:

- Summary statistics
- Missing value analysis
- Distribution analysis
- Correlation analysis
- Regional comparisons
- Multiple visualizations including:

  - Scatter plots
  - Regression plots
  - Histograms
  - Bar charts
  - Heatmap

---

## Database Design

The cleaned dataset was normalized into four related SQLite tables:

- Countries
- Mental_Health
- Mental_Health_Resources
- Happiness

The database uses the ISO3 country code as the primary identifier, with foreign key relationships connecting the related tables.

An Entity Relationship Diagram (ERD) was created to illustrate the database design.

---

## SQL

SQLite was used to create and query the relational database.

The project demonstrates SQL concepts including:

- SELECT
- WHERE
- ORDER BY
- GROUP BY
- Aggregate functions
- INNER JOIN

---

## Custom Python Functions

Several reusable Python functions were created to support the analysis, including functions to:

- Classify happiness levels
- Calculate averages
- Identify top-performing countries
- Compute correlations between variables

These functions improve code readability and reduce duplication throughout the notebook.

---

## Key Findings

The analysis identified several important relationships:

- Countries with higher GDP per capita generally reported higher happiness scores.
- Greater access to mental health resources was associated with smaller treatment gaps.
- Social media use showed a moderate positive relationship with anxiety but little relationship with depression.
- Mental health outcomes varied across world regions.
- Social support, healthy life expectancy, and economic prosperity were among the strongest positive indicators of national happiness.

Overall, the findings suggest that national well-being is influenced by a combination of economic, healthcare, and social factors rather than a single variable.

---

## Limitations

This project has several limitations:

- The dataset contains data for 92 countries.
- Correlation does not imply causation.
- Some variables contained missing values.
- The analysis represents a single point in time rather than long-term trends.

---

## Future Work

Future improvements could include:

- Adding multiple years of data to analyze trends over time.
- Incorporating additional socioeconomic indicators.
- Developing predictive machine learning models for happiness or mental health outcomes.
- Expanding the analysis to include more countries and datasets.

---

## How to Run This Project

1. Clone the repository.

```bash
git clone https://github.com/Bach6969/mental_health_statistics.git
```

2. Navigate to the project folder.

```bash
cd mental_health_statistics
```

3. Install the required packages.

```bash
pip install -r requirements.txt
```

4. Launch Jupyter Notebook.

```bash
jupyter notebook
```

5. Open the notebook located in the `notebooks` folder and run the cells in order.

---

## Author

Created as a Keystone Capstone Project demonstrating skills in:

- Python programming
- Data cleaning and analysis
- Data visualization
- Relational database design
- SQL
- Git and GitHub
- Exploratory data analysis