<div align="center">
  <h1>🧠 AI Dataset Versioning & Evolution Engine</h1>
  <p><strong>Track, Analyze, and Predict Dataset Evolution in ML Workflows</strong></p>
  
  [![Python 3.8+](https://img.shields.io/badge/python-3.8+-blue.svg)](https://www.python.org/downloads/)
  [![FastAPI](https://img.shields.io/badge/FastAPI-0.104.1-009688.svg)](https://fastapi.tiangolo.com/)
  [![React 18](https://img.shields.io/badge/React-18.2.0-61DAFB.svg)](https://reactjs.org/)
  [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
  [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
  [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
  
  <img src="https://img.shields.io/badge/Delta%20Lake-3.0.0-003545.svg" alt="Delta Lake">
  <img src="https://img.shields.io/badge/DVC-3.26.0-13ADC7.svg" alt="DVC">
  <img src="https://img.shields.io/badge/Great%20Expectations-0.17.23-00BFFF.svg" alt="Great Expectations">
  <img src="https://img.shields.io/badge/Gemini%20API-1.0.0-4285F4.svg" alt="Gemini API">
</div>

---

## 📋 Table of Contents
- [Overview](#-overview)
- [Key Features](#-key-features)
- [Why This Project](#-why-this-project)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Quick Start](#-quick-start)
- [API Documentation](#-api-documentation)
- [UI Preview](#-ui-preview)
- [Core Components](#-core-components)
- [Database Schema](#-database-schema)
- [Contributing](#-contributing)
- [License](#-license)
- [Contact](#-contact)

---

## 🎯 Overview

The **AI Dataset Versioning & Evolution Engine** is a comprehensive platform designed to solve one of the most critical challenges in Machine Learning: **managing dataset changes over time**.

In modern ML workflows, datasets constantly evolve through:
- New data additions
- Schema modifications
- Quality improvements
- Feature engineering
- Data cleaning operations

These changes can silently degrade model performance, leading to unexpected failures in production. Our engine provides:

✅ **Complete Version Control** - Track every change in your datasets  
✅ **Schema Evolution Detection** - Automatically identify structural changes  
✅ **Similarity Analysis** - Measure relationships between dataset versions  
✅ **Performance Prediction** - Forecast ML model degradation using AI  
✅ **Data Quality Validation** - Automated checks with Great Expectations  
✅ **Beautiful Dashboard** - Intuitive React UI for monitoring

---

## 🌟 Key Features

### 📊 Dataset Versioning
- **Immutable Versions**: Every dataset upload creates a new immutable version
- **Commit History**: Complete audit trail with commit messages
- **Rollback Support**: Easily revert to previous versions
- **DVC Integration**: Optimized for large datasets (>1GB)
- **Delta Lake**: ACID-compliant storage with time travel

### 🔍 Schema Evolution
- **Automatic Detection**: Identify changes in data structure
- **Change Types**: Detect additions, removals, type changes, and more
- **Impact Analysis**: Understand how schema changes affect models
- **Visual Diff**: Side-by-side comparison of schemas
- **Evolution Timeline**: Track schema changes over time

### 📈 Similarity Analysis
- **Multi-dimensional**: Structural, statistical, content, and semantic similarity
- **Heatmap Visualization**: Visual matrix of version relationships
- **Comparison Engine**: Deep dive into version differences
- **Intelligent Scoring**: AI-powered similarity metrics
- **Version Clustering**: Group similar versions automatically

### 🎯 Performance Prediction
- **AI Integration**: Powered by Google Gemini API
- **Degradation Detection**: Early warning system for performance issues
- **Recommendations**: Actionable insights to prevent degradation
- **Trend Analysis**: Visualize performance over time
- **Metric Tracking**: Accuracy, Precision, Recall, F1, and more

### ✅ Data Quality Validation
- **Great Expectations**: Enterprise-grade validation framework
- **Custom Rules**: Define your own validation criteria
- **Automated Reporting**: Detailed quality reports
- **Quality Score**: Overall data quality metric
- **Issue Tracking**: Identify and track data quality issues

---

## ❓ Why This Project

### The Problem

---

## 🛠️ Tech Stack

### Backend
| Component | Technology | Purpose |
|-----------|------------|---------|
| **Framework** | FastAPI | REST API with automatic documentation |
| **Language** | Python 3.8+ | Primary programming language |
| **Database** | SQLite/PostgreSQL | Metadata and version tracking |
| **Data Lake** | Delta Lake | Versioned data storage with ACID |
| **Version Control** | DVC | Large file versioning |
| **Validation** | Great Expectations | Data quality framework |
| **ML/AI** | scikit-learn, TensorFlow | Similarity and prediction models |
| **AI Integration** | Gemini API | Performance prediction & insights |
| **Processing** | Pandas, NumPy | Data manipulation |
| **Migration** | Alembic | Database schema migration |
| **Server** | Uvicorn | ASGI server |

### Frontend
| Component | Technology | Purpose |
|-----------|------------|---------|
| **Framework** | React 18 | UI library |
| **Styling** | Tailwind CSS | Modern, responsive styling |
| **Charts** | Recharts | Data visualization |
| **Routing** | React Router 6 | Navigation |
| **HTTP** | Axios | API communication |
| **State** | React Context | Global state management |
| **Icons** | Heroicons, FontAwesome | Beautiful icons |
| **Build Tool** | Vite | Fast development server |

### DevOps
| Tool | Purpose |
|------|---------|
| **Docker** | Containerization |
| **Docker Compose** | Multi-container orchestration |
| **GitHub Actions** | CI/CD pipeline |
| **Git** | Version control |

---

## 📁 Project Structure

---

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- Node.js 16+
- Git
- Docker (optional)

### Installation

#### 1. Clone the Repository

```bash
git clone https://github.com/vishakha2121/dataset-evolution-engine.git
cd dataset-evolution-engine

# Navigate to backend
cd backend

# Create virtual environment
python -m venv venv

# Activate virtual environment
# On Windows:
venv\Scripts\activate
# On Mac/Linux:
source venv/bin/activate

# Install dependencies
pip install -r requirements.txt

# Set up environment variables
cp .env.example .env
# Edit .env with your configurations

# Initialize database
cd ../database
python init_db.py

# Run backend server
cd ../backend
uvicorn app.main:app --reload

# Navigate to frontend
cd frontend

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env
# Edit .env with your configurations

# Run development server
npm run dev