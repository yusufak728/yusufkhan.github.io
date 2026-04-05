---
layout: page
title: "SRN-C: Astrocyte-Inspired Self-Repair for Fault-Tolerant Neural Networks"
description: A neuroscience-grounded mechanism to recover accuracy in EP-trained networks under permanent synaptic faults, without fault localization.
img:
importance: 1
category: research
---

Neuromorphic hardware such as memristor crossbars is prone to permanent stuck-at faults that degrade neural network accuracy. Existing approaches typically require fault localization or full model retraining — both expensive in hardware-constrained settings.

**SRN-C** (Self-Repair Network — Contrastive) addresses this by drawing inspiration from astrocytic neuromodulation in biological neural circuits. Astrocytes in the brain detect deviations in population activity and drive compensatory responses; SRN-C instantiates an analogous mechanism within the Equilibrium Propagation (EP) training framework.

### Key Contributions

- **Class-conditional repair targets**: Pre-fault mean activations are recorded per class and used as repair anchors. These targets require **20×–191× less storage** than full model checkpoints.
- **Augmented EP primitive**: SRN-C is integrated as an additional nudge term in EP's contrastive phase, with a dedicated repair strength parameter β_r. The augmentation preserves gradient-equivalence with backpropagation in the theoretical limit.
- **Validated recovery**: Accuracy is recovered across fault rates of **50%–90%** on MLP/MNIST and up to **13%** on CNN/CIFAR-10, without requiring knowledge of which weights are faulty.
- **Generalizes to backpropagation**: Repair effectiveness confirmed beyond EP-trained networks.

### Status

Manuscript in preparation.

**Tools:** PyTorch, CUDA, Python, VSCode, MobaXterm (remote GPU cluster)
