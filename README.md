# Sales/Demand Forecasting System

A web-based time-series forecasting application that analyses historical sales data and predicts future sales using **ARIMA** and **Prophet** models.

The system provides an interactive dashboard to visualize sales trends, generate forecasts, and compare model performance using standard evaluation metrics.

---

## 📌 Project Overview

Sales forecasting helps businesses estimate future sales based on historical data. It supports better planning and decision-making by identifying trends and patterns in past sales.

The **Sales/Demand Forecasting System** simplifies this process by combining time-series forecasting techniques with an interactive web interface.

Users can work with historical date-wise sales data, generate future predictions using different forecasting models, and evaluate their performance through visualizations and error metrics.

## ✨ Features

- **Historical Sales Analysis** – Work with date-wise historical sales data.
- **ARIMA Forecasting** – Generate predictions using the ARIMA time-series model.
- **Prophet Forecasting** – Generate predictions using the Prophet forecasting model.
- **Forecast Visualization** – View historical and predicted sales through visual representations.
- **Model Comparison** – Compare ARIMA and Prophet performance.
- **Performance Evaluation** – Evaluate models using MAE, RMSE, and MAPE.
- **Interactive Dashboard** – Access forecasting results through a user-friendly interface.

## 🛠️ Technology Stack

| Component | Technologies |
|---|---|
| Frontend | React, TypeScript |
| Backend | Python, FastAPI |
| Forecasting Models | ARIMA, Prophet |
| Data Processing | Python data-analysis libraries |
| Development Tools | Visual Studio Code / PyCharm |

## 🏗️ System Architecture

The application follows a frontend-backend architecture.

1. **Frontend:** React and TypeScript provide the user interface and dashboard.
2. **API Layer:** FastAPI receives requests from the frontend.
3. **Data Processing:** Historical sales data is prepared for forecasting.
4. **Forecasting Engine:** ARIMA and Prophet generate future sales predictions.
5. **Evaluation:** Forecast performance is measured using MAE, RMSE, and MAPE.
6. **Visualization:** Forecasts and evaluation results are presented on the dashboard.

## 📊 Forecasting Models

### 1. ARIMA

ARIMA stands for AutoRegressive Integrated Moving Average.

It is a statistical time-series forecasting model that uses past observations, differencing, and moving-average components to predict future values.

### 2. Prophet

Prophet is a time-series forecasting model designed to capture trends and seasonal patterns in data.

It generates future predictions based on patterns identified in historical observations.

## 📈 Model Performance

The following results were obtained on the evaluated test dataset:

| Evaluation Metric | ARIMA | Prophet |
|---|---:|---:|
| MAE | 19.81 | 16.99 |
| RMSE | 24.14 | 19.49 |
| MAPE | 13.09% | 11.45% |

**Observation:** Prophet achieved lower MAE, RMSE, and MAPE values than ARIMA on the evaluated test dataset.

Lower error values indicate better prediction accuracy for this evaluation period.

## ⚙️ Installation and Setup

### Prerequisites

Make sure the following are installed:

- Python
- Node.js and npm
- Git

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd <project-folder>
```

### 2. Backend Setup

Navigate to the backend directory:

```bash
cd backend
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate the environment.

**Windows:**

```bash
venv\Scripts\activate
```

Install the required dependencies:

```bash
pip install -r requirements.txt
```

Start the FastAPI server (adjust the module path if your entry file has a different name):

```bash
uvicorn main:app --reload
```

The backend API will generally be available at:

```text
http://127.0.0.1:8000
```

FastAPI interactive API documentation:

```text
http://127.0.0.1:8000/docs
```

### 3. Frontend Setup

Open a new terminal and navigate to the frontend directory:

```bash
cd frontend
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Open the local URL displayed in your terminal to access the application.

> Note: The folder names, backend entry-point and available npm scripts should match your actual project structure.

## 📁 Project Structure

A suggested structure for the application:

```text
Sales-Demand-Forecasting-System/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── backend/
│   ├── main.py
│   ├── requirements.txt
│   └── ...
│
├── README.md
└── .gitignore
```

## 🚀 Future Enhancements

- Support for larger historical sales datasets.
- Additional forecasting algorithms.
- Automated model selection.
- Product-wise forecasting when product-level data is available.
- Database integration for storing historical sales records.
- Cloud deployment and improved accessibility.

## 🎯 Project Outcome

The Sales/Demand Forecasting System demonstrates how time-series forecasting techniques can be integrated into a web-based application.

By combining ARIMA and Prophet with an interactive dashboard and model evaluation metrics, the system makes historical sales analysis and future sales prediction easier to understand.


**Project:** Sales/Demand Forecasting System  
**Domain:** Machine Learning | Time-Series Forecasting | Web Development
