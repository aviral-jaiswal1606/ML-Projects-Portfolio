# Machine Learning Projects Portfolio

A curated collection of beginner to intermediate machine learning projects implemented in Python and developed for reproducibility and learning. Each project is runnable in Google Colab and includes a clear problem statement, data preprocessing, model training, evaluation, and inference examples.

Badges
- Build: ![CI](https://img.shields.io/badge/ci-pending-lightgrey)
- Python: ![Python](https://img.shields.io/badge/python-3.9%2B-blue)
- License: ![MIT](https://img.shields.io/badge/license-MIT-green)

## Overview

This repository contains multiple small projects focusing on classical ML and deep learning techniques applied to real-world problems in healthcare and education. The aim is to provide clean, reproducible notebooks and a minimal example of how to serve a model for inference.

Key goals:
- Clear notebooks that are beginner friendly
- Reproducible environment and CI checks
- Minimal production example (FastAPI + Dockerfile)
- Guidance on testing, linting, and contribution

## Projects (Notebooks)

- Medical Diagnosis
  - Bone Fracture Classification — `Bone_Break_Classification.ipynb`  
    Convolutional Neural Network on X-ray images for fracture detection.
  - Breast Cancer Detection (Logistic Regression) — `Breast_Cancer_Classification_Using_LR.ipynb`  
    Tabular classification using logistic regression and basic model evaluation.
  - Pneumonia Classification — `Pneumonia_classification.ipynb`  
    Binary image classification with CNN architectures.
- Decision Trees & Basic ML
  - Drug Recommendation using Decision Tree — `drugs using decisiton_tree.ipynb`
  - Student Performance Analysis — `Student_data.ipynb`
  - Iris Flower Classification — `iris_flower_classification.ipynb`

(Each notebook contains: objective, dataset description, reproducible preprocessing, model training, evaluation metrics, and inference examples.)

## Quickstart (local)

1. Clone the repo:
   git clone https://github.com/aviral-jaiswal1606/ML-Projects-Portfolio.git
   cd ML-Projects-Portfolio

2. Create a Python virtual environment and activate it:
   python3 -m venv .venv
   source .venv/bin/activate  # macOS / Linux
   .venv\Scripts\activate     # Windows

3. Install dependencies:
   pip install -r requirements.txt

4. Run tests & quality checks:
   pytest
   black --check .
   ruff .

5. Run the example inference app (local):
   cd inference
   uvicorn app:app --reload --host 0.0.0.0 --port 8000

Note: Notebooks are designed for Google Colab and contain cells to fetch datasets from public URLs. Large model artifacts are not stored in the repository; instructions to download or regenerate models are provided in each notebook.

## Development & Contributions

Please read CONTRIBUTING.md for contribution guidelines and CODE_OF_CONDUCT.md for community expectations.

- Style: black + isort + ruff
- Tests: pytest
- Pre-commit: configured to run formatting and basic checks
- CI: GitHub Actions runs tests and linters on pull requests

## Model Card (summary)
See MODEL_CARD.md for dataset sources, intended uses, evaluation metrics, limitations, and ethical considerations.

## Author

Aviral Jaiswal  
Final Year Student | Machine Learning Engineer (early-career)  
LinkedIn: https://www.linkedin.com/in/aviral-jaiswal-9711b12b6/  
Portfolio: https://yourportfolio.com

Short professional blurb:
I build reproducible machine learning projects and clear educational notebooks that bridge theory and practical implementation. My focus is on approachable model development, transparent evaluation, and simple, reproducible deployment examples suitable for learning and small-scale demos.

## License

This project is licensed under the MIT License — see LICENSE for details.
