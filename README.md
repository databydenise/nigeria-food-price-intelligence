# 🇳🇬 Nigerian Food Price Inflation & Exchange Rate Analysis #

## Project Overview ##
This project investigates the relationship between food prices in Nigeria and major macroeconomic indicators, particularly the USD/NGN exchange rate and Premium Motor Spirit (PMS) prices.
The goal was to determine whether fluctuations in foreign exchange rates correspond to increases in food prices across Nigeria and whether transportation costs (represented by PMS prices) have a measurable influence on selected food commodities.
The analysis uses official monthly food price reports published by the National Bureau of Statistics (NBS), covering all 36 states.

## Motivation ##
Many studies investigate inflation using consumer price indices, but fewer explore the behaviour of individual food commodities.
Initially, the project was intended to collect live market prices through web scraping. However, because reliable nationwide food price data is not consistently available online—and waiting months to accumulate enough observations was impractical—the project instead used official NBS datasets, providing standardized nationwide monthly observations.

## Objectives ##
- Analyse monthly food price trends across Nigeria.
- Measure correlation between food prices and USD/NGN exchange rates.
- Explore whether PMS prices explain variation in selected food prices.
- Identify commodities most sensitive to macroeconomic changes.
- Compare state-level price differences.
- Identify states with the highest and lowest prices for selected foods.

## Dataset ##

### Data Sources ###

- National Bureau of Statistics (NBS) Monthly Selected Food Price Watch
- Historical USD/NGN Exchange Rates
- Historical PMS (Petrol) Prices

### Coverage ###

- Nigeria
- All 36 states
- Multiple food commodities
- Monthly observations
- Data Cleaning

The raw NBS reports required extensive preprocessing.

Cleaning steps included:

- Extracting Excel files from compressed archives.
- Standardising inconsistent column names.
- Removing repeated header rows.
- Handling missing values.
- Cleaning inconsistent food naming conventions.
- Converting prices to numeric values.
- Combining monthly reports into a single analytical dataset.
- Reshaping data into a format suitable for analysis.

### Analysis Performed ###
- Exploratory Data Analysis (EDA)
- Time-series trend analysis
- Correlation analysis
- State-by-state price comparisons
- Highest and lowest price identification
- Exchange rate vs food price analysis
- PMS vs food price analysis

## Key Findings ##

- Prepacked wheat flour exhibited the strongest positive correlation with the USD/NGN exchange rate, followed by white garri, yellow garri, rice, beans, and a crate of eggs (30 pieces).
- Several staple foods increased in price alongside exchange rate depreciation, suggesting that exchange rate movements may influence food prices through import costs, production inputs, or broader inflationary pressures.
- Premium Motor Spirit (PMS) prices explained part of the variation in transportation-dependent foods. However, some commodities that were expected to have a strong positive relationship with PMS—particularly those showing weaker or negative relationships with the exchange rate—did not exhibit strong correlations with PMS prices.
- This suggests that transportation costs alone do not fully explain food price movements and that other domestic factors, such as seasonality, local supply conditions, production costs, and regional market dynamics, likely play important roles.
- Significant price differences were observed across Nigerian states, highlighting regional disparities in food markets.

## Technologies ##
- Python
- Pandas
- NumPy
- Matplotlib
- Jupyter Notebook

Repository Structure Coome back
data/
notebooks/
cleaned_data/
figures/
README.md
requirements.txt

## Future Work ##
1. Extend the dataset with additional years.
2. Incorporate inflation and CPI data.
3. Build forecasting models.
4. Develop an interactive dashboard.
5. Investigate lag effects between exchange rate movements and food prices.

## Author ##

Denise Moemeke
Data Scientist | Aspiring Data Engineer
