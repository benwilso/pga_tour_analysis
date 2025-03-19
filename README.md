**PGA Tour Player Performance Analysis**

**Project Overview**
This project analyzes PGA Tour player performance between 2015 and 2019 using historical data. The goal is to examine player trends, identify key performance drivers, and uncover relationships between strokes gained statistics and player rankings.

**Data Sources**
The analysis leverages two datasets:

PGA Tour Data (2015 - 2022)
Contains tournament details (name, date, location), player performance metrics, and strokes gained measures.
Source: Kaggle - PGA Tour Golf Data
Format: CSV
Records: 36,865 entries (497 players)
Official World Golf Ranking (OWGR)
Includes weekly world rankings of the top 300 players from 1997 to 2021.
Source: Kaggle - Official World Golf Ranking
Format: CSV
Records: 314,783 entries (1,467 players)

**Key Objectives**
Identify players with the largest performance increases and decreases between 2015 and 2019.
Determine the most consistently high-performing players.
Compare strokes gained by elite players vs. average players.
Analyze correlations between strokes gained statistics.

**Data Processing & Cleaning**
Imported both datasets and converted them into Pandas DataFrames.
Standardized column names and formats.
Filtered data to focus on the 2015-2019 period.
Merged datasets on player name and week-year for analysis.
Created new features, including:
Strokes to Par for individual tournament performance.
World Ranking Bins (grouped in increments of 10).
Year-Week format for proper merging.

**Analysis & Visualizations**
Player Performance Trends: Used histograms and line charts to track ranking changes.
Strokes Gained Comparison: Compared elite players vs. lower-ranked players using stacked bar charts and scatter plots.
Tournament Participation Trends: Visualized player participation rates over seasons.
Strokes Gained Correlations: Explored relationships between different strokes gained statistics.

**Findings**
Jon Rahm, Bryson DeChambeau, Tiger Woods, Xander Schauffele, and Patrick Cantlay showed the largest ranking improvements.
Elite players (Top 50) consistently gained more strokes per round, mainly due to superior off-the-tee and approach play.
Strokes Gained Off the Tee and Strokes Gained Approach exhibited a strong positive correlation.
Consistency in performance was more crucial for rankings than occasional high finishes.

**Project Structure**
bash
Copy
Edit
pga_tour_analysis/
│── data/                      # Data files (not included in the repo)
│── notebooks/                 # Jupyter notebooks for analysis
│── scripts/                   # Python scripts for automation
│── visualizations/            # Generated charts and figures
│── 13_psklam_jado_benwilso_2025winter.py   # Main analysis script
│── README.md                  # Project documentation

**Running the Project**
Prerequisites

Ensure you have Python 3.7+ installed and the following packages:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn
Execution

Clone the repository:
bash
Copy
Edit
git clone https://github.com/benwilso/pga_tour_analysis.git
cd pga_tour_analysis
Run the main analysis script:
bash
Copy
Edit
python scripts/13_psklam_jado_benwilso_2025winter.py
View generated visualizations in the visualizations/ folder.

**Contributors**
Ben Wilson – Data cleaning, visualization, and strokes gained analysis.
Peter Sklamberg – Data merging, visualization, and presentation structure.
James Doherty – Data import, preprocessing, and analysis contributions.

**Future Work**
Extend the analysis to 2022 data.
Implement machine learning models for ranking predictions.
Explore additional factors influencing player performance.
