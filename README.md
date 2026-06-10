# An Encoder-Decoder Approach for Packing Circles

This repository contains implementation codes for the paper:

**"An Encoder-Decoder Approach for Packing Circles"**

---

## Paper Summary

This work studies the classical geometric optimization problem of packing identical circles within a larger circle using a novel neural-network-based encoder-decoder framework.

Circle packing problems arise in several areas including:
- Information theory
- Coding theory
- Wireless communications
- Resource allocation
- Computational geometry

The objective is to place smaller circles completely inside a larger circle while minimizing or avoiding overlap among them. Since overlap constraints are inherently non-convex, obtaining globally optimal solutions is computationally challenging.

This work proposes a learning-based encoder-decoder architecture consisting of:
- Encoder block
- Perturbation block
- Decoder block

The proposed framework operates as follows:
- The encoder receives the index of a circle as input and predicts its center coordinates.
- A normalization layer ensures the predicted center lies within the feasible packing region.
- A perturbation layer introduces controlled perturbations while restricting deviations within the radius of the smaller circle.
- The decoder estimates the intended circle index from the perturbed center coordinates.

Both the encoder and decoder are parameterized using neural networks and jointly optimized to minimize decoding error.

Key contributions include:
- A novel encoder-decoder formulation for geometric packing problems
- Integration of normalization and perturbation layers for feasibility control
- Learning-based generation of circle configurations
- Competitive packing performance compared to classical heuristic methods
- A framework extendable to higher-dimensional and non-circular object packing problems

The proposed approach provides sub-optimal yet computationally efficient packing solutions and demonstrates the applicability of deep learning methods to non-convex geometric optimization problems.

---

## Paper Links

### IEEE
[IEEE Xplore](https://ieeexplore.ieee.org/document/10619689)

