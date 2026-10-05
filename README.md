# internship2026-JAP

# Does a skin lesion classifier work equally for everyone?
Fairness audit of an EfficientNet-B0 model on HAM10000 (Kaggle).

## Dataset
https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000

## Method
Lesion-level train/val/test split, class-weighted loss, transfer learning
(ResNet18 / ResNet50 / EfficientNet-B0), per-group evaluation (sex, age, estimated skin tone).

## Key results
Accuracy 0.79, macro F1 0.66, melanoma recall 0.59.

## Limitations
Almost all patients have lighter skin; ITA skin-tone estimate was unreliable; small groups give wide intervals.

## How to run
Open the notebook on Kaggle, attach the dataset above, and Run All (GPU on).
