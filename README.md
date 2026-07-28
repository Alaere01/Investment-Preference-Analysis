#  Investment Preference Analysis

##  Project Overview

This project analyzes investor preferences across different investment avenues using survey data. The objective is to identify investment patterns, understand the factors influencing investment decisions, and provide actionable insights through an interactive Power BI dashboard.

The analysis focuses on demographic characteristics, investment objectives, risk preferences, expected returns, and preferred investment channels.

---

#  Project Objectives

The primary objectives of this project are to:

- Analyze the most preferred investment avenues.
- Compare investment preferences by gender.
- Understand investor objectives.
- Identify the major factors influencing investment decisions.
- Examine preferred investment durations.
- Determine the most trusted sources of investment information.
- Build an interactive dashboard that supports data-driven decision making.

---

#  Dataset Information

- **Dataset Type:** Survey Data
- **Total Records:** 40
- **Total Columns:** 24

The dataset contains demographic information and investor responses on:

- Age
- Gender
- Investment Avenues
- Savings Objectives
- Investment Duration
- Expected Returns
- Investment Monitoring Frequency
- Reasons for Choosing Mutual Funds
- Sources of Investment Information
- Factors Influencing Investment Decisions

---

#  Tools Used

- Microsoft Excel
- Power BI
- Power Query
- DAX

---

#  Data Cleaning Process

The dataset was cleaned before analysis using Power Query.

### Data Cleaning Steps

- Imported the dataset into Power BI.
- Checked for missing values.
- Removed duplicate records.
- Standardized text formatting.
- Corrected inconsistent spellings.
- Renamed columns for readability.
- Verified data types.
- Created calculated columns where necessary.
- Unpivoted investment avenue columns for easier analysis.
- Validated data consistency.

---

#  Data Transformation

Several transformations were performed to prepare the dataset for visualization.

These included:

- Creating Age Groups
- Unpivoting investment preference columns
- Creating calculated measures using DAX
- Formatting percentage measures
- Creating ranking measures
- Building relationships where necessary

---

#  DAX Measures

Examples of measures created include:

```DAX
Total Investors = COUNTROWS(Investors)

Male Investors =
CALCULATE(
COUNTROWS(Investors),
Investors[gender]="Male"
)

Female Investors =
CALCULATE(
COUNTROWS(Investors),
Investors[gender]="Female"
)

Male % =
DIVIDE([Male Investors],[Total Investors])

Female % =
DIVIDE([Female Investors],[Total Investors])

Average Age =
AVERAGE(Investors[age])
```

---

#  Dashboard KPIs

The dashboard includes:

- Total Investors
- Male Investors
- Female Investors
- Male Percentage
- Female Percentage
- Average Age

---

#  Dashboard Visualizations

The dashboard contains:

### 1. Investment Avenue Preference

Displays the popularity of:

- Mutual Funds
- Equity Market
- Government Bonds
- Fixed Deposits
- Public Provident Fund (PPF)
- Gold
- Debentures

---

### 2. Investment Preference by Gender

Compares male and female investment choices.

---

### 3. Investment Objective

Shows why investors save money.

Examples include:

- Retirement Planning
- Wealth Creation
- Children's Education
- Emergency Funds

---

### 4. Factors Influencing Investment Decisions

Analyzes:

- Returns
- Risk
- Liquidity
- Lock-in Period

---

### 5. Investment Duration Preference

Displays preferred holding periods.

---

### 6. Sources of Investment Information

Shows where investors obtain financial advice.

---

#  Business Questions Answered

The dashboard answers the following questions:

1. Which investment avenue is most preferred?

2. Which investment avenue is least preferred?

3. Do males and females invest differently?

4. Which savings objective is most common?

5. What factors influence investment decisions the most?

6. Which investment duration is preferred?

7. What is the most trusted source of investment information?

8. Why do investors choose Mutual Funds?

9. How does age influence investment preference?

10. Which investment avenue performs best across different demographic groups?

---

#  Key Insights

## Investment Preferences

- Public Provident Fund (PPF) and Mutual Funds emerged as the most preferred investment avenues.
- Gold and Debentures recorded the lowest preference.

---

## Gender Analysis

- Male and female investors showed similar preferences for safer investment options.
- Minor differences existed in equity-related investments.

---

## Investment Objectives

Retirement planning was the most common savings objective among respondents.

---

## Decision Factors

Expected Returns were the strongest factor influencing investment decisions.

Lock-in Period had the least impact.

---

## Information Sources

Financial Consultants were the most trusted source of investment information.

---

## Investment Duration

Most investors preferred medium to long-term investments over short-term options.

---

#  Recommendations

Based on the findings:

- Promote Mutual Funds and PPF products for conservative investors.
- Educate investors about diversified portfolios.
- Increase awareness of Government Bonds.
- Improve investor education regarding Gold and Debentures.
- Focus marketing efforts around expected returns while educating investors about balancing returns with risk.
- Encourage financial literacy programs through trusted financial advisors.

---

#  Dashboard Preview

<img width="1049" height="590" alt="DASHBOARD" src="https://github.com/user-attachments/assets/043c0747-c634-4e5f-bded-0d4c09957e0d" />

---

#  Future Improvements

Possible enhancements include:

- Larger survey sample
- Geographic analysis
- Income-based segmentation
- Predictive investment modeling
- Investor clustering using machine learning

---

#  Skills Demonstrated

- Data Cleaning
- Data Transformation
- Power Query
- DAX
- Data Modeling
- Data Visualization
- Dashboard Design
- Business Intelligence
- Insight Generation
- Storytelling with Data

---

# Author

*Ebenezer Alaere*

Connect with me on LinkedIn and feel free to explore this project or provide feedback!

---

## ⭐ If you found this project useful, consider giving it a star!
