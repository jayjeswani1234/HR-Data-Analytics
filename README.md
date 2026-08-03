# 📊 AI-Powered HR Analytics Dashboard

An interactive **AI-Powered HR Analytics Dashboard** built using **Python, Streamlit, Pandas, Plotly, and Machine Learning**. The application provides comprehensive workforce analytics, enabling organizations to monitor employee performance, capacity planning, attrition trends, and HR KPIs through an intuitive dashboard.

> **Production-ready deployment with Docker & Kubernetes (Minikube).**

---

## 🚀 Features

- 📊 Interactive Executive Dashboard
- 👥 Workforce Capacity Analysis
- 📉 Employee Attrition Analytics
- 📈 Department-wise Performance Insights
- 🎯 Recruitment & Hiring Metrics
- 👨‍💼 Employee Demographics Analysis
- 🔍 Advanced Search & Filtering
- 📄 CSV-based Data Processing
- 📊 Dynamic Plotly Visualizations
- 🤖 AI & Machine Learning Ready
- 🐳 Dockerized Application
- ☸️ Kubernetes Deployment with Auto Scaling

---

# 🛠 Tech Stack

### Frontend
- Streamlit

### Backend
- Python

### Data Analytics
- Pandas
- NumPy
- Plotly
- Matplotlib

### Machine Learning
- Scikit-learn
- Joblib

### DevOps
- Docker
- Docker Compose
- Kubernetes (Minikube)
- Horizontal Pod Autoscaler (HPA)
- ConfigMap
- Persistent Volume Claim (PVC)
- Ingress
- Network Policies

### Dataset
- HR Employee Dataset (CSV)

---

# 📂 Project Structure

```text
HR-Data-Analytics/
│
├── src/
│   ├── app.py
│   ├── config.py
│   ├── data.py
│   ├── filters.py
│   ├── utils.py
│   ├── tab_summary.py
│   ├── tab_capacity.py
│   ├── tab_attrition.py
│   └── ...
│
├── k8s/
│   ├── namespace.yml
│   ├── deployment.yml
│   ├── service.yml
│   ├── ingress.yml
│   ├── pvc.yml
│   ├── configmap.yml
│   ├── hpa.yml
│   ├── network-policy.yml
│   ├── resourcequota.yml
│   └── priorityclass.yml
│
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
├── README.md
└── assets/
```

---

# 📥 Installation

Clone the repository

```bash
git clone https://github.com/jayjeswani1234/HR-Data-Analytics.git
```

Move into the project

```bash
cd HR-Data-Analytics
```

Create a virtual environment

```bash
python -m venv .venv
```

Activate the environment

### Windows

```bash
.venv\Scripts\activate
```

### Linux / macOS

```bash
source .venv/bin/activate
```

Install dependencies

```bash
pip install -r requirements.txt
```

---

# ▶️ Run the Application

```bash
streamlit run src/app.py
```

The dashboard will be available at:

```
http://localhost:8501
```

---

# 🐳 Docker Deployment

Build the Docker image

```bash
docker build -t hr-dash .
```

Run the container

```bash
docker run -p 8501:8501 hr-dash
```

Open:

```
http://localhost:8501
```

---

# ☸️ Kubernetes Deployment

Start Minikube

```bash
minikube start
```

Load Docker image into Minikube

```bash
minikube image load hr-dash:latest
```

Deploy Kubernetes resources

```bash
kubectl apply -f k8s/
```

Verify resources

```bash
kubectl get all -n hr-dashboard
```

Access the application

```bash
minikube service hr-dashboard-service -n hr-dashboard
```

---

# 📊 Dashboard Modules

### Executive Summary

- Employee Overview
- Workforce KPIs
- Gender Distribution
- Department Distribution

### Capacity Analysis

- Department Capacity
- Resource Allocation
- Employee Utilization
- Workforce Planning

### Attrition Analysis

- Attrition Rate
- High-Risk Departments
- Employee Retention
- Exit Trends

---

# 🤖 Machine Learning

The project is designed to support predictive HR analytics, including:

- Employee Attrition Prediction
- Workforce Trend Analysis
- Performance Prediction
- HR Forecasting

---

# ⚙️ Kubernetes Features

- ✅ Namespace Isolation
- ✅ Multi-Replica Deployment
- ✅ Load Balancing
- ✅ Horizontal Pod Autoscaler
- ✅ ConfigMaps
- ✅ Persistent Volume Claims
- ✅ Resource Quotas
- ✅ Priority Classes
- ✅ Network Policies
- ✅ Ingress Support

---

# 📸 Screenshots

Add screenshots here.

Example:

```
assets/dashboard.png
assets/summary.png
assets/attrition.png
```

---

# 🔮 Future Improvements

- AI HR Assistant
- Resume Screening Integration
- Email Report Generation
- PDF Report Export
- Authentication & RBAC
- PostgreSQL Integration
- Prometheus & Grafana Monitoring
- CI/CD using GitHub Actions
- Helm Chart Deployment
- Cloud Deployment (AWS EKS / Azure AKS / GKE)

---

# 👨‍💻 Author

**Jay Jeswani**

- GitHub: https://github.com/jayjeswani1234
- LinkedIn: https://linkedin.com/in/jayjeswani1234

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

---

# 📄 License

This project is licensed under the MIT License.
