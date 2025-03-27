# Exoplanet-Inclination-Classification


This project uses a deep learning classifier (CNN) to predict the **orbital inclination class** of exoplanets using real-world data from the NASA Exoplanet Archive.
The model takes in features such as orbital period, radius ratio, and other planetary characteristics, and classifies the planet into one of the defined inclination categories.

---

## 🚀 Overview

Inclination of an exoplanet is a crucial factor for transit detection and understanding planetary systems. This classifier helps analyze how various orbital and physical features relate to inclination, using a supervised learning approach.

---

## 🧠 Model

- **Type**: Neural Network (CNN)
- **Input**: Planetary parameters from CSV data
- **Output**: Inclination class (`low`, `medium`, `high`)
- **Accuracy Achieved**: ~75% on test set

---

## 🧾 Features Used

- `pl_orbper`: Orbital period
- `pl_ratror`: Planet/star radius ratio
- `pl_ratdor`: Semi-major axis to star radius ratio
- `pl_bmassj`: Planet mass (Jupiter units)
- `pl_orbeccen`: Orbital eccentricity
- `pl_orbincl`: Inclination (used to create labels)
- and more...

> Target: `incl_class` (Categorical class of inclination based on thresholds)

---

## 📁 File Structure

- `inclination_classifier.ipynb` – Main notebook for data prep, training and evaluation
- `data/Copy - Total Set 2-Table 1.csv` – Cleaned dataset used for training
- `model/` – (Optional) Saved model weights
- `plots/` – Confusion matrix, accuracy/loss graphs
- `requirements.txt` – Python dependencies
