# Seasonal Agriculture Performance Analysis

This project analyzes agricultural data across **Kharif, Rabi and Zaid** seasons. The main aim is to understand how yield, water use, irrigation, environmental conditions and economic performance change between seasons.

## Problem Statement

Agricultural performance can change with season because of environmental conditions, farming practices, resource availability and market conditions. This project uses data analysis to identify useful seasonal patterns, differences and relationships in the available agricultural data.

## Objectives

- Understand the agricultural dataset
- Clean and prepare the data
- Compare performance across seasons
- Study crop and irrigation differences
- Examine environmental and resource relationships
- Analyze profitability and water efficiency
- Identify unusual patterns and useful insights
- Give practical recommendations based on the results

## Dataset

The dataset contains **4,000 records and 28 columns** covering:

- State and District
- Crop and Season
- Farm area
- Rainfall, temperature, humidity and sunlight
- Soil conditions and nutrients
- Irrigation and fertilizer usage
- Seed quality and pesticide usage
- Yield and production
- Market price, cost, revenue and profit
- Water use and water efficiency
- Disease/pest risk

## Data Cleaning

The raw dataset had 120 missing cells:

- Rainfall: 48
- Soil moisture: 40
- Yield: 32

No duplicate rows were found. Numerical missing values were filled using the median, and categorical missing values were filled using the mode. Infinite values were also checked during preparation.

## Main Results

### Seasonal performance

| Season | Avg. Yield (t/ha) | Avg. Profit (₹) | Avg. Water Use (m³) | Water Efficiency | Pest Risk |
|---|---:|---:|---:|---:|---:|
| Kharif | 5.63 | 178,914.65 | 6,102.20 | 5.89 | 54.47% |
| Rabi | 5.04 | 87,689.47 | 5,846.99 | 5.19 | 40.48% |
| Zaid | 4.64 | -24,804.82 | 6,419.89 | 4.41 | 38.22% |

### Crop profitability

- Sugarcane: average profit **₹817,187.99**
- Chilli: average profit **₹750,878.34**
- Rice, Wheat and Maize had negative average profit in the analyzed data.

### Irrigation

Drip irrigation had the highest average yield (**6.58 t/ha**) and average profit (**₹219,626**) among the irrigation methods.

### Correlation results

- Water efficiency vs yield: **0.913**
- Revenue vs profit: **0.887**
- Production vs yield: **0.883**
- Water efficiency vs profit: **0.489**
- Yield vs profit: **0.488**
- Fertilizer vs yield: **0.000**
- Seed quality vs yield: **-0.007**

Correlation represents association, not causation.

## Tools Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook / Google Colab
- Git and GitHub

## Project Files

```text
Seasonal-Agriculture-Performance-Analysis/
├── Seasonal_Agriculture_Performance_Analysis.ipynb
├── seasonal_agriculture_performance_dataset.csv
├── final_cleaned_agriculture_dataset.csv
├── seasonal_summary.csv
├── README.md
├── insights.txt
└── PPT/
    └── Seasonal_Agriculture_Performance_Analysis.pptx
```

## How to Run

1. Open `Seasonal_Agriculture_Performance_Analysis.ipynb` in Google Colab or Jupyter Notebook.
2. Upload `seasonal_agriculture_performance_dataset.csv`.
3. Run the cells from top to bottom.
4. The notebook performs cleaning, analysis and visualization.

## Conclusion

The analysis shows that seasonal conditions are associated with noticeable differences in agricultural performance. Kharif showed the strongest overall performance, while Zaid needs more attention because of its lower yield, lower water efficiency and negative average profit. Crop choice and irrigation method also showed important differences in the dataset.

This project is intended as a data analysis study based on the supplied dataset. The findings should be treated as observations from the dataset rather than universal agricultural rules.
