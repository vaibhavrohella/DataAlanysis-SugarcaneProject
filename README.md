# Sugarcane Production Analysis 🌾
A comprehensive exploratory data analysis (EDA) project examining global sugarcane production patterns across different countries and continents. This project provides insights into production volumes, land usage, yield efficiency, and per capita production metrics.
## 📊 Project Overview
This project analyzes global sugarcane production data to answer key questions about:

Which countries are the largest sugarcane producers 

How production efficiency varies across regions

The relationship between land area and total production


Continental patterns in sugarcane cultivation

Per capita production distributions

## 🗂️ Dataset
The analysis uses data from the "List of Countries by Sugarcane Production" dataset, which includes:
Features:

Country: Name of the country

Continent: Continental classification

Production (Tons): Total sugarcane production in tons

Production per Person (Kg): Per capita production in kilograms

Acreage (Hectare): Land area dedicated to sugarcane cultivation

Yield (Kg/Hectare): Production efficiency per hectare

Data Source: GeeksforGeeks EDA Sugarcane Project

## 🛠️ Installation & Setup
### Prerequisites
bashPython 3.7+

Required Libraries

bashpip install pandas seaborn matplotlib

Running the Analysis

### Clone this repository:

bashgit clone https://github.com/yourusername/sugarcane-production-analysis.git

cd sugarcane-production-analysis

### Run the Python script:

bashpython sugarcaneproject.py

Or execute the Jupyter notebook if you prefer an interactive environment.

## 📈 Analysis Components
### 1. Data Cleaning & Preprocessing

Removal of formatting characters (dots, commas) from numerical columns

Data type conversions for proper numerical analysis

Handling missing values

Column renaming for consistency

### 2. Univariate Analysis

Continental Distribution: Number of sugarcane-producing countries per continent

Distribution Analysis: Statistical distributions of production metrics

Outlier Detection: Box plots identifying unusual production patterns

### 3. Bivariate Analysis

Top Producers: Countries with highest total production

Land Usage: Countries with largest cultivation areas

Efficiency Leaders: Highest yield per hectare countries

Per Capita Leaders: Highest production per person

### 4. Correlation Analysis

Relationship between land area and total production

Yield efficiency vs. total production correlation

Cross-variable correlation heatmap

### 5. Continental Analysis

Production distribution across continents

Impact of country count on continental production

Land area vs. production relationships by continent

## 🔍 Key Findings
The analysis reveals several important insights:

Production Leaders: Identifies the top sugarcane-producing countries globally

Efficiency Patterns: Countries with smaller land areas can achieve high production through better yield efficiency

Continental Trends: Shows which continents dominate global sugarcane production

Resource Utilization: Correlation between land usage and production outcomes

## 📊 Visualizations
The project generates multiple visualization types:

Bar charts for categorical comparisons

Distribution plots for numerical variables

Box plots for outlier analysis

Scatter plots for correlation analysis

Pie charts for percentage distributions

Heatmaps for correlation matrices

Line plots for trend analysis

## 🚀 Usage Examples
Basic Analysis

pythonimport pandas as pd

import seaborn as sns

from matplotlib import pyplot as plt

# Load and clean data
url = 'https://raw.githubusercontent.com/GeeksforgeeksDS/EDA-Sugarcane-Project/refs/heads/main/List%20of%20Countries%20by%20Sugarcane%20Production.csv'

df = pd.read_csv(url)

# View top producers
top_producers = df.nlargest(10, 'Production(Tons)')

print(top_producers[['Country', 'Production(Tons)']])

Custom Visualizations

python# Create custom production analysis

plt.figure(figsize=(12, 6))

sns.barplot(data=df.head(10), x='Country', y='Production(Tons)')

plt.xticks(rotation=45)

plt.title('Top 10 Sugarcane Producing Countries')

plt.show()

## 📁 Project Structure
sugarcane-production-analysis/
│
├── sugarcaneproject.ipynb          # Main analysis script
├── README.md                    # This file
├── requirements.txt             # Python dependencies
└── results/                     # Generated plots and analysis results
    ├── production_analysis.png
    ├── continental_distribution.png
    └── correlation_heatmap.png
## 🤝 Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

Fork the repository

Create a feature branch (git checkout -b feature/AmazingFeature)

Commit your changes (git commit -m 'Add some AmazingFeature')

Push to the branch (git push origin feature/AmazingFeature)

Open a Pull Request

## 📋 Future Enhancements

 Time series analysis with historical production data
 
 Machine learning models for production prediction
 
 Interactive dashboards using Plotly/Dash
 
 Economic analysis incorporating market prices
 
 Climate impact assessment on production patterns
 
 Export analysis and trade flow visualization

👨‍💻 Author
Vaibhav Rohella - 77vaibhav781@gmail.com
Project Link: https://github.com/vaibhavrohella/sugarcane-production-analysis

🙏 Acknowledgments

Data source: GeeksforGeeks EDA Sugarcane Project
Inspiration from agricultural data analysis community
Python data science libraries: Pandas, Seaborn, Matplotlib


⭐ If you found this project helpful, please give it a star!
📞 Support
If you have any questions or need help with the project, please open an issue or contact the maintainer.

Last updated: June 2025
