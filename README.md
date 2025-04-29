# 📍 Project Overview

This project predicts whether a hotel reservation will be **canceled or honored** based on booking details.  
It is built using a complete **MLOps pipeline**, covering **model training, tracking, versioning, containerization, CI/CD automation, and cloud deployment.**

---

# 🛠️ Tech Stack & Tools Used

- **Python 3.10**
- **Machine Learning:** LightGBM, Scikit-Learn
- **MLOps Tools:** MLflow, Docker, Jenkins, GitHub Actions
- **Backend:** Flask
- **Cloud:** Google Cloud Platform (Cloud Run, Cloud Storage, Artifact Registry)
- **Others:** Pandas, NumPy, YAML, Joblib

---

# 🏗️ Project Architecture

The following architecture represents the complete end-to-end MLOps workflow:

- **Data Ingestion** → **Data Processing & Feature Engineering**
- **Model Training (LightGBM)**
- **Experiment Tracking with MLflow**
- **Model Saving and Versioning**
- **Containerization with Docker**
- **CI/CD Automation with Jenkins**
- **Deployment on Google Cloud Run**

---

# 📦 Project Setup (Local)

## Clone the Repository

```bash
git clone https://github.com/your-username/Hotel-Reservation-Prediction-MLOps.git
cd Hotel-Reservation-Prediction-MLOps
```

## Create Virtual Environment and Install Dependencies

```bash
python -m venv venv
source venv/bin/activate    # For Linux/Mac
.\venv\Scripts\activate     # For Windows
pip install -r requirements.txt
```

## Run MLflow UI (Optional for experiment tracking)

```bash
mlflow ui
```
<img src="https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps/blob/main/images/mlflow.png">

## Run the Flask App Locally

```bash
python application.py
```

The app will be available at: [http://localhost:8080](http://localhost:8080)

---

# 🐳 Docker Setup

## Build Docker Image

```bash
docker build -t hotel-reservation-prediction .
```

## Run Docker Container

```bash
docker run -p 8080:8080 hotel-reservation-prediction
```
<img src="https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps/blob/main/images/docker-1.png">

---

# ⚙️ Jenkins Setup (CI/CD)

- A **Jenkinsfile** is created for pipeline automation.
- Jenkins is configured with Docker and GitHub to pull code, build images, and deploy.

---
<img src="https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps/blob/main/images/jenkins-2.png">

# ☁️ Deployment on Google Cloud Run

- Push Docker Image to **Google Artifact Registry**.
- Deploy the containerized application on **Google Cloud Run**.
- Enjoy **auto-scaling** and **serverless execution**.
<img src="https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps/blob/main/images/gcp-2.png">
<img src="https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps/blob/main/images/gcp-1.png">
<img src="https://github.com/ambuj6392/Hotel-Reservation-Prediction-MLOps/blob/main/images/gcp-3.png">


# 🔗 Live Deployment Link: 
https://ml-project-171607476784.us-central1.run.app/

---


---

# 🧹 Folder Structure

```plaintext
Hotel-Reservation-Prediction-MLOps/
│
├── artifacts/                # Processed data, models
├── config/                   # Configuration files
├── src/                      # Source code
│   ├── data_ingestion.py
│   ├── data_processing.py
│   ├── model_training.py
│   └── logger.py
├── templates/                 # HTML files for Flask
│   └── index.html
├── static/                    # CSS, images, static files
├── Dockerfile
├── Jenkinsfile
├── application.py
├── requirements.txt
├── setup.py
├── README.md
└── mlruns/                    # MLflow tracking folder
```

---

# ✨ Future Improvements

- Add **model drift detection** with **EvidentlyAI**
- Deploy **monitoring dashboards** with **Prometheus + Grafana**
- Setup **model retraining triggers** based on data drift

---

# 🙌 Acknowledgments

Thanks to open-source communities and MLflow, Flask, GCP, and LightGBM contributors.

---

# 🚀 Made by [Ambuj Nayan Mishra]



