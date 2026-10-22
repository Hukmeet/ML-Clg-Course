# Assignment Repository: Machine Learning

Welcome to this repository containing three Jupyter Notebook solutions covering diverse data processing, web API integration, text classification, and predictive machine learning tasks.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Notebook Summaries](#notebook-summaries)
  - [1. Weather Data Retrieval API ](#1-weather-data-retrieval-api)
  - [2. SMS Spam Classifier using Naive Bayes](#2-sms-spam-classifier-using-naive-bayes)
  - [3. MRE Shelf-Life Prediction & Degradation Pipeline](#3-mre-shelf-life-prediction--degradation-pipeline)
- [Tech Stack & Libraries](#tech-stack--libraries)
- [Getting Started](#getting-started)
- [How to Run](#how-to-run)

---

## 🌟 Overview

This repository demonstrates practical implementations of:
- RESTful API interaction and geocoding to retrieve dynamically structured environmental datasets.
- Natural Language Processing (NLP) and text classification using TF-IDF feature extraction.
- Synthetic data generation based on chemical degradation kinetics (Arrhenius equation) and machine learning modeling for continuous shelf-life forecasting.

---

## 📓 Notebook Summaries

### 1. Weather Data Retrieval API
* **File:** `Weather_Data_Collector.ipynb` *(or equivalent weather notebook)*
* **Key Tasks:**
  - Connects to the **Open-Meteo Geocoding API** to query geographic coordinates for a given city (e.g., *Dewas*).
  - Fetches 168 hours (7 days) of detailed hourly weather forecast parameters (Temperature, Relative Humidity, Rain, Cloud Cover, Precipitation Probability).
  - Preprocesses the returned JSON response into a clean Pandas DataFrame and exports it to CSV (`dewas_weather.csv`).

---

### 2. SMS Spam Classifier using Naive Bayes
* **File:** `SMS_Spam_Classifier.ipynb`
* **Dataset:** SMS Spam Collection Dataset (5,572 records).
* **Key Tasks:**
  - Loads and labels raw text messages (`ham`: 0, `spam`: 1).
  - Applies **TF-IDF Vectorization** (`TfidfVectorizer`) with English stop-word filtering.
  - Trains a **Multinomial Naive Bayes (`MultinomialNB`)** classifier.
  - Achieves **~97.85% Test Accuracy** with real-time text sample predictions.

---

### 3. MRE Shelf-Life Prediction & Degradation Pipeline
* **File:** `MRE_Shelf_Life_Prediction.ipynb`
* **Key Tasks:**
  - Simulates a realistic 1,000-sample dataset modeling food/ration degradation using the **Arrhenius Rate Equation** (k = A • e^{-Ea / RT}).
  - Incorporates variables: Average Storage Temperature (℃), Storage Days, Humidity Spikes, Packaging Type, and Freshness Percentage.
  - Features complete Data Preprocessing, Exploratory Data Analysis (EDA), and machine learning regression model setup (`LinearRegression`, `DecisionTreeRegressor`, `RandomForestRegressor`).

---

## 🛠️ Tech Stack & Libraries

- **Language:** Python 3.x
- **Data Manipulation:** `pandas`, `numpy`
- **Web & APIs:** `requests`
- **Machine Learning & NLP:** `scikit-learn` (`TfidfVectorizer`, `MultinomialNB`, `LinearRegression`, `DecisionTreeRegressor`, `RandomForestRegressor`)
- **Data Visualization:** `matplotlib`, `seaborn`

---

## 🚀 Getting Started

### Prerequisites

Make sure you have Python 3.8+ installed along with the required libraries.

```bash
pip install numpy pandas requests scikit-learn matplotlib seaborn notebook
```

---

## 🏃 How to Run

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPOSITORY_NAME.git
   cd YOUR_REPOSITORY_NAME
   ```

2. **Launch Jupyter Notebook or Google Colab:**
   ```bash
   jupyter notebook
   ```

3. **Execute Notebooks:** Open any `.ipynb` file and execute the cells sequentially from top to bottom.

---

*Created for college assignment submission.*
