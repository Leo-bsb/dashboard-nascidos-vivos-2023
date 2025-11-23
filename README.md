# 📊 Brazilian Live Births Dashboard (SINASC 2023)

<p align="center">
  <img src="https://img.shields.io/badge/Framework-Streamlit-red.svg" />
  <img src="https://img.shields.io/badge/Visualization-Plotly-blue.svg" />
  <img src="https://img.shields.io/badge/Data-Pandas-yellow.svg" />
  <img src="https://img.shields.io/badge/Python-3.x-green.svg" />
  <img src="https://img.shields.io/badge/Status-Live%20App-brightgreen.svg" />
</p>

An interactive dashboard for exploring **Brazilian live birth data (SINASC 2023)**, with filters, charts and demographic insights.

🔗 **Live Dashboard:** [https://dashboard-nascidos-vivos-2023.streamlit.app/](https://dashboard-nascidos-vivos-2023.streamlit.app/)

> **Language:** The interface is in *Portuguese (PT-BR)*, as it targets Brazilian healthcare professionals and public health analysts.

---

## 📘 Overview

This dashboard provides an intuitive interface to explore **live births recorded in Brazil in 2023** using data derived from SINASC.
It includes filtering by demographic, parental and birth-related attributes, along with visualizations that help analyze patterns and distributions across Brazilian states.

The app loads and processes the dataset `Nascidos_Vivos_Dashboard_Reduzido.csv`, applies data cleaning steps, and renders dynamic charts with Plotly inside Streamlit.

---

## 🧰 Tech Stack

* **Python**
* **Streamlit**
* **Pandas**
* **Plotly**
* **Squarify** (for treemap rendering logic used in Plotly)

---

## 🎯 Main Features

### **✔️ Multi-level Filtering**

The dashboard allows filtering by:

* **Baby attributes:** Race/Color, Sex
* **Birth conditions:** Location of birth, Induction of labor, Type of presentation, State (UF)
* **Parents:** Mother's civil status, Mother's age group

### **✔️ Interactive Visualizations**

Based on the filtered dataset, the app displays:

* **Bar chart:** Birth counts per Brazilian state (UF)
* **Line chart:** Prenatal visits distribution by mother's education level
* **Pie charts:**

  * Births by sex
  * Births by type of delivery
* **Treemap:** Mother's marital status distribution

### ✔️ **Summary Metrics**

* Total births
* Average mother's age
* Average father's age
* Average newborn weight

---

## 🗂️ Data Notes

The code performs dataset cleaning, including:

* Harmonizing column names
* Standardizing categories (e.g., marital status, place of birth)
* Validating allowed values for filters
* Removing or nullifying unexpected categories

---

## 🚀 Running Locally

```bash
pip install -r requirements.txt
streamlit run app.py
```

*(The exact requirements should match the libraries imported in the code.)*

---

## 🔗 Access

Launch the dashboard here:
👉 **[https://dashboard-nascidos-vivos-2023.streamlit.app/](https://dashboard-nascidos-vivos-2023.streamlit.app/)**
