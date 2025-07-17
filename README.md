#  SpaceX Falcon 9 Launch Analysis Project

##  Problem Statement

SpaceX's Falcon 9 rocket launches play a critical role in reducing the cost of space missions by reusing boosters. However, mission outcomes—especially booster landings—are influenced by multiple factors like launch site, payload mass, and booster type. The goal of this project is to analyze historical Falcon 9 launch data, predict mission success using machine learning, and build an interactive dashboard to visualize insights for decision-making.

---

##  Project Overview

This end-to-end data science project uses SpaceX launch data to:
- Extract and clean data from API and web sources
- Explore trends via visual and geospatial analysis
- Query insights using SQL
- Build ML models to predict mission success
- Deploy a Dash dashboard to interact with the data

---

##  Technologies Used
Python, Pandas, SQLite, BeautifulSoup, Plotly, Dash, Folium, Scikit-learn, Matplotlib, Seaborn

---

##  Components Breakdown

### 1. Data Collection
- `jupyter-labs-spacex-data-collection-api-v2.ipynb`
- Pulls SpaceX launch data using REST API
- Normalizes JSON into structured DataFrame

### 2. Web Scraping
- `SpaceX-web-scraping.ipynb`
- Extracts booster landing data from HTML tables using BeautifulSoup
- Merges scraped data with API results

### 3. Data Wrangling
- `Spacex-Data wrangling.ipynb`
- Cleans, merges, and standardizes datasets
- Saves combined data as `spacex_launch_geo.csv`

### 4. Exploratory Data Analysis
- `SpaceX-EDA-Data-Visualization.ipynb`
- Analyzes launch success rates by site and payload
- Uses scatter plots, pie charts, and bar graphs

### 5. SQL-Based Analysis
- `jupyter-labs-eda-sql-coursera_sqllite.ipynb`
- Loads cleaned CSV into SQLite
- Uses SQL queries to validate and explore trends

### 6. Geospatial Visualization
- `SpacexX-Folium-Visualization.ipynb`
- Uses Folium to map launch sites with interactive markers
- Shows success/failure by location

### 7. Machine Learning
- `SpaceX-Machine-Learning-Prediction-Part-5-v1.ipynb`
- Builds classifiers (LogReg, SVM, Tree) to predict mission outcome
- Uses payload, site, booster version as features
- Evaluates models with confusion matrices and accuracy scores

---

## Interactive Dashboard

- Built using Dash & Plotly with live controls
- Dropdown filters, scatter and pie charts, payload slider
- Launch site and booster version selection
- **🔗 Live Dashboard**: [https://spacex-falcon-9.onrender.com](https://spacex-falcon-9.onrender.com)

---

## Run Locally

```bash
git clone https://github.com/Samidha9/SpaceX-Falcon-9.git
cd SpaceX-Falcon-9
pip install -r requirements.txt
python app.py
