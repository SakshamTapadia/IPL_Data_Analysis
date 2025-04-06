# IPL Dataset Analysis

![IPL Teams](https://raw.githubusercontent.com/genieincodebottle/generative-ai/main/images/ipl-image.png)

A comprehensive analysis of Indian Premier League (IPL) data using `matches.csv` and `deliveries.csv`. This project includes data preprocessing, exploratory data analysis (EDA), feature engineering, and preparation for predictive modeling.

## Features

- **Data Ingestion**: Load and inspect IPL match and delivery data.
- **Data Cleaning**: Handle missing values, correct data types, and standardize team names.
- **Exploratory Data Analysis (EDA)**:
  - Match distribution across seasons.
  - Team performance analysis (most successful teams).
  - Toss decision impact on match outcomes.
  - Venue analysis (most frequent match locations).
  - Player performance (Player of the Match awards).
  - Win margin analysis (runs vs. wickets).
- **Visualizations**: Interactive plots using Plotly and Matplotlib/Seaborn.
- **Feature Engineering**: Derive new features like `win_by_runs`, `win_by_wickets`, and date components.

## Dataset Details

### `matches.csv`
- **Columns**: `id`, `season`, `city`, `date`, `venue`, `team1`, `team2`, `toss_winner`, `toss_decision`, `winner`, `result`, `player_of_match`, and more.
- **Description**: Contains match-level details (2008–2024), including results, venues, and toss decisions.

### `deliveries.csv`
- **Columns**: `match_id`, `inning`, `batting_team`, `bowling_team`, `over`, `ball`, `batter`, `bowler`, `runs`, `wickets`, and more.
- **Description**: Ball-by-ball delivery data for all matches.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/sakshamtapadia/sakshamtapadia-ipl_data_analysis.git
   cd sakshamtapadia-ipl_data_analysis
   ```

2. Install required libraries:
   ```bash
   pip install pandas numpy plotly matplotlib seaborn jupyter
   ```

## Usage

1. Run the Jupyter Notebook:
   ```bash
   jupyter notebook ipl-dataset-analysis.ipynb
   ```

2. Follow the notebook sections:
   - **Data Loading**: Load and inspect datasets.
   - **Data Cleaning**: Handle missing values and inconsistencies.
   - **EDA**: Visualize trends (e.g., team wins, toss impact).
   - **Feature Engineering**: Prepare data for modeling.

## Key Results

- **Most Successful Team**: Mumbai Indians (144 wins).
- **Toss Impact**: Teams winning the toss won ~50.8% of matches. Choosing to field first led to a higher win rate (53.9%).
- **Top Venue**: Eden Gardens hosted the most matches (77).
- **Player of the Match**: AB de Villiers (25 awards).

## Directory Structure

```
sakshamtapadia-ipl_data_analysis/
├── deliveries.csv
├── ipl-dataset-analysis.ipynb
├── matches.csv
└── README.md
```

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments
- Dataset sourced from publicly available IPL records.
- Visualizations powered by Plotly and Matplotlib/Seaborn.
