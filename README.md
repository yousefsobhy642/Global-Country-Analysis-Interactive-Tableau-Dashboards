# Global Country Analysis: Interactive Tableau Dashboards

Interactive Tableau dashboards analyzing demographic, health (HIV)
and economic indicators across 200+ countries, built with
parameters, calculated fields, dashboard actions and a Tableau Story.

**Live dashboards:** [Tableau Public link here]

## Dashboards and Findings

### 1. Global Demographics Overview
![Dashboard 1](images/dashboard1_demographics.png)

- **Lower-income countries lead on births and infant mortality.**
  Most countries with high birth rate, fertility rate and infant
  mortality have GDP per capita below 10,000. This suggests
  population growth and child-health needs are concentrated in
  lower-income countries.
- **Africa stands out geographically.** The map shows the highest
  birth rates clustered in Africa.
- **Births and infant mortality move together.** Countries with
  higher birth rates tend to have higher infant mortality,
  pointing to limited healthcare access in the same places.
- **Wealthier countries tend to have fewer children per woman.**
- **Density is dominated by small territories.** Ranking by
  population density favors small countries, so it is a poor
  basis for comparing large nations.

### 2. HIV & Health Indicators
![Dashboard 2](images/dashboard2_hiv_health.png)

- **HIV is concentrated, not universal.** 22 countries have adult
  prevalence of 5% or more, and 21 of them are in the Poor income
  group. Most Poor-group countries still have prevalence below
  1%, so income alone does not explain the spread.
- **Deaths follow the same pattern.** Most of the countries with
  the highest HIV/AIDS deaths are in Africa.
- **Wealthier countries stay low.** Among countries with HIV
  data, prevalence in the Rich and Very Rich groups stays below
  1%.
- **Life expectancy gaps are wide.** Rich countries mostly exceed
  60 years, while many lower-income countries fall below 60. Lower-income
  countries also vary widely, from the 30s to about 80, so
  income does not fully determine life expectancy.

### 3. Global Economy & Growth
![Dashboard 3](images/dashboard3_economy.png)

- **Size is not living standard.** China's GDP is about 7.3
  trillion, yet its GDP per capita (5,600) is far below the US
  (40,100). Per-capita figures are better for assessing markets.
- **Growth is weakly linked to wealth.** Growth rates cluster
  between roughly 0% and 10% at almost every income level.
- **Investment is a weak predictor.** Countries with similar
  investment levels show very different growth rates.
- **Industry can outpace the economy.** Among the countries with
  the widest gaps, industrial output grows much faster than
  overall GDP.
- **Small, lower-income economies dominate** the dataset, and most
  of them grow at moderate or fast rates. Large economies are rare.
- **Trade is imbalanced.** Among the 15 largest economies, the US
  deficit (about 690 billion) is several times larger than the
  biggest surplus (Germany, about 175 billion).

## Tools and Techniques

Tableau, Python (data collection and cleaning), calculated
fields, parameters, dashboard actions (filter, highlight,
navigation), Tableau Story, maps, treemap, heat maps, scatter
plots with trend lines, box plot, pie chart, dumbbell chart.

## Data

Country-level indicators (CIA World Factbook style): 264 rows,
45 columns covering demographics, health, economy, energy and
infrastructure. Cleaning in Python: removed the extra data-type
row, converted text columns to numbers, and excluded non-country
entities such as European Union.

## Limitations

- The data is cross-sectional with no reference year, so figures
  are a single snapshot and may differ from current values.
- Findings show associations, not causes.
- Many columns have missing values. Countries with missing data
  are excluded from the relevant charts.

## Repository Structure

```
├── README.md
├── data/        # source and cleaned CSV files
├── workbook/    # MiniProject_tableau.twbx (data included)
├── scripts/     # Python data collection and cleaning
└── images/      # dashboard screenshots
```

## How to Open

Download `workbook/MiniProject_tableau.twbx` and open it with
Tableau Desktop or the free Tableau Reader. The data is packaged
inside the file.
