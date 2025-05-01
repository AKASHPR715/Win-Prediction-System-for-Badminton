
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
