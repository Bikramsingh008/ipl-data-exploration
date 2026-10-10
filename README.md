# IPL Match Data Exploration

Exploratory data analysis of IPL (Indian Premier League) match data from 2008-2024, using Python, Pandas, NumPy, and Matplotlib.

## Dataset
1095 matches, 20 columns including: team1, team2, winner, toss_winner, toss_decision, venue, season, player_of_match, result_margin.

Source: [Kaggle - IPL Complete Dataset](https://www.kaggle.com/datasets)

## Tools Used
- **Pandas** – loading, cleaning, and analyzing match data
- **NumPy** – numerical calculations
- **Matplotlib** – data visualization

## What I Did
- Loaded and inspected the dataset (`.shape`, `.info()`, `.isnull().sum()`)
- Found total wins per team using `value_counts()`
- Created a derived column to test whether winning the toss predicts winning the match
- Analyzed toss decisions (bat vs field), top venues, and top Player of the Match winners
- Visualized findings with bar charts, including handling readability for many categories using `figsize`

## Key Findings
- **Mumbai Indians** are the most successful team with **143 wins**, followed by Chennai Super Kings (138) and Kolkata Knight Riders (131).
- Winning the toss does **not** reliably predict winning the match — toss winners won only **554 out of 1095** matches (about **50.6%**), essentially a coin flip.
- Teams overwhelmingly prefer to **field first** after winning the toss (704 times) over batting first (391 times), reflecting the modern T20 trend of chasing targets.
- **Eden Gardens** is the most-used venue (77 matches), followed by Wankhede Stadium (73).
- **AB de Villiers** has won the most Player of the Match awards (25), followed by Chris Gayle (22) and Rohit Sharma (19).

## What I Learned
- Analyzing categorical data using `value_counts()` and `groupby()`
- Creating a derived/calculated column to test a hypothesis (toss winner vs match winner)
- Using `figsize` to make charts with many categories readable
- Applying the same Pandas/NumPy/Matplotlib workflow to a second, different dataset to build confidence

## Files
- `ipl_eda.ipynb` – full notebook with code, outputs, and analysis
