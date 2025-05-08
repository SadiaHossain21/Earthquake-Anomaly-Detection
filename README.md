# Earthquake Pattern and Anomaly Detection

This project analyzes historical earthquake data from South Asia to detect unusual seismic patterns using statistical techniques and visualizations. It transforms geospatial and temporal data into formats suitable for detecting spikes in magnitude and frequency over time.

## Key Features

- Preprocessing of South Asian earthquake dataset
- Coordinate rounding and time transformation into "days since 1900"
- Frequency and magnitude-based visual anomaly detection
- Moving average and percentile-based anomaly detection
- Interactive plots for exploration

##  Data Source

Data is sourced from the Kaggle dataset: **Earthquakes in South Asia**

##  Technologies Used

- Python
- Pandas & NumPy
- Matplotlib
- Custom date transformation functions
- Statistical thresholding (moving average, percentiles)

## Project Structure
earthquake-anomaly-detection/
├── earthquake-anomaly-detection.ipynb # Main analysis notebook
└── README.md # Project overview

##  What This Project Does
- Loads and cleans raw earthquake data
- Rounds coordinates and standardizes features
- Converts timestamps to "days since 1900" for time analysis
- Visualizes the distribution of magnitudes and depths
- Detects unusual earthquake spikes using:
  - Rolling averages
  - Percentile thresholds
  - Visual inspection of time plots
- Trains a **logistic regression model** to classify high and low earthquake activity zones
- Evaluates the model using a confusion matrix (accuracy: **91%**)


##  How to Run It

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/earthquake-anomaly-detection.git
   cd earthquake-anomaly-detection
2. Install dependencies:
   pip install pandas numpy matplotlib scikit-learn
3. Open Notebook
   jupyter notebook earthquake-anomaly-detection.ipynb

## Why It Matters
This analysis provides a basic but effective way to detect abnormal earthquake behavior and could support future development of early warning systems.
