# ☁️ Google Cloud Cost & Usage Analysis (EDA)

A comprehensive **Exploratory Data Analysis (EDA)** of a **Google Cloud billing dataset** using Python, Pandas, Plotly, Seaborn, and Matplotlib to uncover insights around **cloud spending patterns, service-level cost distribution, regional usage, and network data transfer behavior**.

---

# 🌟 Features

## Core Features

- **Data Cleaning & Preprocessing:** Data type standardization and validation of cost and usage metrics.
- **Service-Level Cost Analysis:** Identifying which Google Cloud services contribute the most to overall spending.
- **Regional Spending Analysis:** Understanding how cloud costs vary across different regions.
- **Usage & Data Transfer Analysis:** Evaluating network data transfer patterns and high data usage services.
- **Cost Optimization Insights:** Highlighting high-cost services and infrastructure areas for potential optimization.
- **Visualization:** Interactive and static plots using Plotly, Seaborn, and Matplotlib.

---

# 🗂 Project Structure

The project folder is organized as follows:

```text
Google_Cloud_Cost_EDA/
├── data
|    ├── gcp.csv               # Google Cloud billing dataset
├── Google_Cloud_EDA.ipynb     # Jupyter Notebook with full EDA
├── requirements.txt           # Python dependencies
└── venv/                      # Virtual environment
```

---

# 🏗️ EDA Architecture

```text
+---------------------------+
|        DATA LAYER         |
|  Google Cloud Billing     |
|      Dataset (CSV)        |
+------------+--------------+
             ↓
+------------------------------+
|       ANALYSIS LAYER         |
|  - Data Cleaning             |
|  - Cost Distribution         |
|  - Service-level Analysis    |
|  - Regional Cost Analysis    |
|  - Data Transfer Analysis    |
|  - Usage Pattern Insights    |
+------------+-----------------+
             ↓
+---------------------------------------+
|      VISUALIZATION LAYER              |
|  - Interactive Charts (Plotly)        |
|  - Static Plots (Seaborn & Matplotlib)|
|  - Bar Charts, Histograms, Boxplots   |
+---------------------------------------+
```

---

# 🛠 Tech Stack

- **Language:** Python 3.8+
- **Libraries:**

  - **Data Manipulation:** Pandas, NumPy
  - **Visualization:** Matplotlib, Seaborn, Plotly

- **Environment:** Jupyter Notebook
- **Data Source:** Google Cloud Billing / Cloud Cost Dataset

---

# 📊 Dataset Overview
**Columns include:**
- **Resource ID**: Unique identifier for the GCP resource being used. (Text)  
- **Service Name**: Name of the Google Cloud service (e.g., Compute Engine, Cloud Storage) associated with the usage. (Text)  
- **Usage Quantity**: Amount of the resource consumed during the billing period (e.g., VM hours, GB of storage). (Numeric)  
- **Usage Unit**: Unit in which the resource usage is measured (e.g., hours, GB, requests). (Text)  
- **Region/Zone**: Geographic region or zone where the resource is located (e.g., `us-central1`, `asia-south1`). (Text)  
- **CPU Utilization (%)**: Average CPU usage percentage for the resource during the billing period. (Numeric)  
- **Memory Utilization (%)**: Average memory usage percentage for the resource during the billing period. (Numeric)  
- **Network Inbound Data (Bytes)**: Amount of incoming network traffic in bytes. (Numeric)  
- **Network Outbound Data (Bytes)**: Amount of outgoing network traffic in bytes. (Numeric)  
- **Usage Start Date**: Start date of the usage period. (Date)  
- **Usage End Date**: End date of the usage period. (Date)  
- **Cost per Quantity ($)**: Price of a single unit of the resource. (Numeric)  
- **Unrounded Cost ($)**: Raw cost calculated before rounding. (Numeric)  
- **Rounded Cost ($)**: Cost rounded to the nearest cent. (Numeric)  
- **Total Cost (INR)**: Total cost of the resource usage converted to Indian Rupees. (Numeric)

**Dataset Source:** [Kaggle – GCP Dataset](https://www.kaggle.com/datasets/sairamn19/gcp-cloud-billing-data)
---

## Context

This dataset represents **Google Cloud Platform (GCP) resource usage and billing information** across multiple services, regions, and infrastructure components.

It captures **resource utilization metrics (CPU, memory, network traffic)** along with **billing data**, enabling analysis of:

- Cloud service cost distribution
- Resource utilization efficiency
- Regional infrastructure spending
- Network traffic patterns
- Potential cost optimization opportunities

Such analysis helps organizations **identify underutilized resources, monitor cloud spending, and improve infrastructure efficiency.**

---

## Inspiration

Cloud cost management is a critical aspect of modern infrastructure operations. By analyzing **usage patterns, service-level costs, and resource utilization**, organizations can:

- Reduce unnecessary infrastructure spending  
- Improve resource allocation efficiency  
- Optimize cloud workloads  
- Build cost-aware cloud architectures

---

# 🚀 Quick Start

## 1. Clone Repository

```bash
git clone https://github.com/TejasMJ/Google_Cloud_Cost_EDA.git
```

---

## 2. Create Virtual Environment

```bash
python -m venv venv
```

---

## 3. Activate Virtual Environment

### Windows

```bash
.\venv\Scripts\activate
```

### Mac/Linux

```bash
source venv/bin/activate
```

---

## 4. Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 5. Run Notebook

```bash
jupyter notebook
```

---

# 📊 Cloud Cost Analysis Project

## Key Analyses Performed

### Service Cost Analysis

- Cost distribution across Google Cloud services
- Identification of highest cost services
- Average cost per service

### Regional Cost Analysis

- Cloud spending patterns across regions
- Identification of regions with higher infrastructure costs
- Average spending per region

### Usage & Data Transfer Analysis

- Network data transfer distribution
- Identification of services with high outgoing data traffic
- Conversion of usage metrics (Bytes → GB)

### Cost Concentration Analysis

- Detection of services driving a large share of cloud spending
- Identification of potential optimization areas

### Visualization

- Interactive dashboards using **Plotly**
- Static plots using **Seaborn** and **Matplotlib**

---

# 👨‍💻 Author

**Tejas Jadhav**

- GitHub: [@TejasMJ](https://github.com/TejasMJ)
- LinkedIn: [Tejas Jadhav](https://www.linkedin.com/in/tejas-m-jadhav/)
