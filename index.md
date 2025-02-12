---
title: "HybriDNA Project Demo"
theme: minima
markdown: kramdown
---

# HybriDNA

## A Hybrid Transformer-Mamba2 Long-Range DNA Language Model

[Read the Full Paper](#)

## 📄 Abstract

Advances in natural language processing and large language models have sparked growing interest in modeling DNA, often referred to as the “language of life”. However, DNA modeling poses unique challenges. First, it requires the ability to process ultra-long DNA sequences while preserving single-nucleotide resolution, as individual nucleotides play a critical role in DNA function. Second, success in this domain requires excelling at both generative and understanding tasks: generative tasks hold potential for therapeutic and industrial applications, while understanding tasks provide crucial insights into biological mechanisms and diseases. To address these challenges, we propose HybriDNA, a decoder-only DNA language model that incorporates a hybrid Transformer-Mamba2 architecture, seamlessly integrating the strengths of attention mechanisms with selective state-space models. This hybrid design enables HybriDNA to efficiently process DNA sequences up to 131kb in length with single-nucleotide resolution. HybriDNA achieves state-of-the-art performance across 33 DNA understanding datasets curated from the BEND, GUE, and LRB benchmarks, and demonstrates exceptional capability in generating synthetic cis-regulatory elements (CREs) with desired properties. Furthermore, we show that HybriDNA adheres to expected scaling laws, with performance improving consistently as the model scales from 300M to 3B and 7B parameters. These findings underscore HybriDNA’s versatility and its potential to advance DNA research and applications, paving the way for innovations in understanding and engineering the “language of life”.

Key Highlights:
- Processes sequences up to 131kb
- Combines Transformer and Mamba2 blocks
- Echo Embedding for understanding fine-tuning
- Achieves SOTA performance on BEND, GUE, LRB benchmarks
- Generative ability to design various functional sequence



---

## 🧪 Benchmark Results

### **GUE Benchmark**

![image](gue.png)

### **BEND Benchmark**

![image](bend.png)

**LRB Benchmark**

![image](lrb.png)

---

## 🧬 DNA Generation

### **Synthetic cis-regulatory elements (CREs)**

HybriDNA demonstrates exceptional proficiency in generating synthetic CREs with desired functional properties:

- **Human Enhancers:** 

![image](human_enhancer.png)

- **Yeast Promoters:

![image](yeast_promoter.png)

---

## 🏗️ Architecture Details

HybriDNA is a hybrid DNA language model that integrates:
- **Transformer Attention Mechanisms:** Enhances focus on fine-grained details.
- **Mamba2 Selective State-Space Models:** Efficiently processes long sequences.

This hybrid design enables HybriDNA to process sequences up to 131kb with single-nucleotide resolution.

![image](detail_architect.png)

---

## ⚙️ Methodology

1. **Pretraining:** Multi-species genomes using next-token prediction.
2. **Fine-tuning:** Echo embedding for understanding tasks.
3. **Generative Modeling:** Task-specific prompts for synthetic DNA design.

![image](pipeline.png)

---

## 📬 Contact

For inquiries, please reach out to the **HybriDNA Team** at mamq@umich.edu

---

_This demo is powered by GitHub Pages & Jekyll._
