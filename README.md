# AIE332 Deep Learning — Assignments and Projects

**Student:** Ahmed Hisham  
**Student ID:** 223106291  
**Course:** Deep Learning AIE 332  
**Supervisor:** Dr. Shaker Elsappagh  
**University:** Galala University

This repository contains the course assignments and the two main deep-learning projects completed for AIE332.

## Repository Contents

### Assignment 1 — CNN on CIFAR-10
Folder: `Assignment_1_CNN_CIFAR10/`

A PyTorch convolutional neural network was implemented and trained on CIFAR-10.

- 10 image classes
- 10 training epochs
- Final training accuracy: **96.13%**
- Test accuracy: **70.83%**

### Assignment 2 — LSTM, GRU & Attention
Folder: `Assignment_2_LSTM_GRU_Attention/`

This assignment uses the UCI Human Activity Recognition dataset with 9 sensor features and compares:

- LSTM
- GRU
- LSTM + Attention
- GRU + Attention

Recorded test accuracies in the notebook:

| Model | Test Accuracy |
|---|---:|
| LSTM | 83.10% |
| GRU | 22.94% |
| LSTM + Attention | 90.87% |
| GRU + Attention | 13.84% |

### Project 1 — Image Classification
Folder: `Project_1_Image_Classification/`

The project uses the Intel Image Classification dataset and compares:

- Custom CNN
- ResNet18 with transfer learning
- Vision Transformer (ViT)

Final test accuracy:

| Model | Test Accuracy | Macro F1 |
|---|---:|---:|
| Custom CNN | 80.30% | 80.56% |
| ResNet18 | 91.00% | 91.16% |
| Vision Transformer | 92.17% | 92.35% |

The Vision Transformer achieved the strongest final result in this project.

### Project 2 — Human Activity and Postural Transition Recognition
Folder: `Project_2_Human_Activity_Recognition/`

This project uses raw smartphone accelerometer and gyroscope signals to classify 12 activities/postural transitions.

Five architectures were evaluated:

- CNN
- LSTM
- GRU
- CNN-LSTM
- Transformer

The best configuration was the **CNN using both accelerometer and gyroscope sensors**.

Final result:

- Test Accuracy: **93.73%**
- Precision: **93.99%**
- Recall: **93.73%**
- Weighted F1: **93.65%**
- Macro F1: **86.76%**
- Trainable Parameters: **44,620**

Sensor ablation:

| Sensor Configuration | Accuracy | Macro F1 |
|---|---:|---:|
| Accelerometer Only | 91.90% | 69.14% |
| Gyroscope Only | 72.23% | 66.89% |
| Both Sensors | 93.73% | 86.76% |

## Notes

- The notebooks contain the original experiment code and recorded outputs.
- Dataset files are **not included** in this repository.
- Some notebooks contain local dataset paths from the original development environment. Update those paths before rerunning on another computer.
- The final Human Activity Recognition report is included in the `report/` folder when available.

## Main Software

PyTorch, torchvision, NumPy, Pandas, Matplotlib, scikit-learn, and Jupyter Notebook.
