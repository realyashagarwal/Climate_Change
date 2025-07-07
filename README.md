# CarbonCast: Development's Carbon Cost
**Development's Carbon Cost**

[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org/)
[![scikit-learn](https://img.shields.io/badge/scikit--learn-1.2.2-red.svg)](https://scikit-learn.org/)

## 🌍 Project Overview

CarbonCast is a comprehensive machine learning project that analyzes the relationship between socioeconomic development indicators and CO₂ emissions across nations. By leveraging historical data spanning multiple decades, this project builds predictive models to forecast future carbon emissions trajectories based on economic and social factors.

### Key Features
- **Multi-dimensional Analysis**: Examines correlations between GDP, population, energy consumption, and CO₂ emissions
- **Predictive Modeling**: Implements multiple regression algorithms for accurate forecasting
- **Interactive Visualizations**: Comprehensive exploratory data analysis with matplotlib and seaborn
- **Future Projections**: Generates emission scenarios for policy planning and climate action


## 🔧 Technical Stack

```
Frontend:     Jupyter Notebooks
Backend:      Python 3.8+
ML Libraries: scikit-learn, statsmodels
Visualization: matplotlib, seaborn
Data Processing: pandas, numpy
File Handling: openpyxl
```

## 📂 Repository Structure

```
Climate_Change/
├── 📁 data/
│   ├── 📁 raw/                    # Original datasets
│   │   └── climate_change_download_0.xls
│   └── 📁 processed/              # Cleaned, analysis-ready data
│       └── data_cleaned.csv
├── 📁 notebooks/                  # Jupyter analysis notebooks
│   ├── 1-Data_Preprocessing.ipynb
│   ├── 2-Exploratory_Data_Analysis.ipynb
│   └── 3-Model_Training_and_Future_Forecasting.ipynb
├── 📁 models/                     # Trained ML models
│   └── Trained-Model.pkl
├── requirements.txt               # Python dependencies
├── README.md                      # Project documentation
└── LICENSE                        # MIT License
```

## 🚀 Quick Start

### Prerequisites
- Python 3.8 or higher
- Git (with Git LFS for large files)
- Jupyter Notebook/Lab

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/realyashagarwal/Climate_Change.git
   cd Climate_Change
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter**
   ```bash
   jupyter notebook
   ```

### Execution Workflow

Execute notebooks in the following sequence:

1. **📊 Data Preprocessing** (`1-Data_Preprocessing.ipynb`)
   - Data cleaning and validation
   - Missing value imputation
   - Feature engineering

2. **🔍 Exploratory Data Analysis** (`2-Exploratory_Data_Analysis.ipynb`)
   - Statistical summaries
   - Correlation analysis
   - Visualization of trends and patterns

3. **🤖 Model Training & Forecasting** (`3-Model_Training_and_Future_Forecasting.ipynb`)
   - Model selection and training
   - Performance evaluation
   - Future emission predictions

## 📈 Key Findings

- **Strong Correlation**: GDP per capita shows significant positive correlation with CO₂ emissions
- **Development Patterns**: Emerging economies display steeper emission growth trajectories
- **Policy Implications**: Model predictions suggest urgent need for decoupling economic growth from carbon intensity

## 🔮 Future Projections

The model generates three emission scenarios:
- **Business as Usual**: Current trends continue
- **Moderate Action**: 25% reduction in carbon intensity
- **Aggressive Action**: 50% reduction targeting Paris Agreement goals

## 🛠️ Dependencies

```
pandas==1.5.3          # Data manipulation and analysis
numpy==1.23.5           # Numerical computing
scikit-learn==1.2.2     # Machine learning algorithms
matplotlib==3.7.1       # Static visualizations
seaborn==0.12.2         # Statistical data visualization
statsmodels==0.14.0     # Statistical modeling
openpyxl==3.1.2         # Excel file handling
ipykernel==6.22.0       # Jupyter notebook kernel
```

## 📝 Usage Examples

### Loading and Preprocessing Data
```python
import pandas as pd
from sklearn.preprocessing import StandardScaler

# Load cleaned data
df = pd.read_csv('data/processed/data_cleaned.csv')

# Feature scaling
scaler = StandardScaler()
features_scaled = scaler.fit_transform(df[['GDP_per_capita', 'Population']])
```

### Making Predictions
```python
import pickle

# Load trained model
with open('models/Trained-Model.pkl', 'rb') as f:
    model = pickle.load(f)

# Generate predictions
predictions = model.predict(features_scaled)
```

## 📊 Data Sources

- World Bank


## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Yash Agarwal**
- GitHub: [@realyashagarwal](https://github.com/realyashagarwal)
- LinkedIn: [Connect with me](www.linkedin.com/in/yashagarwal2004)
- Email: y2907ash@gmail.com


---

⭐ **Star this repository if you found it helpful!**

*"The climate crisis is a race we are losing, but it is a race we can win." - UN Secretary-General António Guterres*
