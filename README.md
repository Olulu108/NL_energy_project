# Analysing energy consumption trends in the Netherlands

## Project Overview

This data analysis project explores energy consumption patterns in the Netherlands, with a special focus on The Hague (`'s-Gravenhage`). Using open data from 2004–2024, it investigates how factors like housing type, construction year, household size, population density, and income influence electricity and gas usage.

## Data Source

Data used in this project comes from the [Centraal Bureau voor de Statistiek (CBS)](https://www.cbs.nl/nl-nl/reeksen/publicatie/kerncijfers-wijken-en-buurten), the national statistical office of the Netherlands. Specifically, the "Kerncijfers wijken en buurten" dataset was used, which includes neighborhood-level indicators such as population, housing, income, and energy use.

## Project Objectives

To analyze and visualize:

- National trends in household energy use
- Energy efficiency across different housing types
- The impact of household characteristics and neighborhood demographics on energy consumption
- Forecasts for future energy trends
  
## Research Questions 

### Q1: How has average energy consumption (electricity and gas) changed from 2004–2024?

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q1_test.png) 

The plot illustrates the national average household consumption of electricity and gas in the Netherlands from 2004 to 2023. Both electricity and gas consumption show a downward trend over time.

---

### Q2: Which residential house types are more energy efficient?

#### Electricity consumption per differen house type
![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q2el_test.png) 
This visualization shows the average electricity consumption by housing type in the Netherlands from 2004 to 2023. All housing types exhibit a clear downward trend, with negative slopes indicating consistent reductions in electricity use over time. Detached houses remain the highest consumers, while apartments consume the least on average. However, apartments are also improving the slowest: their electricity use is decreasing by only about 16 kWh per year, compared to 43–44 kWh per year for rowhouses and corner houses. This suggests that while all housing types are becoming more energy efficient, larger improvements are occurring in low- and mid-density housing types.

#### Gas consumption per differen house type
![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q2gas_test.png) 
Between 2004 and 2023, all housing types in the Netherlands showed a clear downward trend in average gas consumption, with negative slopes across the board. Detached houses consumed the most gas overall but also achieved the steepest reduction—about −68 m³ per year—indicating significant efficiency gains. Apartments, while consistently the lowest consumers, saw the slowest progress, with only −27 m³ per year. Other housing types (rowhouses, corner houses, semi-detached homes) fall in between, with steady but less dramatic decreases

#### Trend analysis of gas consumption
![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q2trend_test.png) 
This code forecasts average gas consumption by housing type in the Netherlands through 2035, using linear regression models trained on data from 2015–2023 (with 2021 interpolated). It includes five residential types: apartments, rowhouses, corner houses, semi-detached, and detached homes. The model fits historical trends for each housing type and extends them into the future.

The forecast shows that although all housing types are reducing gas consumption, detached houses—historically the highest consumers—are declining at the fastest rate. Based on this trend, detached homes could approach the consumption levels of other types by around 2035.

However, this convergence is theoretical. In practice, differences in size, insulation, and heating needs mean that complete equalization is unlikely to occur, even if the trajectories suggest otherwis


---
