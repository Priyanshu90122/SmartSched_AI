# SmartOs — CPU Scheduling & Page Replacement Simulator

A Django-based web application that simulates CPU Scheduling Algorithms and Page Replacement Algorithms, enhanced with Machine Learning models to predict CPU burst times and improve scheduling efficiency.

---

## Overview

SmartOs combines classical Operating System concepts with Machine Learning to simulate and analyze process scheduling. Users can input process data, run scheduling simulations, and get ML-powered burst time predictions through an interactive web interface.

---

## Features

- Simulate CPU Scheduling Algorithms (FCFS, SJF, Round Robin, Priority)
- Simulate Page Replacement Algorithms (FIFO, LRU, Optimal)
- ML-based CPU Burst Time Prediction using trained models
- Performance metrics — Waiting Time, Turnaround Time, System Throughput
- Django web interface with production-ready deployment
- Deployed on Heroku with Gunicorn server

---

## ML Models

| Model | File | Purpose |
|-------|------|---------|
| Predictive Model | `predictive_model.pkl` | CPU burst time prediction |
| Gradient Boosting (GBR) | `predictive_model_gbr.pkl` | 85% accuracy on process workload data |
| Scheduler Model | `scheduler_model.pkl` | Scheduling efficiency optimization |

---

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Python, Django |
| ML | Scikit-learn, Gradient Boosting |
| Database | SQLite3 |
| Deployment | Heroku, Gunicorn |

---
**## Project Structure
Smart-Os/
│
├── PRD/                      # Production settings
├── app/                      # Main Django app
├── venv/                     # Virtual environment
├── manage.py                 # Django entry point
├── db.sqlite3                # SQLite database
├── predictive_model.pkl      # Trained ML model
├── predictive_model_gbr.pkl  # Gradient Boosting model (85% accuracy)
├── scheduler_model.pkl       # Scheduler prediction model
├── procfile                  # Heroku process config
├── runtime.txt               # Python version for Heroku
└── requirements.txt          # Python dependencies**

---

## How to Run Locally

**1. Clone the Repository**
```bash
git clone https://github.com/ravi0-web/Smart-Os.git
cd Smart-Os
```

**2. Create Virtual Environment**
```bash
python -m venv venv
source venv/bin/activate        # On Windows: venv\Scripts\activate
```

**3. Install Dependencies**
```bash
pip install -r requirements.txt
```

**4. Run Migrations**
```bash
python manage.py migrate
```

**5. Start the Server**
```bash
python manage.py runserver
```

Open `http://127.0.0.1:8000` in your browser.

---

## Performance Metrics Analyzed

- **Waiting Time** — Time a process waits in the ready queue
- **Turnaround Time** — Total time from arrival to completion
- **System Throughput** — Number of processes completed per unit time
- **Burst Time Prediction Accuracy** — 85% using Gradient Boosting (GBR)

---



## Project Structure
