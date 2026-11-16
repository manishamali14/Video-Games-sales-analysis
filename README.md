# Video Game Sales Analysis

An exploratory data analysis of video game sales to find out which platforms, genres, games and regions sold the most, and how sales changed over the years.

## Dataset

The data comes from the Video Game Sales dataset on Kaggle (vgsales.csv). It has 16,598 games with at least 0.01 million copies sold.

Columns: Rank, Name, Platform, Year, Genre, Publisher, NA_Sales, EU_Sales, JP_Sales, Other_Sales, Global_Sales. All sales are in millions of units.

## Tools

Python, Pandas, NumPy, Matplotlib, Seaborn

## Data Cleaning

1. Removed extra spaces from column names and text columns.
2. Filled 58 missing Publisher values with "Unknown".
3. Kept 271 missing Year values as NA instead of guessing them.
4. Checked for exact duplicate rows. None were found.
5. Corrected one wrong release year (2020 changed to 2009).
6. Checked for negative sales and confirmed regional sales add up to global sales.

Outliers were kept because they are real best sellers, not errors.

## Key Findings

1. PS2 is the best selling platform with 1,255.64 million units.
2. Action is the top genre (1,751.18 million), followed by Sports and Shooter.
3. Wii Sports is the best selling game at 82.74 million units, and all of the top 10 games are Nintendo titles.
4. North America is the biggest market with about 49% of total sales.
5. Sales peaked in 2008 at 678.9 million units and declined after that.
6. Global sales are most closely linked to North America (0.94) and Europe (0.90) sales.

## Limitations

The data only goes up to 2016, 271 games have no release year, and the sales figures cover physical copies only.

## How to Run

Open the notebook in Jupyter or Kaggle, make sure vgsales.csv is available and update the file path if needed, then run all cells from the top.
