
# World Happiness Report 2019: Advanced EDA with D3.js and Predictive Modeling with PyCaret

This repository showcases an analysis of the **2019 World Happiness Report** dataset using:
- **D3.js**: For interactive and advanced visualizations embedded in a Google Colab notebook.
- **PyCaret**: For automated machine learning workflows, including model building, comparison, and evaluation.

---

## Table of Contents

1. [Overview](#overview)
2. [Dataset](#dataset)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Project Workflow](#project-workflow)
   - [Exploratory Data Analysis (EDA) with D3.js](#exploratory-data-analysis-eda-with-d3js)
   - [Predictive Modeling with PyCaret](#predictive-modeling-with-pycaret)


---

## Overview

The **2019 World Happiness Report** ranks countries by happiness levels based on socio-economic factors such as GDP, social support, life expectancy, freedom, and more. This project provides insights and predictions using:
1. **Interactive Visualizations**: Created using **D3.js**, these include:
   - A scatter plot: Happiness Score vs GDP per Capita.
   - A bar chart: Top 10 happiest countries.
   - A heatmap: Correlation between socio-economic factors.
2. **Predictive Modeling**: Built with **PyCaret's regression module**, the project identifies the best model to predict happiness scores based on the dataset.

---

## Dataset

The dataset is sourced from the [World Happiness Report on Kaggle](https://www.kaggle.com/unsdsn/world-happiness). It contains the following columns:

| Column Name                | Description                                             |
|----------------------------|---------------------------------------------------------|
| `Country`                  | Name of the country                                     |
| `Happiness Score`          | Overall happiness score for the country                |
| `GDP per Capita`           | Economic performance per individual                    |
| `Social Support`           | Availability of social connections                     |
| `Life Expectancy`          | Healthy life expectancy of citizens                    |
| `Freedom`                  | Perceived freedom in decision-making                   |
| `Generosity`               | Community support and charitable contributions         |
| `Corruption`               | Perception of corruption in government/business        |

---

## Technologies Used

- **D3.js**: For interactive, browser-based visualizations.
- **PyCaret**: A low-code machine learning library for Python.
- **Google Colab**: For hosting and running Python and JavaScript code.
- **Pandas**: For data manipulation and analysis.
- **Matplotlib/Seaborn**: For static visualizations during initial EDA.

---

## Installation

### Prerequisites
1. Install **PyCaret** and related dependencies:
   ```bash
   pip install pycaret pandas matplotlib seaborn
   ```
2. Ensure your environment supports **D3.js** in Jupyter or Colab notebooks.

### Repository Setup
1. Clone this repository:
   ```bash
   git clone https://github.com/subhashpolisetti/apache-beam-and-eda-projects.git



## Project Workflow

### 1. Exploratory Data Analysis (EDA) with D3.js
We explore the data with both static and interactive visualizations:
- **Scatter Plot**: Explore the relationship between **Happiness Score** and **GDP per Capita**.
- **Bar Chart**: Visualize the **Top 10 happiest countries**.
- **Heatmap**: Show correlations between features like **Freedom**, **Generosity**, and **Corruption**.

#### Sample Code: Scatter Plot with D3.js
The scatter plot visualizes **Happiness Score vs GDP per Capita** with interactive tooltips:
```html
<div id="scatterplot" style="width: 800px; height: 500px;"></div>
<script src="https://d3js.org/d3.v7.min.js"></script>
<script>
    const data = [...]  // Data passed from Python
    const margin = {top: 20, right: 30, bottom: 50, left: 50};
    const width = 800 - margin.left - margin.right;
    const height = 500 - margin.top - margin.bottom;

    const svg = d3.select("#scatterplot").append("svg")
        .attr("width", width + margin.left + margin.right)
        .attr("height", height + margin.top + margin.bottom)
        .append("g")
        .attr("transform", "translate(" + margin.left + "," + margin.top + ")");

    // Define scales and add axes...
    // Add circles for data points...
</script>
```

### 2. Predictive Modeling with PyCaret
#### Steps:
1. **Setup the PyCaret Environment**:
   ```python
   from pycaret.regression import setup, compare_models, tune_model, evaluate_model
   regression_setup = setup(data=happiness_2019, target='Happiness Score', session_id=123, normalize=True)
   ```
2. **Model Comparison**:
   ```python
   best_model = compare_models()
   ```
3. **Model Tuning**:
   ```python
   tuned_model = tune_model(best_model)
   ```
4. **Evaluation**:
   ```python
   evaluate_model(tuned_model)
   ```

#### Features:
- Compare multiple machine learning models.
- Tune hyperparameters for the best model.
- Visualize feature importance and residual plots.




