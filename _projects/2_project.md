---
layout: page
title: "Theoretical Analysis of Augmented Equilibrium Propagation"
description: Proving gradient-equivalence and characterizing implicit regularization induced by astrocyte-motivated auxiliary state variables in EP dynamics.
img:
importance: 2
category: research
---

Equilibrium Propagation (EP) is a biologically-plausible learning algorithm that computes gradients through the energy difference between free and nudged equilibrium states. This project investigates what happens when EP is augmented with auxiliary state variables motivated by astrocytic neuromodulation.

### Key Results

- **Gradient equivalence**: Proved that the augmented EP contrastive update recovers the standard backpropagation gradient in the appropriate theoretical limit — establishing that the biological augmentation does not break the learning rule's correctness.
- **Implicit regularization**: Characterized how the auxiliary state buffers induce implicit weight regularization in the reduced EP equilibrium landscape. The structure of this regularization distinguishes augmented EP from standard EP even when gradients match in expectation.
- **Finite-rate corrections**: At finite nudging rates, the augmentation introduces a dynamic tracking signal that further separates the learning dynamics from vanilla EP.
- **Neural state invariance**: Proved that the neural state dynamics at equilibrium are unchanged by the augmentation — isolating the effect to the weight update rule only.

### Status

Work in progress; details withheld pending submission.

**Tools:** PyTorch, Python, CUDA
