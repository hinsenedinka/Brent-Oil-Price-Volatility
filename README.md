# Brent-Oil-Price-Volatility

**Objectives**

  * Defining the data analysis workflow
  * Understanding the model and data
  * Extracting statistically valid insights in relation to the  business objective

**Repository Structure**

├── .gitignore              # To ignore unwanted files (e.g., .ipynb_checkpoints, virtual environments)
├── README.md               # The main documentation file (will be significantly expanded)
├── requirements.txt        # List of all Python dependencies
│
├── data/                   # Dedicated folder for all data files
│   ├── raw/                # The original, unprocessed Brent oil price data
│   └── events/             # The compiled event data (e.g., events.csv)
│
├── notebooks/              # Jupyter Notebooks for exploratory work and visualizations
│   ├──eda.ipynb   # For initial EDA and time series properties analysis
│   └──change-point-analysis.ipynb # For applying change point models and visualizing results
│
├── src/                    # Source code for reusable functions and scripts
│
│
└── models/  

**Data**

The analysis relies on two datasets, which should be placed in the data/ folder as follows:

Brent Oil Price Data: A CSV file containing historical Brent crude oil prices (e.g., brent_prices.csv). Place this file in data/raw/.

Event Data: A CSV file named events.csv containing a structured list of major events and their dates. A sample file is included in data/events/.

**Analysis Workflow**
The analysis is structured into a logical, two-step process:

1. Exploratory Data Analysis (EDA): Run the eda.ipynb notebook to get an initial understanding of the data. This notebook visualizes price trends, checks for stationarity, and provides a first look at how major events align with price movements.

2. Change Point Analysis: Run the change-point-analysis.ipynb notebook. This is the core of the project, where change point detection algorithms are applied to the Brent oil price data. The notebook will output the dates of the detected change points, display new statistical parameters for each segment, and correlate the findings with the events data.

**Assumptions and Limitations**

Briefly summarize the key assumptions and limitations discussed in the analysis.