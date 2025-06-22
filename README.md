
# Inventory-Optimization-And-Demand-Forecasting-Using-Machine-Learning-MINOR-1
This project builds an intelligent inventory forecasting system using ARIMA and Random Forest. It preprocesses sales data, predicts future demand, visualizes results, enables user interaction, stores data securely, and collects feedback to continuously improve accuracy and optimize stock levels for better inventory management.

# Project: Inventory Optimization and Demand Forecasting Using Machine Learning ⚙

## Overview
This project provides a web-based application for inventory optimization and demand forecasting, using machine learning algorithms to help businesses make informed decisions on demand forecasting and stock management.

## Table of Contents
1. [Features](#features)
2. [Installation](#installation)
3. [Setup and Configuration](#setup-and-configuration)
4. [Usage](#usage)
5. [Working with the Project](#working-with-the-project)
6. [Models Used](#models-used)
7. [Development Platforms](#development-platforms)
8. [Contributing](#contributing)
9. [License](#license)

## Features
- **User Authentication**: Allows user registration, login, and password reset.
- **Inventory and Demand Forecasting**: Predicts future demand using various forecasting models.
- **Data Visualization**: Provides interactive charts for data analysis.
- **Dark and Light Mode Support**: Adapts to the user’s system theme for a better viewing experience.

## Installation
### Prerequisites
Ensure you have:
- **Python 3.8+**
- **pip** to install required packages

### Step 1: Clone the Repository
```bash
git clone https://github.com/sethuraman-y/INVENTORY-OPTIMIZATION-AND-DEMAND-FORECASTING-USING-MACHINE-LEARNING.git
cd INVENTORY-OPTIMIZATION-AND-DEMAND-FORECASTING-USING-MACHINE-LEARNING
```

### Step 2: Install Required Packages
```bash
pip install -r requirements.txt
```

## Setup and Configuration
### Setting Up Database
This project uses SQLite for managing user accounts. On the first run, it automatically creates `users_data.db` and initializes the required tables.

## Usage
### Step 1: Start the Application
```bash
streamlit run ML_project_main.py
```

### Step 2: Navigate the Application
- Open the browser tab launched by Streamlit.
- Login or register to access forecasting features.

## Working with the Project
### Step 1: User Registration and Login
- **Sign Up** with email, username, and password.
- **Login** using credentials.
- **Reset Password** via email or username input.

### Step 2: Data Upload and Preprocessing
- Upload CSV datasets.
- Automatically handles missing values, scaling, and formatting.

### Step 3: Model Selection and Forecasting
Choose among:
- **Linear Regression**
- **Random Forest**
- **ARIMA**
- **LSTM**
Parameter tuning is available for each model.

### Step 4: Visualizing Forecast Results
- Interactive **Plotly** charts.
- Inventory demand trends and actionable insights.

### Step 5: Make Informed Inventory Decisions
Use predictions to manage stock levels, reduce holding costs, and schedule reorders.

## Models Used
- **Linear Regression**: For basic trend estimation.
- **Random Forest Regressor**: Ensemble method for capturing nonlinear trends.
- **ARIMA**: Statistical time-series model.
- **LSTM**: Deep learning model for time dependencies.

## Development Platforms
### 1. **Visual Studio Code (VS Code)**
Recommended for local development.
```bash
streamlit run ML_project_main.py
```

### 2. **Jupyter Notebook / JupyterLab**
Use for testing model blocks and preprocessing logic.

### 3. **Google Cloud Platform (GCP)**
For online deployment:
```bash
streamlit run ML_project_main.py --server.port <port_number> --server.address 0.0.0.0
```
Ensure firewall rules are set.

### 4. **Google Colab**
For GPU-based model testing:
```python
!pip install streamlit pyngrok
from pyngrok import ngrok
!streamlit run ML_project_main.py &
public_url = ngrok.connect(port="8501")
print(public_url)
```

## Contributing
Contributions are welcome! Steps to contribute:
1. Fork the repository
2. Create a feature branch
3. Commit and push changes
4. Open a pull request

**Project Author: SETHU RAMAN Y**

## License
This project is licensed under the MIT License.
