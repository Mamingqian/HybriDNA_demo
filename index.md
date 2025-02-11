---
title: "HybriDNA Project Demo"
theme: minima
markdown: kramdown
---

# Welcome to HybriDNA Demo

## 🚀 Project Overview

**HybriDNA: A Hybrid Transformer-Mamba2 Long-Range DNA Language Model**

Submitted to **MLGenX Workshop at ICLR 2025**

HybriDNA is a cutting-edge DNA language model designed to address the unique challenges of DNA modeling. It integrates Transformer attention mechanisms with Mamba2 selective state-space models to efficiently process ultra-long DNA sequences with single-nucleotide resolution.

---

## 📄 Abstract

DNA modeling requires handling ultra-long sequences while maintaining single-nucleotide resolution. HybriDNA excels in both generative and understanding tasks through a hybrid architecture, enabling state-of-the-art performance across 33 DNA datasets.

Key Highlights:
- Processes sequences up to 131kb
- Combines Transformer and Mamba2 blocks
- Achieves SOTA performance on BEND, GUE, LRB benchmarks

[Read the Full Paper](#)

---

## 🧪 Model Results

### **GUE Benchmark**

| Model               | Promoter Detection (MCC) | Core Promoter Detection (MCC) |
|---------------------|--------------------------|-------------------------------|
| HybriDNA-300M       | 83.29                    | 68.87                         |
| HybriDNA-3B         | 85.40                    | 69.50                         |
| HybriDNA-7B         | 86.53                    | 71.37                         |

### **LRB Benchmark**

| Model               | Causal eQTL (AUROC) | OMIM (AUPRC) |
|---------------------|---------------------|--------------|
| HybriDNA-300M       | 0.74                | 0.003        |
| HybriDNA-7B         | 0.88                | 0.003        |

---

## ⚡ Try the Model

Enter your DNA sequence below to get the predicted output:

<form method="GET" action="">
  <input type="text" name="sequence" placeholder="Enter DNA sequence" />
  <button type="submit">Predict Fitness</button>
</form>

{% if page.sequence %}
**Predicted Output:** {{ page.sequence | upcase }}
{% endif %}

---

## 🔍 Applications

- **DNA Understanding:** Transcription factor binding, promoter detection
- **DNA Generation:** Designing synthetic cis-regulatory elements (CREs)
- **Scalability:** Performance improves from 300M to 7B parameters

---

## 📬 Contact

For inquiries, please reach out to the **HybriDNA Team** at [email@example.com](mailto:email@example.com).

---

_This demo is powered by GitHub Pages & Jekyll._
