# Constrained Black-Box Optimization for DNN Accelerators

## Overview
This repository contains the research draft and supplementary materials for a novel hardware design optimization framework. The project addresses the inefficiencies of traditional cycle-level simulation by proposing a **decoupled, data-driven approach** to constrained black-box optimization in discrete hardware design spaces.

Key contributions include:
*   **Decoupled Learning Framework:** Separates objective prediction from constraint learning using Optimization with Constraint Learning (OCL) to avoid optimization conflicts.
*   **Discrete-Space Conservative Training:** Replaces gradient-based negative sampling with Genetic Algorithms (GA) and adaptive penalty functions to handle non-smooth, high-infeasibility hardware landscapes.
*   **Semantic-Aware Embeddings:** Utilizes contrastive learning to construct task-oriented embedding spaces where semantic distance correlates with latency similarity, improving negative sample matching.
*   **Evolutionary Multi-Task Optimization:** Leverages shared parameter spaces across different DNN models (e.g., MobileNetV2, U-Net) to accelerate convergence and improve solution quality via implicit knowledge transfer.

## Document Contents
The uploaded `Draft.pdf` covers the following sections:
1.  **Research Background & Problem Statement:** Limitations of existing offline methods (PRIME, COMs) and traditional simulation workflows.
2.  **Core Technical Contributions:** Detailed methodology on decoupled loss functions, GA-based search, and semantic embeddings.
3.  **Future Work:** Extension to evolutionary multi-task optimization and validation on open-source dataflow architectures (MAESTRO, NVDLA, ShiDianNao).
4.  **Summary & Outlook:** Current achievements (Kendall’s Tau 0.7–0.8) and next-step roadmap.

## Key Terminology
*   **DNN Accelerator:** Specialized hardware for deep neural network inference.
*   **Black-Box Optimization:** Optimizing objectives without explicit mathematical formulations, relying on expensive simulations.
*   **Chance-Constrained Multiple-Choice Knapsack Problem:** The formal problem definition underlying the resource allocation and design selection process.
*   **Surrogate Model:** Transformer + Mixture-of-Experts architecture used to predict hardware performance metrics.

## Status
🚧 **Work in Progress**  
Current focus: Integrating MAESTRO-based evaluation and implementing the multi-task optimization module.
