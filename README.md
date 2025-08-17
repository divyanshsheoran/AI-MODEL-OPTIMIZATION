# AI Model Optimization Project

This project explores model compression techniques — Quantization, Pruning, and Knowledge Distillation — to optimize deep learning models for deployment in resource-constrained environments.
We experimented with MobileNetV2 and MobileNetV3 on the CIFAR-10 dataset using PyTorch.

Folder Structure:
- notebooks/: Jupyter notebooks for experiments
- scripts/: Python scripts for training and evaluation
- models/: Saved trained models
- results/: Metrics and graphs
- report/: Dissertation docs and notes

## 📊 Experimental Results

| Model                          | Accuracy (%) | Size (MB) | Notes                                  |
| ------------------------------ | ------------ | --------- | -------------------------------------- |
|  MobileNetV2 Baseline          | **58.26**    | 9.19      | Standard training                      |
|  MobileNetV2 Dynamic Quantized | **58.26**    | 9.19      | Same accuracy, negligible reduction    |
|  MobileNetV2 Pruned            | **13.70**    | 18.02     | Failed: no fine-tuning, size increased |
|  MobileNetV2 Student (KD)      | **49.78**    | 4.04      | Reduced size, accuracy drop            |
|  MobileNetV3 Baseline          | **89.51**    | 6.25      | Data augmentation boosted accuracy     |
|  MobileNetV3 Dynamic Quantized | **89.50**    | 4.45      | Maintained accuracy, \~29% smaller     |

