# IPL Data Analysis (2008–2025)

This project explores IPL data from 2008 to 2025 using Python.  
The dataset contains ball-by-ball information, which is cleaned and transformed to study team performance, batting trends, scoring patterns, and venue behaviour.  
The goal of the project is to understand how teams and players have performed over the years and how the game has evolved.

---

## Project Structure
```
ipl-eda/
│── data/
│ ├── IPL.csv                                  # raw dataset
│ ├── ipl_cleaned_final.csv                    # cleaned ball-by-ball data
│ ├── matches_one_row.csv                      # match-level table
│ ├── batter_stats.csv                         # batter stats
│── images/                                    # generated plots
│── notebooks/
│ ├── IPL_EDA.ipynb                            # main analysis notebook
│── requirements.txt
│── README.md

```
---

## Data Processing

The raw CSV file needed cleaning and normalization.  
The following steps were carried out:

- Standardized column names  
- Converted date and season formats  
- Added helper features:
  - `over_number`
  - `is_boundary`
  - `is_wicket`
  - `valid_ball`
- Fixed team names  
- Created a one-row-per-match table  
- Built batter-level summaries using `runs_batter` and `valid_ball`  
- Saved cleaned datasets for reuse

---

## Team Analysis

The team section looks at:

- Total wins  
- Season-wise wins  
- Win percentage  
- Basic trends across seasons  

Generated plots include:

- Wins by team  
- Season-wise wins heatmap  
- Win percentage comparison  

These give a clear view of which teams have been the most consistent across seasons.

---

## Batting Analysis

Batting performance is calculated using true per-ball values from the dataset.  
The analysis includes:

- Top run scorers  
- Strike rate (minimum ball threshold)  
- Boundary count  
- Boundary percentage  
- Top scorer for each season  

This helps highlight long-term consistent batters as well as aggressive players.

---

## Runs per Over (Match Phases)

Runs are also analyzed by match phases:

- Powerplay (1–6)
- Middle overs (7–15)
- Death overs (16–20)

This section shows how scoring patterns differ by phase and how they have changed over the years.

---

## Venue Analysis

The venue section includes:

- Number of matches at each ground  
- Average innings runs by venue  
- Basic comparison of high-scoring and low-scoring venues  

This helps identify stadiums that favour batting or bowling.

---

## How to Run

Clone the repository and install dependencies.

```bash
git clone https://github.com/krishakapadia/ipl-eda
cd ipl-eda
pip install -r requirements.txt

```

Launch the notebook:
```
jupyter notebook
```

Open: 
```
notebooks/IPL_EDA.ipynb
```


Run all cells top to bottom inside the notebook.

## Summary

The project covers the main areas of IPL analysis:

- Team performance over 18+ seasons

- Batting trends and season leaders

- Scoring patterns across match phases

- Venue behaviour

- Clean feature engineering and organized workflow

It can be extended further by adding bowling analysis, player clusters, or prediction models if needed.


# Author

Krisha Kapadia

