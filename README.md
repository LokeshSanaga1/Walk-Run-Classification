# WalkRun Activity Classification

## Overview
This project focuses on accurately classifying **walking** and **running** activities using motion sensor data (accelerometer and gyroscope). It empowers **wearable technologies**, **digital health apps**, and **fitness platforms** to deliver smarter insights and better user experiences.

The system is designed for real-time deployment in smartwatches and fitness bands and supports advanced analytics such as **gait tracking**, **fatigue detection**, and **mobility recovery monitoring**.

### Key Objectives
- Classify activities (walking or running) using 3-axis motion sensor data.
- Support health recovery tracking and athletic performance enhancement.
- Enable integration with IoT-based wearable devices for real-time monitoring.

## Domain Analysis
- **Healthcare**: Tracks patient recovery post-surgery and detects irregular movement patterns.
- **Fitness**: Supports training analysis, calorie tracking, and performance metrics.
- **Wearables**: Real-time classification from wrist-based sensor data (smartwatches, bands).

## Dataset Features
The dataset consists of multiple attributes captured from wrist-mounted sensors:
- **DateTime**: Helps identify patterns in daily activity levels.
- **Username**: Supports personalized feedback and tracking.
- **Wrist**: Sensor placement (Left/Right), ensures wearable compatibility.
- **Activity**: Target label – walking or running.
- **Acceleration (x, y, z)**: Measures directional movement intensity.
- **Gyroscope (x, y, z)**: Captures rotational movement (e.g., wrist rotation).

## Business Case
- Empowers smart wearables with real-time motion intelligence.
- Enables healthcare providers to track patient mobility progression.
- Offers scalable opportunities like **multi-activity classification**, **fatigue detection**, and **personalized gait analytics**.
- Opens revenue channels through:
  - Device licensing
  - SaaS platforms
  - Premium fitness subscriptions

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/LokeshSanaga1/WalkRun-Activity-Classification.git
   cd WalkRun-Activity-Classification

## Install dependencies:

```bash
pip install -r requirements.txt
```
## Requirements
```
pandas
numpy
matplotlib
seaborn
scikit-learn
xgboost
imblearn
```
## Usage
- Prepare Data:
  - Load and preprocess the dataset (e.g., remove nulls, encode activity labels).
- Train Model:
  - Multiple models were tested: Logistic Regression, Decision Tree, KNN, SVM, Random Forest.
  - XGBoost achieved the best results in terms of accuracy, F1-score, and generalization.
  - Example:
    ```bash
    Copy
    Edit
    python train_model.py
    ```
- Evaluate:
  - Assess performance using metrics like accuracy, precision, recall, F1-score, and ROC-AUC.
- Predict:
  - Use the trained XGBoost model to classify new walking/running data points.

## Methodology
- Data Preprocessing: Normalized sensor data, handled label encoding, and used SMOTE for balancing.
- Model Testing:
  - Evaluated multiple classifiers.
  - XGBoost showed the best performance in cross-validation.
- Model Evaluation: Metrics used include F1-score, accuracy, and confusion matrix.

## Results
- Best Model: XGBoost outperformed all others, providing superior accuracy and robustness.
- Real-time prediction ready, optimized for deployment in wearable devices.
- Enhances user experience by delivering reliable activity insights.

## Contributing
Contributions are welcome! Feel free to submit issues or pull requests to enhance the project.

