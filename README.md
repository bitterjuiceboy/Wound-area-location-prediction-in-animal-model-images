# Wound Area Location Prediction

Machine learning models for predicting wound locations in animal model images using Random Forest and XGBoost.

## Overview

Predicts bounding box coordinates (x, y, width, height) of wound areas in images using regression models.

## Models

- **Random Forest**: 100 estimators with label normalization
- **XGBoost**: 100 rounds with 5x data augmentation

## Usage

```bash
# Training
python train_rf.py
python train_xgboost.py

# Testing
python test_rf.py
python test_xgboost.py
```

## Requirements

```
numpy, scikit-learn, xgboost, torch, torchvision, PIL, matplotlib, shapely
```

## Files

- `train_*.py` / `test_*.py` - Training and testing scripts
- `model_rf.sav` / `model_xgboost.json` - Trained models
- `Wound/` - Dataset directory

## Evaluation Metrics

- Mean Squared Error (MSE)
- Overlap ratio
- Error distribution analysis

---

*CISC3023 Project 2024*
```
