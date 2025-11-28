# IPL_Franchise_Team_Analysis-Python_Project
This project builds a data-driven IPL Franchise Team based on player performance from 2021 to 2024.
Using Python and Jupyter Notebook, the analysis focuses on selecting an optimal, role-balanced XI using unique scoring techniques and statistical insights.

## 🎯 Project Summary
Over four IPL seasons (2021–2024), hundreds of players batted, bowled, and contributed differently. Instead of simply picking top run-scorers or wicket-takers, this project analyzes:

- Multi-season performance
- Player consistency
- Role-specific strengths
- Statistical normalization
- Balanced team-building logic
- Visual pattern recognition

The final result is a high-impact Franchise XI backed by data — reliable, balanced, and optimized for real match conditions.

## 📁 About This Notebook
This project is entirely contained in one Jupyter Notebook, which includes:

- Data cleaning
- Player performance analysis
- Visualizations
- Scoring system
- Team optimization logic
- Final selected IPL XI

There is no external script — all logic, visuals, and outputs are in a single notebook for easy review.

## 📊 Dataset Used

**Source:** Kaggle IPL Dataset  

**Files analyzed:**
- `matches.csv`
- `deliveries.csv`

**Filters applied:**
- Seasons from **2021 to 2024**
- Minimum **3 matches** for player inclusion


## 🧹 Data Cleaning & Preparation

During preprocessing, the following steps were performed:

- ✔️ Loaded IPL datasets (`matches.csv` and `deliveries.csv`)
- ✔️ Converted data types (balls, overs, runs, wickets)
- ✔️ Extracted `season_year` from match dates
- ✔️ Merged match data with ball-by-ball deliveries
- ✔️ Removed missing or incomplete records
- ✔️ Filtered data to include seasons **2021 to 2024** only

These steps ensure the analysis uses clean, relevant, and high-quality data.

## 🏏 Batting Performance Analysis

For each IPL season from **2021 to 2024**, batting performance was evaluated using:

- Total runs scored
- Balls faced
- Strike rate
- Matches played (minimum 3)
- Season-wise ranking of top batsmen

### 🔍 Insight
This analysis helps identify **consistent batting performers** across multiple seasons rather than one-season peaks.

### 📈 Visualization
**Top Batsmen Runs Trend (2021–2024)**  
A line chart showing run trends across seasons, helping visualize performance patterns and year-to-year consistency.


## 🎯 Step 3 — Bowling Performance Analysis

Key bowling metrics calculated:

- Wickets taken
- Balls bowled
- Overs
- Economy rate
- Bowling strike rate
- Match consistency
  
### 🔍 Insight:
Allows comparison of control (economy) vs impact (wickets).

### 📊 Visualization:
**Bowler Efficiency — Wickets vs Economy**
Clear scatter plot with non-overlapping legend to show separation between strike bowlers and economical bowlers.

## 🔁 Step 4 — All-Rounder Analysis

All-rounders were evaluated using both batting and bowling contributions:

- Runs
- Strike rate
- Wickets
- Economy
- Match impact score
  
### 🔍 Insight:
Shows which players offer true dual-department value — essential for team balance.

## 🔢 Step 5 — Normalization & Scoring (Unique Approach)

Instead of raw stats, a balanced and fair scoring system was used.

✔ Normalized Features:
- Runs (0–1)
- Strike Rate (0–1)
- Wickets (0–1)
- Inverse Economy (1/economy → better for lower economy)

✔ Role-Specific Scoring:
**Batsman Score = 60% Runs + 40% Strike Rate**
**Bowler Score = 70% Wickets + 30% Economy Impact**
**All-Rounder Score = Balanced combo from both**

This ensures players are judged based on their role, not unfair comparisons.

## ⭐ Step 6 — Consistency Score (Your Unique Idea)
A special score was added to reward players who performed across multiple seasons.
`Consistency = Number of seasons played (2021–2024)`

### 🔍 Insight:
Consistent performers are more valuable in a franchise system than one-season spikes.

## 🧮 Step 7 — Final Score (Weighted Approach)
To combine all factors:
`Final Score = 0.85 × Performance Score  + 0.15 × Consistency Score`

This maintains:

- Strong weight on actual performance
- Bonus for multi-season reliability

## 🛠 Step 8 — Team Building Logic (Balanced XI)

The final Franchise XI follows a real cricket team structure:

- 4 Batsmen
- 2 All-Rounders
- 4 Bowlers
- 1 Additional Best Player (based on final score)
  
This ensures:

- ✔ Depth in batting
- ✔ Strong bowling attack
- ✔ Versatility through all-rounders
- ✔ No overloading of any role

This approach is unique, logical, and easy to justify.

## 🏆 Final Output — Best IPL Franchise XI (2021–2024)

The notebook outputs:

- Player name
- Role
- Final score
- Main stats (Runs, Wickets, SR, Economy)
- Season participation details
  
Plus a bar chart visualization of final player scores.

## 📊 Final Visualizations Included in Notebook

These charts make the analysis clear and visually strong:

1. Top Batsmen Trend (Line Plot)
2. Bowler Efficiency Chart (Scatter Plot)
3. All-Rounders Performance (Scatter Plot)
4. Final Team Score Plot (Bar Chart)
5. Team Role Distribution (Pie Chart)

Each chart includes clean styling and legends placed outside the graph.

## 🔧 Technologies Used

- Python
- Jupyter Notebook
- pandas
- numpy
- seaborn
- matplotlib

## 📝 Interpretation & Key Insights

- Data across multiple seasons gives much better reliability than single-year stats.
- Normalization allows fair comparison across roles.
- Consistency helps identify real franchise value players.
- Balanced team structure is crucial for making a practical XI.
- Visuals reveal performance patterns not visible in raw tables.
- Unique scoring formula makes the final team selection unbiased and replicable.

