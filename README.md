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

