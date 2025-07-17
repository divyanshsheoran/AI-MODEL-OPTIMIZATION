# AI Model Optimization Project

This project investigates model compression techniques (quantization, pruning, distillation) to optimize large-scale AI models for deployment in resource-constrained environments. The baseline model used is MobileNetV2 on the CIFAR-10 dataset using PyTorch.

Folder Structure:
- notebooks/: Jupyter notebooks for experiments
- scripts/: Python scripts for training and evaluation
- models/: Saved trained models
- results/: Metrics and graphs
- report/: Dissertation docs and notes

## 📊 Experimental Results

| Model                     | Accuracy (%) | Size (MB) | Notes |
|----------------------------|--------------|-----------|-------|
| 🧑‍🏫 Teacher (Baseline)      | **58**       | 9.19      | Best accuracy |
| 📉 Dynamic Quantized        | **58**       | ~9.16     | Same accuracy, negligible size reduction |
| ✂️ Pruned                   | **15.7**     | 18.02     | Failed: masks & no fine-tuning |
| 👶 Student (Knowledge Distillation) | **55.6** | 4.04      | Smaller, reasonable accuracy |

### 📈 Accuracy & Size Comparison


