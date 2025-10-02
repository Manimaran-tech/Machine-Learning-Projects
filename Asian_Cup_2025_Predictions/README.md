# 🏏 T20 Tournament Prediction using XGBoost

This project simulates a T20 cricket tournament (Asia Cup style) using historical T20I match data from [Cricsheet](https://cricsheet.org/). The model predicts winners of group stage matches, Super 4 matches, and the final, based on team statistics and an XGBoost classifier.  

> **Note:** The model **excludes match data from 9th Sept 2025 to 28th Sept 2025** to ensure fair predictions without “cheating.”

---

## 📌 Features

- Loads **Cricsheet JSON data** and extracts match stats.
- Calculates **historical team performance**:
  - Win rate
  - Average runs
  - Wickets
  - Other relevant metrics
- Trains an **XGBoost model** for match outcome prediction.
- Simulates tournament stages:
  - **Group Stage** → Only group stage match data is required as input.
  - **Super 4 Stage & Finals** → Teams automatically advance based on **group stage points**.
- Generates prediction results as CSV files.
- Provides **table and chart visualizations** for tournament flow.

---

## 🔍 How It Works

### 1️⃣ Load Historical Data
- Load all available T20I matches from Cricsheet.  
- **Exclude match data from 09/09/2025 to 28/09/2025** to prevent data leakage.

### 2️⃣ Feature Extraction
- Calculate team statistics like win rate, average runs, wickets, etc.
- Prepare features suitable for the XGBoost model.

### 3️⃣ Model Training
- Train an **XGBoost classifier** using historical match features and outcomes.

### 4️⃣ Group Stage Prediction
- Predict outcomes of **group stage matches** using the trained model.  
- Calculate **points for each team** in the group.

### 5️⃣ Super 4 & Final Simulation
- Top teams from each group automatically advance to **Super 4**.  
- Based on Super 4 points, **top 2 teams advance to the final**.  
- No additional input beyond group stage matches is required.

---

## 🗂️ Tournament Flow

Group Stage Matches (Input)
│
▼
Points Calculation
│
▼
Top Teams Advance → Super 4
│
▼
Top 2 Teams → Final
│
▼
Winner Predicted


---

## 📊 Outputs

- `group_stage_predictions.csv` → Group stage match results  
- `super4_predictions.csv` → Super 4 results  
- `final_predictions.csv` → Final match result  

> Using this approach, the model accurately replicated the **Asia Cup 2025**, with **India vs Pakistan** in the final. The model correctly predicted **India as the winner** with **79% confidence**.

---

## 🛠️ Requirements

- Python 3.8+
- Install dependencies:
```bash
pip install pandas numpy xgboost scikit-learn matplotlib seaborn
