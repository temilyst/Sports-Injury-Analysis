# Sports Injury Analysis

Analysis of **15,000 sports injury records** to understand injury patterns, treatment effectiveness, and athlete recovery outcomes.

---

## Project Overview

This project analyzes sports injury data to identify patterns in injury occurrence, recovery outcomes, and treatment effectiveness. The goal is to generate insights that can help improve athlete safety and injury prevention strategies.

---

## Project Objectives

- Identify sports with the highest injury frequency
- Understand the most common injury types
- Analyze treatment effectiveness
- Evaluate injury recurrence rates
- Explore the relationship between training workload and injuries

---

## Tools Used

- Microsoft Excel
- Pivot Tables
- Data Cleaning
- Data Modeling
- Dashboard Design

---

## Dataset Information

The dataset contains **15,000 records** of sports injuries.

### Fact Table

**Injury_Fact_Table**

Columns include:

- Injury_ID
- Athlete_ID
- Sport_ID
- Injury_Type_ID
- Treatment_ID
- Injury_Date
- Recovery_Days
- Recurrence
- Training_Hours
- Age
- Gender
- Severity_Level
- Recovery_Status

Each row represents **one injury event**.

---

### Dimension Tables

#### Sport_Dimension

| Sport_ID | Sport_Name |
|--------|-----------|
| 1 | Football |
| 2 | Basketball |
| 3 | Tennis |

#### Injury_Type_Dimension

| Injury_Type_ID | Injury_Type |
|---------------|-------------|
| 1 | Sprain |
| 2 | Fracture |
| 3 | Muscle Tear |

#### Treatment_Dimension

| Treatment_ID | Treatment_Type |
|-------------|---------------|
| 1 | Physiotherapy |
| 2 | Surgery |
| 3 | Rest |

---

## Data Modeling

A **star schema** was used.

Relationships:

- `Sport_ID` links **Sport_Dimension → Injury_Fact_Table**
- `Injury_Type_ID` links **Injury_Type_Dimension → Injury_Fact_Table**
- `Treatment_ID` links **Treatment_Dimension → Injury_Fact_Table**

This structure improves data organization and analysis performance.

---

## Data Cleaning Steps

1. Removed duplicate records
2. Checked for missing values
3. Standardized injury names
4. Verified column data types
5. Created calculated columns for analysis

---

## Dashboard Features

The Excel dashboard includes:

- Total Injury Count
- Recurrence Rate
- Average Recovery Days
- Injuries by Sport
- Injuries by Injury Type
- Treatment Effectiveness
- Training Workload vs Injury Risk

---

## Key Insights

- Some sports show significantly higher injury frequency
- Certain injuries require longer recovery periods
- Training workload may influence injury likelihood
- Treatment methods impact recovery outcomes

---

## Project Structure

```
Sports-Injury-Analysis
│
├── Data
│   └── [Open Dataset + Dashboard](sport%20injury%20analysis%20the%20real%20deal.xlsx)
│
├── Dashboard
│   └── injury_dashboard.xlsx
│
├── Images
│   └── dashboard_preview.png
│
└── README.md
```

---

## Author

Portfolio project demonstrating **data analysis, data modeling, and dashboard design using Excel**.
