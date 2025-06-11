# Correlations in Sorare: Premier League 2024–2025 Analysis
An analysis of correlations between positions in Sorare using Premier League 2024–2025 data

## Overview

This repository contains an analysis of correlations between positions within the same team to analyse stacking strategies in Sorare, by using Premier League data from January 2024 to June 2025. In Sorare—an online fantasy football game—stacking (using multiple players from the same team) is a popular tactic believed to increase performance due to shared match conditions like weak opponents.

But does stacking actually help?

## Goal of the Analysis

If stacking is effective, we should observe strong correlations in player scores between teammates. In this analysis, I examine the correlations in Sorare scores across positions (goalkeepers, defenders, midfielders, and forwards) to see how much synergy actually exists within teams.

### Data Source

- All Sorare player scores were collected via the [Sorare API](https://github.com/sorare/api).
- Only Premier League players from Jan 2024 to Jun 2025 were included.
- Players were filtered to only include those who played at least 60 minutes.

## Key Findings

- **Defender–Goalkeeper pairs** show the strongest positive correlation — logical due to shared clean sheet potential.
- **Midfielder–Defender pairs** have weak but positive correlations, mostly driven by all-around (AA) scores.
- **Forwards** have little to no correlation with any other position, including their own goalkeeper or defender.
- Stacking should be done strategically: don’t assume a good fixture means all your players will perform well.

## How to Run This Notebook

To replicate this analysis:

### 1. Clone this repository:
   ```bash
   git clone https://github.com/WilliamLuiten/sorare-correlation-analysis.git
   ```
### 2. Install required packages:

pip install -r requirements.txt

### 3. Open and run the Jupyter notebook:

jupyter notebook "Sorare Premier League correlations.ipynb"

⚠️ Note: You need a Sorare account to access data via the API. Instructions for using the API can be found here [Sorare API](https://github.com/sorare/api).
You also need to fill in your credentials in the Sorare Premier League correlations.ipynb file.

## Repository Structure
.                 
├── notebooks/
│   └── Sorare Premier League correlations.ipynb
├── requirements.txt
├── README.md
└── .gitignore

## License
This project is licensed under the MIT License. See LICENSE for details.

