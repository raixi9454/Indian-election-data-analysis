
# Indian Election Data Analysis

**An end-to-end data analysis and visualization project on Indian Parliamentary Elections**  
**Technologies used:** Python (Pandas) for data wrangling, Tableau Desktop for visual storytelling

---

## 📌 Project Overview

This project leverages publicly available data on Indian General Elections to uncover insights into voting behavior, candidate demographics, party performance, and constituency-level dynamics across India. The goal is to prepare a clean, analysis-ready dataset and create a series of interactive Tableau dashboards to support data-driven understanding of electoral trends.

---

## 🎯 Objectives

- Clean and standardize raw election data for analytical use  
- Analyze patterns in voter turnout, candidate participation, and party representation  
- Build interactive Tableau dashboards to visualize election trends by state, year, gender, and party  

---

## 🧰 Tools & Technologies

| Tool            | Purpose                          |
|------------------|----------------------------------|
| **Python**       | Data cleaning and transformation |
| **Pandas**       | Data wrangling and preprocessing |
| **Jupyter**      | Interactive coding environment   |
| **Tableau Desktop** | Dashboarding & data visualization |

---

## 🗂️ Project Structure

```bash
Indian-election-data-analysis/
├── Election_clean.ipynb          # Jupyter notebook for data preprocessing
├── Indian_election_dataset.csv   # Raw election dataset
├── election_cleaned.csv          # Cleaned, transformed dataset
├── Tableau_dashboard.twbx        # Tableau dashboard (if available)
└── README.md                     # Project documentation
```

---

## 🔧 Data Cleaning Process

The notebook `Election_clean.ipynb` performs the following key steps:

- **Column Dropping:** Removed non-informative columns such as `pc_no`, `partyabbre`  
- **Duplicate Removal:** Ensured data uniqueness using `.drop_duplicates()`  
- **Column Renaming:** For clarity and consistency:

  | Original Column         | New Column                    |
  |-------------------------|-------------------------------|
  | `st_name`               | `state`                       |
  | `pc_name`               | `parliamentary_constituency` |
  | `cand_sex`              | `cand_gender`                 |
  | `partyname`             | `party_name`                  |
  | `totvotpoll`            | `Total_Votes_Polled`          |
  | `pc_type`               | `constituency_type`           |

- **Data Summary:** 73,079 records, 9 relevant columns  
- **Missing Values:** Identified and handled during Tableau processing  

---

## 📊 Tableau Visualizations

The data is visualized using Tableau Desktop with interactive dashboards featuring:

- 🧍‍♂️ **Gender Representation:** Candidate distribution by gender and state  
- 🗳️ **Voter Turnout Analysis:** Polled vs total electors across regions and years  
- 🏛️ **Party Performance:** Vote shares and winning patterns by political parties  
- 📍 **Constituency Type Distribution:** General, SC, ST seat classification over time  

> 📁 Open the dashboard in Tableau Desktop: `Tableau_dashboard.twbx`

---

## 📈 Sample Dataset Schema

| Column Name                 | Description                             |
|----------------------------|-----------------------------------------|
| `state`                    | Indian state or UT name                 |
| `year`                     | Election year                           |
| `parliamentary_constituency` | Constituency name                    |
| `constituency_type`        | General, SC, or ST seat classification  |
| `cand_name`                | Candidate name                          |
| `cand_gender`              | Candidate gender (Male/Female/Other)    |
| `party_name`               | Political party                         |
| `Total_Votes_Polled`       | Number of votes polled                  |
| `electors`                 | Total registered voters                 |

---

## 🚀 How to Run the Project

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/Indian-election-data-analysis.git
cd Indian-election-data-analysis
```

### 2. Run the Notebook
Launch `Election_clean.ipynb` in Jupyter to preprocess the dataset.

### 3. Load Data into Tableau Desktop
Open `election_cleaned.csv` in Tableau Desktop to explore or build your dashboard.

---

## 📃 License

This project is licensed under the **MIT License**.  
You are free to use, modify, and distribute with proper attribution.

---

## 🙋‍♀️ Acknowledgements

- Election Commission of India (data source)  
- Python & Tableau community for tools, packages, and documentation  
