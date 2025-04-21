# 🧠 Log Anomaly Detection using Isolation Forest

This project demonstrates how to analyze system logs using **AI-powered anomaly detection**. We use the **Isolation Forest** machine learning algorithm from `scikit-learn` to automatically detect suspicious patterns in log files.

---

## 📌 Features

- Parse timestamped log entries (INFO, WARNING, ERROR, CRITICAL)
- Assign numeric scores to log severity
- Add log message length as a feature
- Detect anomalies using Isolation Forest
- Print structured anomaly report

---

## 🛠 Technologies Used

- Python 3.8+
- pandas
- scikit-learn (Isolation Forest)
- numpy
- Regular Expressions (for log parsing)

---

## 📂 Sample Input Format

Each line in your `system_logs.txt` should follow:

```txt
2024-04-19 11:45:22 ERROR Connection failed to database
2024-04-19 11:45:25 INFO  User login successful

🚀 How to Run

Clone this repository:

git clone https://github.com/sreeni85/log-analysis-isolation.git
cd log-analysis-isolation

Set up a virtual environment (recommended):

python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

python log_anomaly_detector.py

📊 Output Sample

🔍 **Detected Anomalies:**
2024-04-19 11:46:30 ❌ Anomaly: CRITICAL Memory leak detected
2024-04-19 11:46:45 ❌ Anomaly: WARNING Slow query response

🧠 Why Isolation Forest?
Isolation Forest is a fast and effective unsupervised anomaly detection algorithm well-suited for high-dimensional, unlabeled data — perfect for log pattern analysis.







