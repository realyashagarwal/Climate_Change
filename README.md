# CarbonCast: Development's Carbon Cost
**Predicting National CO₂ Trajectories Through Socioeconomic Indicators**

`mermaid
graph LR
A[Raw Data] --> B(Preprocessing)
B --> C[Cleaned Data]
C --> D(EDA)
D --> E(Model Training)
E --> F[Forecasts]
`

## 📂 Repository Structure
`
Climate_Change/
├── data/
│   ├── raw/                 # Original datasets
│   └── processed/           # Analysis-ready data
├── notebooks/               # Jupyter notebooks
├── models/                  # Trained models (Git LFS)
├── outputs/                 # Forecast results
├── docs/                    # Documentation assets
├── requirements.txt         # Python dependencies
└── README.md                # Project documentation
`

## ⚙️ Setup
`powershell
# Install Git LFS first (if not installed)
git lfs install

# Clone repository
git clone https://github.com/realyashagarwal/Climate_Change.git
cd Climate_Change

# Install dependencies
pip install -r requirements.txt
`

## ▶️ Execution Order
1. `notebooks/1-Data_Preprocessing.ipynb`
2. `notebooks/2-Exploratory_Data_Analysis.ipynb`
3. `notebooks/3-Model_Training_and_Future_Forecasting.ipynb`

[Full documentation and insights](https://github.com/realyashagarwal/Climate_Change)
