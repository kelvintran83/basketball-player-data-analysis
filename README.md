# Predicting Height of Basketball Players Data

This project is an introductory exploration of data analytics and statistical modeling in the context of international basketball player data. Using Python and Jupyter Notebook, the objective is to predict the height of professional basketball players. The project involves data preparation, exploration, statistical modeling, and performance evaluation.

## Overview

### Data Source
The dataset used in this project is sourced from Kaggle and contains basketball player stats from 1999 to 2020, spanning 49 international leagues. The dataset includes 53,798 instances of data and 30 independent features, with the target variable being the height of the players.

[Link to the Dataset](https://www.kaggle.com/jacobbaruch/basketball-players-stats-per-season-49-leagues)

### Project Objective
The primary goal of this project is to analyze the distribution of basketball players' heights and investigate their relationship with other variables. This analysis involves exploring the distribution, variance, and predictability of height using regression models and obtaining a reduced model. Additionally, the predictability of height is assessed through R-squared values and p-values.

### Descriptive Features
The dataset includes various features, such as:
- Stage: Nominal variable representing the stage of the season (International, Playoffs, Regular Season)
- MIN: Continuous variable indicating the total minutes played
- TOV: Continuous variable for total turnovers
- REB: Continuous variable for total rebounds
- AST: Continuous variable for total assists
- STL: Continuous variable for total steals
- BLK: Continuous variable for total blocks
- PTS: Continuous variable for total points
- height_cm: Continuous variable for player height in centimeters
- weight_kg: Continuous variable for player weight in kilograms

```python
import numpy as np
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns
import statsmodels.api as sm
import statsmodels.formula.api as smf
import patsy
from IPython.display import display, HTML