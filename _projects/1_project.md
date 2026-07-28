---
layout: page
title: "STAR: Keeping AI Models Reliable When Hardware Memory Fails"
description: A retraining-based repair method for AI models on memristive hardware that develops permanent faults, needing no extra hardware or fault localization.
img:
importance: 1
category: research
---

Neuromorphic hardware such as memristor crossbars is prone to permanent stuck-at faults that degrade neural network accuracy. Existing approaches typically require fault localization or full model retraining — both expensive in hardware-constrained settings.

**STAR** (astrocyte-inspired STate-Augmented Repair) addresses this by drawing inspiration from astrocytic neuromodulation in biological neural circuits. Astrocytes in the brain detect deviations in population activity and drive compensatory responses; STAR instantiates an analogous mechanism within the Equilibrium Propagation (EP) training framework: before deployment, a compact snapshot of the healthy model's internal states is stored, and after faults appear, this snapshot guides retraining to recover accuracy with no knowledge of which memory cells are broken.

### Key Contributions

- **Class-conditional repair targets**: Pre-fault mean activations are recorded per class and used as repair anchors. These snapshots require **20×–191× less storage** than a full model checkpoint.
- **Augmented EP primitive**: STAR is integrated as an additional nudge term in EP's contrastive phase. The augmented training dynamics are proven to retain fixed-point convergence guarantees under Lipschitz-continuity conditions.
- **Validated recovery**: Achieves **+59%** accuracy recovery over standard retraining on CNN/CIFAR-10 and MLP/MNIST benchmarks, across fault rates up to **90%**, without requiring knowledge of which weights are faulty.

### Publication

Y. A. Khan, Z. Han, A. Sengupta, "STAR: Astrocyte-Inspired State-Augmented Repair for Supervised Memristive AI Hardware Systems," *arXiv:2607.15415*, Jul 2026. [[Link]](https://arxiv.org/abs/2607.15415)

**Tools:** PyTorch, CUDA, Python, VSCode, MobaXterm (remote GPU cluster)
