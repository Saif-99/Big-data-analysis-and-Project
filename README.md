# Big-data-analysis-and-ProjectProject Structure
├── A1 (A) Bigdata.ipynb   # Main Jupyter/Colab notebook with full analysis
├── sample_data/           # Folder containing input CSV files
│   ├── flat-ui__data-<date>.csv   # Original dataset
│   └── test1.csv                   # Filtered dataset (2000–2020)
├── README.md              # Project documentation

Setup Instructions

This project was developed in Google Colab, but you can also run it locally.

1. Clone the Repository
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>

2. Install Dependencies

If running locally, install the required Python libraries:

pip install pandas numpy matplotlib scikit-learn

3. Data Requirements

The dataset file (flat-ui__data-<date>.csv) should be placed in the sample_data/ folder.


4. Running the Notebook

Open A1 (A) Bigdata.ipynb in:

Google Colab → Recommended (includes Google Drive mounting).

Jupyter Notebook → Local environment.

Methodology

The project is divided into three main parts:

Loading the data 
Data Cleaning & Visualization
Model Development & Forecasting

Models used:
Linear Regression
Ridge Regression
Gradient Boosting Regressor

Evaluation metrics: R² Score and RMSE.
Forecast emissions for 2021–2040 for each country.

Results

Linear & Ridge Regression: Near-perfect performance (R² ≈ 1.0, RMSE < 1), indicating strong correlation between fuel-based features and total emissions.

Gradient Boosting: Strong explanatory power but higher prediction error (R² ≈ 0.9996, RMSE ~11,100).

Forecasts (2021–2040):

Developed countries (USA, Canada): Emissions decline or stabilize, consistent with climate commitments.

Developing countries (Brazil, Colombia): Emissions continue rising due to industrial growth and energy demand.

Example Plots

The notebook generates:

Total emissions (2000–2020) by country.

Per capita emissions trends.

Fuel-specific emissions (Gas Fuel, Solid Fuel).

Forecast plots for each country (2021–2040).

Replication

To reproduce:

Place dataset in sample_data/.

Run notebook cells sequentially.

Forecast results and plots will be generated automatically.

License

This project is released under the MIT License. You are free to use, modify, and distribute it with proper attribution.
