# IPL Match Analysis Using Python

An exploratory data analysis project on Indian Premier League (IPL) match data using Python, Pandas, NumPy, and Matplotlib. This project explores team performance, scoring patterns, toss impact, venue statistics, and season-wise comparisons through data analysis and visualizations.

## Project Overview

The Indian Premier League is a competitive T20 cricket tournament where match outcomes can be analyzed through team wins, scoring trends, toss decisions, and winning margins.

This project uses a single IPL match dataset covering seasons from 2008 to 2026 to explore match-level data and identify patterns through simple Python analysis and visualizations.

The goal is to practice practical data analytics skills, turn raw data into meaningful findings, and communicate results using charts.

## Objectives

- Explore and understand IPL match data.
- Identify teams with the highest number of match wins.
- Analyze high-scoring matches and average scoring trends.
- Compare scoring patterns across venues and seasons.
- Examine toss wins and their relationship with match outcomes.
- Analyze winning margins and match counts across seasons.
- Practice data cleaning, aggregation, and visualization using Python.

## Tools and Technologies

- **Python** — Data analysis and calculations
- **Pandas** — Data manipulation, filtering, grouping, and aggregation
- **NumPy** — Numerical computing
- **Matplotlib** — Data visualization
- **Jupyter Notebook / Google Colab** — Analysis environment

## Dataset

**Dataset name:** IPL 2008–2026 Matches Dataset  
**Dataset file:** `IPL_Matches_Data_2008_2026.csv`  
**Original source:** Kaggle  
**Dataset author:** arjunsinghgangwar

The dataset contains match-level information, including teams, seasons, scores, wickets, toss decisions, match winners, venues, and Player of the Match awards.

The analysis uses the provided CSV file without merging another dataset.

## Project Structure

```text
IPL-Match-Analysis/
│
├── IPL_Match_Analysis_Using_Python.ipynb
├── IPL_Matches_Data_2008_2026.csv
└── README.md
```

## Data Exploration and Preparation

The notebook includes the following exploratory checks:

- Dataset dimensions and column inspection
- Data types and statistical summaries
- Missing-value analysis
- Duplicate-row checks
- Examination of matches without a recorded winner
- Investigation of missing match numbers and Player of the Match values
- Review of score and wicket distributions
- Identification of unusually high wicket values
- Creation of a combined-runs column for match-level scoring analysis

Missing values are investigated rather than automatically removed, because some can be associated with ties or matches without a result.

## Analysis and Key Questions

### 1. Match and Scoring Analysis

- What are the 10 highest-scoring matches based on combined team runs?
- How does average combined scoring vary across IPL seasons?
- Which venues have the highest average combined scores?

### 2. Team Performance

- Which 10 teams have the most recorded match wins?
- Which teams have the highest average winning margins in matches decided by runs?

### 3. Toss Analysis

- Which teams have won the toss most often?
- How often does the toss winner also win the match?
- Does the toss winner's success differ between choosing to bat and choosing to bowl?

### 4. Season-Wise Comparisons

- How many matches are recorded in each season?
- How many matches per season were won by the toss winner?
- How does the average winning margin in runs change across seasons?

### 5. Player Awards

- Which players have received the most Player of the Match awards in the dataset?

## Selected Findings

The following findings come from the calculations saved in the notebook:

- **Toss winner and match winner:** In 1,218 matches with a recorded winner, the toss winner also won 628 matches, representing **51.56%**.
- **Toss winner choosing to bat:** The toss winner also won 185 out of 408 matches, approximately **45.34%**.
- **Toss winner choosing to bowl:** The toss winner also won 443 out of 810 matches, approximately **54.69%**.
- **Highest combined-scoring match:** The highest combined score identified in the notebook was 549 runs, from Sunrisers Hyderabad versus Royal Challengers Bangalore on 15 April 2024.

These findings describe the dataset analyzed and should not be interpreted as proof that winning the toss causes a team to win.

## Visualizations

The project uses Matplotlib to create visualizations such as:

- Top 10 IPL teams by total wins
- Average combined runs by season
- Top 5 venues by average combined runs
- Top 5 teams by toss wins
- Top 5 teams by average winning margin in runs
- Total matches played by season
- Matches where the toss winner also won, by season
- Average winning margin by season

The charts help summarize trends and compare match outcomes across teams, venues, and seasons.

## How to Run the Project

### Option 1: Google Colab

1. Download or clone this repository.
2. Open `IPL_Match_Analysis_Using_Python.ipynb` in Google Colab.
3. Upload `IPL_Matches_Data_2008_2026.csv` to the Colab session.
4. Ensure the CSV filename matches the path in the notebook.
5. Run the notebook cells from top to bottom.

### Option 2: Run Locally

1. Clone the repository:

   ```bash
   git clone https://github.com/YOUR-USERNAME/IPL-Match-Analysis.git
   ```

2. Navigate to the project directory:

   ```bash
   cd IPL-Match-Analysis
   ```

3. Install the required libraries:

   ```bash
   pip install pandas numpy matplotlib seaborn jupyter
   ```

4. Start Jupyter Notebook:

   ```bash
   jupyter notebook
   ```

5. Open the notebook and ensure the CSV path points to the local dataset file.

## Skills Demonstrated

- Exploratory Data Analysis (EDA)
- Data inspection and quality checks
- Handling missing values
- Duplicate detection
- Filtering and sorting DataFrames
- Grouping and aggregation with Pandas
- Descriptive statistics
- Creating calculated columns
- Data visualization with Matplotlib
- Interpreting analytical findings

## Limitations

- The analysis is based on the fields available in the supplied match-level dataset.
- Player-level batting and bowling statistics are not included, so individual runs and wickets cannot be analyzed from this file alone.
- Venue averages can be influenced by the number of matches recorded at each venue.
- Season labels use different formats, so chronological ordering should be checked when interpreting season-wise charts.
- Historical team names may differ across seasons.
- The dataset's coverage and values have not been independently verified against official IPL records.

## Future Improvements

- Improve chronological ordering of season labels.
- Add match counts alongside venue scoring averages.
- Compare team performance using win percentages rather than win counts alone.
- Build an interactive dashboard using Power BI or Plotly.
- Add further analysis if a compatible dataset containing individual player statistics becomes available.

## Conclusion

This project demonstrates how Python can be used to explore cricket match data, compare team performance, identify scoring patterns, and investigate the relationship between toss decisions and match outcomes.

It serves as a practical beginner-level data analytics project combining data exploration, Pandas operations, visualization, and evidence-based interpretation.

---

**Author:** Priyank Dewashish  
**Project:** IPL Match Analysis Using Python  
**Domain:** Sports Analytics | Data Analytics