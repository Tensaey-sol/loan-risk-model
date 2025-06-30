# 📊 Loan Risk Model

This repository contains the implementation of an end-to-end machine learning pipeline for **Loan Risk Model**, a credit risk scoring system developed for a hypothetical bank's buy-now-pay-later service in partnership with an eCommerce platform. The project focuses on building, deploying, and automating a credit risk model using RFM-based proxy variables, feature engineering, and model training, with deployment via FastAPI and CI/CD integration.

---

## 🚀 Getting Started

Follow these steps to set up the project locally:

### 1. Clone the Repository

```bash
git clone https://github.com/Tensaey-sol/loan-risk-model.git
cd loan-risk-model
```

### 2. Set Up a Virtual Environment

```bash
python -m venv .venv
```

Activate it:

- **Windows:**

  ```bash
  .venv\Scripts\activate
  ```

- **macOS/Linux:**

  ```bash
  source .venv/bin/activate
  ```

### 3. Install Dependencies

```bash
pip install --upgrade pip
pip install -r requirements.txt
```

---

## 📂 Project Structure

```
loan-risk-model/
├── .github/
│   └── workflows/
│       └── ci.yml             # GitHub Actions workflow for CI/CD
├── .gitignore                 # Ignore rules for Git
├── requirements.txt           # Project dependencies
├── README.md                  # Project documentation
├── notebooks/                 # Jupyter Notebooks for EDA and experimentation
│   └── README.md
├── tests/                     # Unit tests for scripts and functions
│   └── __init__.py
├── src/                       # Scripts for data processing, feature engineering, and API
│   ├── __init__.py
│   └── README.md
├── data/                      # Raw and processed datasets (ignored via .gitignore)
│   ├── raw/
│   └── processed/
└── .venv/                     # Local virtual environment (ignored via .gitignore)
```

---

## ⚙️ GitHub Actions CI

A CI workflow is configured to run on every push to the main branch:

- Uses **Python 3.x** (specified in `requirements.txt`)
- Installs dependencies from `requirements.txt`
- Runs a linter (e.g., flake8) for code style checks
- Executes unit tests in `/tests` using pytest

See `.github/workflows/ci.yml` for setup and the **Actions** tab of the GitHub repository for its status.

---

## 🛠 Tools & Technologies

- Python **3.13.1**
- `venv` for isolated Python environments
- **VSCode** (Recommended editor)
- Scikit-learn for model training and pipelines
- MLflow for experiment tracking and model registry
- FastAPI and Uvicorn for API deployment
- Docker and docker-compose for containerization
- Xverse and WoE for feature engineering
- Jupyter Notebooks for exploratory data analysis
- Git & GitHub for version control
- GitHub Actions for CI/CD automation
- Pytest for unit testing
- Flake8 or Black for linting

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♀️ Questions or Suggestions?

Feel free to open an issue or submit a pull request if you’d like to contribute or raise a question.
