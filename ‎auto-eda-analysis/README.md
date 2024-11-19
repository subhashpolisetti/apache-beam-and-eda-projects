
# **Netflix Dataset Analysis Using Sweetviz**

This project demonstrates an exploratory data analysis (EDA) of the **Netflix Movies and TV Shows dataset** using **Sweetviz**, a Python library for automated and visually appealing reports. The analysis aims to uncover key insights about Netflix content and provide a structured overview of the dataset.

---

## **Table of Contents**
1. [Dataset Overview](#dataset-overview)
2. [Features](#features)
3. [Tools and Libraries](#tools-and-libraries)
4. [Key Insights](#key-insights)
5. [Next Steps](#next-steps)

---

## **Dataset Overview**
The dataset contains metadata about Netflix Movies and TV Shows, including:
- Titles
- Content types (Movie or TV Show)
- Genres
- Directors and cast
- Countries of origin
- Release years
- Ratings and durations

**Dataset Source**: [Netflix Movies and TV Shows on Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)

---

## **Features**
Key features analyzed in this project:
- **Type**: Movie or TV Show.
- **Title**: Name of the content.
- **Director**: Director of the content.
- **Cast**: Main actors/actresses.
- **Country**: Country of origin.
- **Release Year**: Year of release.
- **Rating**: Maturity rating (e.g., PG-13, R).
- **Duration**: Length in minutes (Movies) or seasons (TV Shows).
- **Genre**: Category of the content.

---

## **Tools and Libraries**
The following tools and libraries were used:
- **Python**: Programming language.
- **Google Colab**: Cloud-based notebook environment.
- **Kaggle API**: For downloading the dataset.
- **Sweetviz**: For automated EDA reports.
- **Pandas**: For data inspection and manipulation.
- **Matplotlib & Seaborn**: For custom visualizations.



## **How to Run the Notebook**
1. Clone this repository:
   ```bash
   git clone https://github.com/subhashpolisetti/apache-beam-and-eda-projects.git
   ```
2. Open the `Netflix_EDA.ipynb` notebook in Google Colab.
3. Upload your `kaggle.json` API token to configure the Kaggle API.
4. Follow the step-by-step instructions in the notebook to generate the Sweetviz report.

---

## **Key Insights**
- **Content Type**: Movies dominate Netflix's catalog compared to TV Shows.
- **Release Year Trends**: A significant increase in content production post-2010.
- **Popular Ratings**: TV-MA and TV-14 are the most frequent ratings.
- **Missing Data**: Some records lack information about directors and cast, which can be addressed during preprocessing.

---

## **Next Steps**
- Perform deeper analysis, such as:
  - Predicting content popularity using machine learning.
  - Clustering content based on genres, release years, or ratings.
  - Analyzing viewer preferences by integrating user data (if available).


