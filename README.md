# MLOps Pipeline

A CI/CD pipeline for machine learning projects using GitHub Actions.

## Overview 

This project demonstrates a complete ML pipeline with automated checks including:
- Code linting with flake8
- ML environment verification with PyTorch
- Artifact uploading

## Pipeline Steps

1. **Checkout Code** — Clones the repository onto the runner
2. **Set up Python** — Installs Python 3.10
3. **Install Dependencies** — Installs `torch` and `flake8` from `requirements.txt`
4. **Linter Check** — Runs `flake8` to check code style and syntax
5. **Model Dry Test** — Verifies PyTorch is installed and the ML environment is ready
6. **Upload Project Doc** — Saves `README.md` as a downloadable artifact

## Trigger

The pipeline runs on:
- Every push to any branch **except** `main`
- Every pull request

## Test
