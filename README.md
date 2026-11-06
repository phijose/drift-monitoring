# Introduction

A bank uses an ML model to predict loan default. The world changes — incomes rise, a new customer segment arrives, a recession starts. The model was trained on old data, so it slowly gets worse, and nobody notices. My service serves the model, logs every prediction, and checks every day whether live data still looks like training data. If not, it raises an alert.

Built a model-serving and drift-monitoring service: FastAPI inference API, MLflow tracking and registry, prediction logging in PostgreSQL, per-feature drift detection (PSI) and delayed-label performance tracking with alerts — Dockerized, CI on GitHub Actions, pytest-covered.
