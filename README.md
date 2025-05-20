# COVID-19 Global Data Tracker

## Project Description
This project is a data analysis and reporting notebook (or app) that tracks global COVID-19 trends. It analyzes cases, deaths, recoveries, and vaccinations across countries and time. The project involves cleaning and processing real-world data, performing exploratory data analysis (EDA), generating insights, and visualizing trends using Python data tools.

By the end, you'll have a detailed data analysis report with visuals and narrative insights suitable for presentation or publishing.

---

## Project Objectives

- Import and clean COVID-19 global data
- Analyze time trends (cases, deaths, vaccinations)
- Compare metrics across countries/regions
- Visualize trends with charts and maps
- Communicate findings in a Jupyter Notebook or PDF report

---

## Project Segments (Step-by-Step Guide)

### 1️⃣ Data Collection

**Goal:** Obtain a reliable COVID-19 dataset.

**Data Sources:**

- Our World in Data COVID-19 Dataset (CSV & API)  
- Johns Hopkins University GitHub Repository

**Recommended:** Use the cleaned CSV from Our World in Data (easy to load with pandas).

**Action:**  
Download `owid-covid-data.csv` from [Our World in Data](https://ourworldindata.org/covid-cases) and save it in your project working folder.

---

### 2️⃣ Data Loading & Exploration

**Goal:** Load the dataset and explore its structure.

**Tasks:**

- Load data using `pandas.read_csv()`.
- Check columns with `df.columns`.
- Preview rows using `df.head()`.
- Identify missing values with `df.isnull().sum()`.

**Tools:** pandas

**Key columns to note:**  
`date, location, total_cases, total_deaths, new_cases, new_deaths, total_vaccinations`, etc.

---

### 3️⃣ Data Cleaning

**Goal:** Prepare data for analysis.

**Tasks:**

- Filter countries of interest (e.g., Kenya, USA, India).
- Drop rows with missing dates or critical values.
- Convert `date` column to datetime format using `pd.to_datetime()`.
- Handle missing numeric values with `fillna()` or `interpolate()`.

**Tools:** pandas

---

### 4️⃣ Exploratory Data Analysis (EDA)

**Goal:** Generate descriptive statistics and explore trends.

**Tasks:**

- Plot total cases over time for selected countries.
- Plot total deaths over time.
- Compare daily new cases between countries.
- Calculate death rate as `total_deaths / total_cases`.

**Visualizations:**

- Line charts for cases and deaths over time.
- Bar charts showing top countries by total cases.
- Optional: heatmaps for correlation analysis.

**Tools:** matplotlib, seaborn

---

### 5️⃣ Visualizing Vaccination Progress

**Goal:** Analyze vaccination rollouts.

**Tasks:**

- Plot cumulative vaccinations over time for selected countries.
- Compare percentage of vaccinated population.

**Charts:**

- Line charts.
- Optional: Pie charts for vaccinated vs. unvaccinated.

**Tools:** matplotlib, seaborn

---

### 6️⃣ Optional: Build a Choropleth Map

**Goal:** Visualize cases or vaccination rates by country on a world map.

**Tools:** Plotly Express or geopandas (advanced)

**Tasks:**

- Prepare a dataframe with `iso_code` and `total_cases` for the latest date.
- Plot a choropleth showing case density or vaccination rates.

---

### 7️⃣ Insights & Reporting

**Goal:** Summarize findings.

**Tasks:**

- Write 3-5 key insights from the data, e.g., "Country X had the fastest vaccine rollout."
- Highlight anomalies or interesting patterns.
- Use markdown cells in Jupyter Notebook to write your narrative.

**Deliverables:**

- A well-documented Jupyter Notebook combining code, visualizations, and narrative explanations.
- Optional: Export notebook to PDF or prepare a PowerPoint with screenshots.

---

## Recommended Tools

- Jupyter Notebook (or VS Code with Jupyter extension)
- pandas
- matplotlib & seaborn
- Optional: plotly, geopandas

---

## References

- [Our World in Data COVID-19 Dataset](https://ourworldindata.org/covid-cases)
- [Johns Hopkins University GitHub Repository](https://github.com/CSSEGISandData/COVID-19)
- [Kaggle COVID-19 Datasets](https://www.kaggle.com/datasets)

---

## How to Run

1. Download the dataset CSV and place it in your working folder.
2. Open the Jupyter Notebook (`.ipynb`) in VS Code or Jupyter environment.
3. Run cells sequentially from data loading to analysis.
4. Add your insights in markdown cells towards the end.
5. Export or share your final notebook/report.


