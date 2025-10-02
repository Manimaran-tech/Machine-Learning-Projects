# 🏏 T20 Tournament Prediction using XGBoost

This project simulates a T20 cricket tournament (Asia Cup style) using historical T20I match data from [Cricsheet](https://cricsheet.org/).  
The model predicts winners of group stage matches, Super 4 matches, and the final, based on team statistics and an XGBoost classifier.

---

## 📌 Features
- Loads **Cricsheet JSON data** and extracts match stats.
- Calculates **historical team performance** (win rate, average runs, wickets, etc.).
- Trains an **XGBoost model** for predicting match outcomes.
- Simulates:
  - Group Stage
  - Super 4 Stage
  - Final Match
- Generates prediction results as CSV files.
- Provides **table and chart visualizations** for the tournament flow.

---

## 📊 Outputs
- `group_stage_predictions.csv` → Group stage match results  
- `super4_predictions.csv` → Super 4 results  
- `final_predictions.csv` → Final match result  

---

## 🛠️ Requirements
- Python 3.8+
- Install dependencies:
  ```bash
  pip install pandas numpy xgboost scikit-learn matplotlib seaborn
