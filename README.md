# 📊 Graph Datasets for MST and ACO Research

This repository provides two structured datasets of **complete undirected weighted graphs**, intended for benchmarking and experimental analysis in **Minimum Spanning Tree (MST)** and **Ant Colony Optimization (ACO)** algorithms.

---

## 📁 Dataset Overview

The datasets are organized into two categories:

### 1. `dataset_wamiliana/` – Random Graphs (Uncontrolled)
- Contains 30 randomly generated complete graphs for each graph size (10 to 100 vertices).
- Weights are generated without statistical control, resulting in wide variability.
- Useful for testing algorithm robustness under irregular and highly variant input conditions.

**Source Reference**:
> Prof. [Wamiliana](https://scholar.google.com/citations?hl=en&user=v4sjk3cAAAAJ)  
> Universitas Lampung, Indonesia  
> Expertise: Operations Research, Combinatorics, Graph Theory (especially Spanning Tree)  

### 2. `dataset_normalisasi/` – Normalized Graphs (Controlled)
- Also includes 30 instances per graph size (10–100 vertices).
- Edge weights are sampled from **normal distributions** with defined `mean (μ)`, `std deviation (σ)`, and bounded `min-max` values:
  
| Vertex Size | Mean (μ) | Std Dev (σ) | Min Weight | Max Weight |
|-------------|-----------|--------------|-------------|--------------|
| 10–50       | 50        | 10           | 10          | 100          |
| 60–100      | 100       | 20           | 20          | 200          |

- Designed for reproducibility and experimental fairness.
- Ensures consistency in statistical characteristics across all instances.

---

## 📦 File Format

Each `.csv` file contains 30 columns, where each column represents one unique graph instance.  
Each row corresponds to an edge, and contains its respective weight in each instance.

- Number of edges per graph is calculated using:
  
  \[
  E = \frac{n(n-1)}{2}
  \]

  where `n` is the number of vertices.

---

## 🔧 Suggested Usage

You can use these datasets for:

- Benchmarking MST algorithms (e.g., Kruskal, Prim)
- Comparing performance of ACO variants on graph optimization tasks
- Analyzing how input characteristics influence algorithm accuracy and runtime

If you wish to generate your own graphs based on these principles, check the `scripts/` directory (optional).

---

## 🛡️ License

This dataset is made available under the **MIT License**.  
Please cite the original academic reference to Prof. Wamiliana if used in research/publications.

---

## ✍️ Contact

For feedback or collaboration:  
📧 [Your Email]  
🔗 GitHub: [Your Profile Link]

