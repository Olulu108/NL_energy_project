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

### Q3: How does household size affect energy usage per person?

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q3_hhsize.png) 

By analyzing both electricity and gas usage per person, the plot shows that larger households are more energy-efficient. In contrast, smaller households, such as those with one or two members, tend to consume more energy per individual.

---

### Q4: Are newer homes (post-2000) more energy-efficient?

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q4_before2k.png) 

This graph illustrates the relationship between the percentage of houses built before 2000 and average energy consumption per house, based on data from all municipalities in the Netherlands over the period filtered for the years 2014–2022 for this analysis. Both electricity and gas consumption increase as the share of older buildings rises.

====================================================================================================================

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q4_before2k22.png) 

This graph shows the relationship between the percentage of houses built before 2000 and the average energy consumption per house for all Dutch municipalities in 2022. Electricity consumption slightly decreased (−7 kWh) and gas consumption increased (+8 m³) for every 1% rise in the share of houses built before 2000. These opposing trends highlight how different energy sources respond to housing age, emphasizing the continued dependence of older homes on gas infrastructure

====================================================================================================================

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q4_after2k.png) 


====================================================================================================================

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q4_before2kDH.png) 



====================================================================================================================

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q4_before2kDH22.png) 

---

### Q5: Do densely populated neighborhoods have different energy consumption patterns than sparse ones?

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q5_bev_dich_DH.png) 

In The Hague, neighborhoods with higher population density tend to have lower average household energy consumption. This inverse relationship is consistent for both electricity and gas usage. The trend suggests that denser areas—often associated with smaller dwellings and shared infrastructure—are generally more energy-efficient on a per-household basis.

---

### Q6: Are more expensive homes (woz) also more energy efficient?

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q6_woz_DH22.png) 

In The Hague (2022), neighborhoods with higher average house values also exhibit higher average energy consumption per household. Both electricity and gas usage increase with property value, as shown by positive linear trends. This suggests that more expensive homes—likely larger and with more appliances or heating demands—consume more energy overall

---

### Q7: How does average income influence energy consumption?

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q7_ink_DH.png) 

In The Hague, neighborhoods with higher average income per income recipient tend to have higher household energy consumption. This positive relationship holds for both electricity and gas usage. Linear trend lines indicate that as income increases, energy consumption rises—suggesting that wealthier households, likely living in larger homes or with more energy-intensive lifestyles, consume more energy on average.

![image_url](https://github.com/Olulu108/NL_energy_project/blob/main/graphs/Q7_ink_DH22.png) 

---

## Tools Used

- Python, Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn (for regression & forecasting)

---

## Conclusion

This project reveals clear trends in Dutch energy consumption:
- Smaller homes, newer constructions, and denser neighborhoods are typically more energy-efficient.
- Wealth and property value correlate with *higher*, not lower, energy use — possibly due to home size and lifestyle.

---

## Future Work

- Incorporate geographic mapping (e.g., GeoPandas or Folium)
- Use clustering to segment neighborhood types
- Extend forecasting to electricity usage
- Compare The Hague with other Dutch cities

---

## Author

Created by **[Olga Pershina]**

Data: © [CBS (Centraal Bureau voor de Statistiek)](https://www.cbs.nl)  
For questions, suggestions, or contributions, feel free to open an issue or fork the project!





