# Predictive Maintenance Dashboard for Industrial Equipment

This project provides a Predictive Maintenance Dashboard using machine learning techniques to anticipate equipment maintenance needs. It enables real-time monitoring and predictive analytics based on sensor data, helping reduce unplanned downtime and optimise maintenance schedules.

---

## What the Project Does

### Data Collection and Preprocessing
- Collects historical sensor data (temperature, vibration, pressure, RPM, etc.).
- Cleans and preprocesses the data to handle missing values and outliers.
- Engineers relevant features (e.g., change in temperature or vibration) to enhance model accuracy.

### Predictive Model Training
- Trains machine learning models (Random Forest, Gradient Boosting, Neural Networks) using historical patterns.
- Identifies key indicators that suggest impending equipment failure or maintenance needs.

### Model Deployment
- Deploys the trained model within a web application.
- Exposes predictions via an API, allowing real-time interaction with incoming data.

### Dashboard Interface
- Interactive dashboard displays:
  - Real-time metrics (temperature, vibration, pressure, etc.)
  - Predictions and maintenance alerts
  - Historical data analysis
- Allows users to explore predictions by machine or time period.

### Real-Time Monitoring and Alerts
- Continuously monitors incoming sensor data.
- Triggers alerts when high failure probability is detected.

### User Interaction
- Designed for use by:
  - Maintenance engineers
  - Operations managers
- Provides an intuitive, non-technical interface for viewing predictions and insights.

---

## Project Workflow

1. Data Input – Collect and feed real-time sensor data.
2. Data Processing – Clean and preprocess the data.
3. Model Prediction – Run data through the machine learning model.
4. Dashboard Update – Display machine status and predictions.
5. Alerting – Trigger alerts when needed.

---

## Benefits

- Proactive Maintenance: Avoid breakdowns with predictive alerts.
- Data-Driven Decisions: Maintenance teams gain actionable insights.
- Operational Efficiency: Reduces downtime and extends equipment life.

---

## Use Cases

- Manufacturing plants needing continuous machine uptime.
- Industries with high maintenance costs.
- Scenarios where unplanned downtime causes financial or safety risks.

---

## Features

- Real-time data visualisation (bar charts and trend plots)
- Predictive maintenance alerts
- Historical data tracking and analysis

---

## Installation

```bash
git clone https://github.com/yourusername/predictive-maintenance.git
cd predictive-maintenance

python -m venv venv
source venv/bin/activate   # On Windows: venv\Scripts\activate

pip install -r requirements.txt
# Install dependencies
pip install -r requirements.txt

# Run preprocessing
python src/data_preprocessing.py

# Feature engineering
python src/feature_engineering.py

# Train the model
python src/model_training.py

# Evaluate the model
python src/model_evaluation.py

# Start the web app
python app/app.py

predictive-maintenance/
├── app/
│   └── app.py               # Main Flask app
│   └── dash_app.py          # Dashboard logic
├── models/                  # Trained machine learning models
├── src/
│   ├── data_preprocessing.py
│   ├── feature_engineering.py
│   ├── model_training.py
│   └── model_evaluation.py
├── templates/               # HTML templates
├── static/                  # CSS and JS assets
├── config.yaml              # App configuration file
├── requirements.txt         # Dependency list
└── README.md                # Project documentation
```

## License
This project is licensed under the MIT License.

