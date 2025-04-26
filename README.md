# 📍 Project Overview

This project predicts whether a hotel reservation will be **canceled or honored** based on booking details.  
It is built using a complete **MLOps pipeline**, covering model training, tracking, versioning, containerization, CI/CD automation, and cloud deployment.

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

```mermaid
flowchart TD
A[Data Ingestion] --> B[Data Processing & Feature Engineering]
B --> C[Model Training (LightGBM)]
C --> D[Experiment Tracking with MLflow]
D --> E[Model Saving and Versioning]
E --> F[Containerization with Docker]
F --> G[CI/CD Automation with Jenkins]
G --> H[Deployment on Google Cloud Run]
