# 🏸 Badminton Win Prediction & Live Match Simulation using Machine Learning

This project is a comprehensive machine learning system designed to predict the outcome of badminton matches and simulate live match progress using match data. It incorporates real-time analytics, probabilistic forecasting, and momentum-based insights to determine match outcomes.

---

## 📌 Table of Contents

- [Overview](#-overview)
- [Key Features](#-key-features)
- [License](#-license)

---

## 🧠 Overview

The project is focused on predicting the winner of a badminton game using historical match point-by-point data. The idea is to train a machine learning model on match features such as score progression, who served, point difference, and cumulative scoring to determine the likelihood of winning. Additionally, the model provides a **live simulation view** with dynamic probability changes and momentum tracking.

---

## 🚀 Key Features

- 🔍 **Data Cleaning & Preprocessing:** Standardizes scores and handles missing values intelligently.
- 🤖 **Machine Learning Model:** Trained using Random Forest Classifier for binary classification (Win/Loss).
- 📈 **Win Prediction Engine:** Predicts match results and probabilities based on historical score data.
- 🕒 **Live Game Simulator:** Simulates a game with real-time predictions and updates using momentum and time-stamped scoring.
- 📊 **Probability Insights:** Dynamic win probability calculation based on current score and momentum swings.
- 💾 **Model Saving & Loading:** Trained model is saved using `joblib` for reuse.

---

## 📁 Project Structure

---

## 🛠️ How It Works

### 📉 Dataset

- Format: CSV with columns like `SCORE_SHEET_ID`, `SET_NO`, `SERVER`, `RECIEVER`, `SCORE`, `SCOREDBY`, `OPPONENT SCORE`, and `TIME`.
- Irrelevant columns are removed.
- Scores are standardized based on who scored the point (server or receiver).

### 🧪 Feature Engineering

- `STANDARDIZED_SCORE` and `STANDARDIZED_OPPONENT_SCORE`
- `POINT_DIFFERENCE`
- `CUMULATIVE_SCORE` (tracks point count per player)

### 🤖 Model Training

- Model: `RandomForestClassifier`
- Evaluation: Accuracy and classification report
- Trained model is saved as a `.pkl` file

### 🔮 Prediction

- Input: Match CSV file
- Output: Match outcome predictions, live scores, probabilities for each player

### 🎮 Live Simulation

- Time-based simulation of matches using `time.sleep()`
- Predicts winner dynamically based on updated scores and momentum shifts

---

## 📦 Installation

1. Clone the repository:

```bash
git clone https://github.com/yourusername/Badminton-Win-Predictor.git
cd Badminton-Win-Predictor

