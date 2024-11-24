
# Apache Beam and Exploratory Data Analysis Projects

This repository showcases three projects that demonstrate the use of advanced data processing, interactive visualizations, and automated exploratory data analysis (EDA). The projects utilize **Apache Beam**, **D3.js**, and **Sweetviz** for real-time processing, visual insights, and structured data analysis. Each project includes detailed documentation, sample code, and references to Colab notebooks and YouTube tutorials.

---

## Table of Contents

1. [Project Descriptions](#project-descriptions)
   - [1. Apache Beam: Real-Time Movie Data Processing](#1-apache-beam-real-time-movie-data-processing)
   - [2. World Happiness Report 2019: Advanced EDA with D3.js and PyCaret](#2-world-happiness-report-2019-advanced-eda-with-d3js-and-pycaret)
   - [3. Netflix Dataset Analysis Using Sweetviz](#3-netflix-dataset-analysis-using-sweetviz)
2. [Technologies Used](#technologies-used)
3. [How to Use](#how-to-use)
4. [Repository Structure](#repository-structure)
5. [Colab Notebooks and YouTube Tutorials](#colab-notebooks-and-youtube-tutorials)

---

## Project Descriptions

### 1. Apache Beam: Real-Time Movie Data Processing

**Objective:** Demonstrate the use of **Apache Beam** for processing movie data with features like filtering, transforming, and windowing operations in a simulated real-time streaming environment.

#### Key Features
- **Composite Transforms:** Encapsulates multiple processing steps into reusable components.
- **ParDo:** Applies custom logic to individual elements.
- **Windowing and Triggers:** Groups data into 60-second intervals for processing.
- **Simulated Streaming:** Generates dynamic streaming data for real-time applications.
- **Dynamic Outputs:** Writes processed results to Google Drive for easy access.

#### Pipeline Steps
1. Simulate streaming movie data.
2. Parse raw CSV data into structured dictionaries.
3. Apply windowing to group data by fixed intervals.
4. Use composite transforms to filter and format movie data.
5. Save results as a text file in Google Drive.

#### Output
A processed output file (`movies_output.txt`) containing movie titles and their respective countries:
```
Title_1: Country_1
Title_2: Country_2
...
```

---

### 2. World Happiness Report 2019: Advanced EDA with D3.js and PyCaret

**Objective:** Analyze the **2019 World Happiness Report** dataset to uncover insights through **interactive visualizations** and **predictive modeling**.

#### Key Features
- **Interactive Visualizations with D3.js:**
  - Scatter Plot: Happiness Score vs GDP per Capita.
  - Bar Chart: Top 10 happiest countries.
  - Heatmap: Correlation between socio-economic factors.
- **Predictive Modeling with PyCaret:**
  - Automates regression model comparison, tuning, and evaluation.
  - Identifies the best predictors for happiness scores.

#### Dataset
The dataset includes socio-economic indicators like:
- GDP per Capita
- Social Support
- Freedom
- Life Expectancy
- Generosity
- Corruption

#### Workflow
1. Perform EDA with D3.js for interactive visual insights.
2. Use PyCaret to build and evaluate regression models predicting happiness scores.

---

### 3. Netflix Dataset Analysis Using Sweetviz

**Objective:** Automate the EDA of the Netflix dataset to uncover trends and patterns using **Sweetviz**, a Python library for visually appealing reports.

#### Key Features
- Generate interactive reports summarizing data distributions and correlations.
- Identify trends in content type, ratings, and release years.

#### Insights
- **Content Type:** Movies dominate Netflix’s catalog.
- **Popular Ratings:** TV-MA and TV-14 are most common.
- **Release Year Trends:** A significant rise in content production post-2010.

#### Output
An HTML report (`Netflix_Analysis.html`) with an in-depth summary of the dataset.

---

## Technologies Used

- **Apache Beam:** Distributed data processing framework.
- **D3.js:** JavaScript library for interactive, browser-based visualizations.
- **Sweetviz:** Python library for automated EDA.
- **PyCaret:** Low-code machine learning library for regression modeling.
- **Google Colab:** Cloud-based environment for running Python and JavaScript code.
- **Pandas, Matplotlib, Seaborn:** Data manipulation and static visualizations.

---

## How to Use

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/subhashpolisetti/apache-beam-and-eda-projects.git
   ```

2. **Set Up Dependencies:**
   - Install Python libraries:
     ```bash
     pip install apache-beam pandas matplotlib seaborn sweetviz pycaret
     ```

3. **Run Projects:**
   - Open the Colab notebooks for each project and follow the instructions provided.

---

## Repository Structure

```
apache-beam-and-eda-projects/
├── apache-beam-processing/
│   ├── Composite_Transforms_and_Real_Time_Data_with_Apache_Beam.ipynb
│   ├── README.md
│   └── movies_output.txt-00000-of-00001
│
├── eda-d3js-visualizations/
│   ├── World_Happiness_Report_2019_Advanced_EDA_with_D3_js_Visualizations.ipynb
│   ├── bar_chart_html.html
│   ├── heatmap_html.html
│   ├── scatter_plot.html
│   └── README.md
│
├── auto-eda-analysis/
│   ├── Netflix_EDA_with_Sweetviz.ipynb
│   ├── Netflix_Analysis.html
│   └── README.md
│
└── README.md
```

---

## Colab Notebooks and YouTube Tutorials

| **Project**                                           | **Colab Notebook**                                        | **YouTube Tutorial**                                       |
|-------------------------------------------------------|-----------------------------------------------------------|-----------------------------------------------------------|
| Apache Beam: Real-Time Movie Data Processing          | [Open in Colab](https://github.com/subhashpolisetti/apache-beam-and-eda-projects/blob/main/apache-beam-processing/Composite_Transforms_and_Real_Time_Data_with_Apache_Beam.ipynb)                                        | [Watch Tutorial](https://www.youtube.com/playlist?list=PL6O21IOHvBmfnPYmHJRWiovggjKClTI_w)                                       |
| World Happiness Report 2019: Advanced EDA with D3.js  | [Open in Colab](https://github.com/subhashpolisetti/apache-beam-and-eda-projects/blob/main/eda-d3js-visualizations/World_Happiness_Report_2019_Advanced_EDA_with_D3_js_Visualizations.ipynb)                                        | [Watch Tutorial](https://www.youtube.com/playlist?list=PL6O21IOHvBmfnPYmHJRWiovggjKClTI_w)                                       |
| Netflix Dataset Analysis Using Sweetviz               | [Open in Colab](https://github.com/subhashpolisetti/apache-beam-and-eda-projects/blob/main/%E2%80%8Eauto-eda-analysis/Netflix_EDA_with_Sweetviz.ipynb)                                        | [Watch Tutorial](https://www.youtube.com/playlist?list=PL6O21IOHvBmfnPYmHJRWiovggjKClTI_w)                                       |



