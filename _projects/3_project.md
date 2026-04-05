---
layout: page
title: "Sleep Stage Classification from Single-Channel EEG"
description: 5-class sleep staging using engineered EEG features; 96.2% validation accuracy with Ensemble Bagged Trees. Published at ICCCI 2024.
img:
importance: 3
category: research
---

Automatic sleep stage classification from EEG is a clinically important problem. Manual scoring by experts is time-consuming and subjective; single-channel systems are especially challenging due to limited signal information.

This project was completed as a Bachelor's thesis under the supervision of Prof. Omar Farooq at Aligarh Muslim University.

### Approach

Using the publicly available **Sleep-EDF** database, EEG signals were processed and the following features were engineered per epoch:

- **KL Divergence** across EEG sub-bands (delta, theta, alpha, beta)
- **Spectral entropy**
- **Interquartile Range (IQR)** and **Median Absolute Deviation (MAD)**

These features were fed into an **Ensemble Bagged Trees** classifier for 5-class staging (Wake, N1, N2, N3, REM).

### Results

- **96.2% validation accuracy** (Ensemble Bagged Trees)
- **94.9% validation accuracy** (Ensemble Boosted Trees)

The significance of KL Divergence as a discriminative feature across sleep stages was validated and highlighted as a key finding.

### Publication

Y. A. Khan, A. Mahboob, O. Farooq, "Enhancing Sleep-Wake Classification Accuracy: Unveiling the Significance of KL Divergence in EEG Signal Analysis," *ICCCI 2024*.

**Tools:** MATLAB, Python
