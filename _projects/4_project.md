---
layout: page
title: "EMG-Based Prosthetic Control System"
description: Real-time EMG prosthetic control with biofeedback rehabilitation loop using residual muscle signals from a MuscleBioAmp sensor and Arduino UNO.
img:
importance: 4
category: research
---

This project developed a real-time electromyography (EMG)-based prosthetic control system aimed at enabling natural, effort-minimized control for amputees and supporting rehabilitation.

### System Design

- **Sensing**: MuscleBioAmp BisCute sensor captures surface EMG signals from residual muscles.
- **Processing**: Arduino UNO reads and processes the EMG signal in real time.
- **Control**: Decoded muscle intent drives prosthetic actuation, minimizing the physical effort required from the user.
- **Biofeedback loop**: A rehabilitation loop was implemented using residual muscle signals to provide feedback during recovery, supporting both assistive mobility and motor re-learning.

### Motivation

Conventional prosthetics often require significant residual limb strength. This system targets patients in rehabilitation where residual muscle activity is weak, using biofeedback to gradually restore control while enabling functional use of the prosthetic.

**Tools:** Arduino UNO, MuscleBioAmp BisCute sensor, Python
