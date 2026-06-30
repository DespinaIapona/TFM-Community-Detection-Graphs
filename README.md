# Clustering and Community Detection in Graphs

**Master's Thesis** | Universidad Carlos III de Madrid | 2026

**Author:** Despoina Iapona  
**Supervisor:** Prof. Francisco Temprano García

## Overview

This repository contains Python code for the Master's thesis on community detection in graphs. 
We implement and compare four community detection algorithms across different network types.

## Algorithms Implemented

- **Louvain** - Modularity optimization
- **Infomap** - Information-theoretic approach
- **Walktrap** - Random walk-based method
- **Leiden** - Improved version of Louvain

## Networks Tested

1. **Karate Club** - Small undirected network with ground truth
2. **Wikipedia Vote** - Large directed network
3. **LFR Benchmark** - Synthetic networks with controlled parameters
4. **Les Misérables** - Weighted character network
5. **Southern Women** - Bipartite network
6. **UC Irvine College Messages** - Real directed network

## Project Structure
 1) notebooks/        # Jupyter notebooks with full analysis
 2) code/             # Python scripts (cleaner versions)
 3) README.md         # This file

## Requirements
networkx
matplotlib
numpy
cdlib
scipy

Install with:
```bash
pip install -r requirements.txt
```

## Usage

### Run in Google Colab

Each notebook can be run directly in Google Colab by clicking the link in the notebook header.

### Run Locally

```python
python code/karate_club.py
python code/wikipedia_vote.py
# ... etc
```

## Key Findings

- **Infomap** performs best on strong communities but collapses on weak structures
- **Walktrap** is the most robust across difficult cases
- **Leiden** provides higher quality communities than Louvain
- **Direction matters** - directional information significantly affects results
- **Small networks and dense networks** are challenging for all algorithms

## Thesis Structure

See the full thesis for:
- Detailed theoretical background (Chapter 2)
- Algorithm descriptions and optimization approaches (Chapter 3)
- Comprehensive experimental results (Chapter 4)
- Real-world applications analysis (Chapter 5)
- Survey network methodology (Chapter 6)

