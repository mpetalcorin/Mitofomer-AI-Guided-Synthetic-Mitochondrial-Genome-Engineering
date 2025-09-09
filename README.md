# Mitofomer-AI-Guided-Synthetic-Mitochondrial-Genome-Engineering
This repository contains the full code, models, and documentation for Mitofomer, an AI-guided synthetic genome design pipeline for optimizing mitochondrial bioenergetics.

## Abstract

Mitofomer is an AI guided framework that links mitochondrial DNA sequence and multi-omics features to energy phenotypes, ATP, ROS, and OCR. A transformer predicts phenotype scores from encoded sequence windows and multi-omics vectors, a generative module proposes new mitochondrial genome designs, and a composite ranker selects candidates that raise ATP output, reduce ROS signals, and improve oxygen consumption. The platform uses only simulated data in this repository, serving as a transparent demonstration of methods, figures, and expected outputs, with a clear validation plan, worms, human cells, mice, for future real data integration.

A proof of concept platform that unites multi-omics integration, transformer based prediction, generative genome design, and high throughput in silico phenotyping, with clear figures and a data driven graphical abstract ready for reviewers.

> Important note, all datasets in this repository are simulated, the goal is to demonstrate the method and the expected outputs once real data are connected

## Importance

Mitochondria set the pace of cellular life, energy output declines with age and stress, and reactive oxygen species accumulate. Mitofomer shows how an AI system can learn sequence to function rules, propose improved mitochondrial genome designs, and rank candidates that raise ATP, lower ROS, and improve OCR, with an experimental path across worms, human cells, and mice. The purpose is to demonstrate the methodological framework and the type of insights possible when integrating AI-guided synthetic biology into mitochondrial genome engineering.

## Key Features
***•	Multi-Omics Integration***\
Simulated mitochondrial datasets integrating DNA, RNA, proteomics, and metabolic flux features.\
***•	Transformer-Based Prediction (Mitofomer)***\
> AI model predicts three critical phenotypes:\
	    •	ATP Production\
	    •	ROS Accumulation\
	    •	OCR (Oxygen Consumption Rate)\
> 
***•	Generative Genome Design***\
GPT-inspired generative module proposes optimized mitochondrial DNA designs.\
***•	Scoring & Ranking***\
Candidates are ranked using a composite optimization score to prioritize high-ATP, low-ROS designs.\
***•	In Silico High-Throughput Phenotyping***\
Evaluation of engineered mitochondrial genomes across C. elegans, human cells, and mouse models.\
***•	Graphical Abstract***\
A data-driven visualization summarizing the entire Mitofomer pipeline with embedded performance metrics.

## Repository map
<img width="940" height="324" alt="image" src="https://github.com/user-attachments/assets/a1fbee22-02b4-4584-b51f-f909b0ddfacc" />

# Datasheet for Mitofomer Simulated Multi-Omics Dataset

**Dataset Name:** Synthetic Multi-Omics Dataset for Mitochondrial Optimization  
**Version:** 2.0  
**Maintainer:** Mark I.R. Petalcorin  
**Contact:** m.petalcorin@gmail.com 
**Last Updated:** September 2025  

## **1. Motivation**
This dataset was synthetically generated to demonstrate AI-driven mitochondrial bioengineering. It combines **DNA sequence encodings** and **multi-omics features** to simulate mitochondrial function, enabling the training and testing of the **Mitofomer** transformer model.

## **2. Composition**
- **Number of samples:** 10,000 synthetic mitochondrial genome segments  
- **Sequence length:** 300 bp  
- **Omics features per sample:** 50 features  
    - Gene expression levels  
    - Proteomics data  
    - Fluxomics-derived bioenergetics  
- **Phenotypic outputs:**  
    - ATP production efficiency  
    - ROS accumulation  
    - Oxygen consumption rate (OCR)

## **3. Collection Process**
No real biological samples were used. The dataset was simulated using statistical priors derived from publicly available mitochondrial studies and flux balance models.

## **4. Intended Uses**
- Training **Mitofomer** (transformer-based phenotype prediction)
- Benchmarking generative synthetic genome design
- Demonstrating the workflow for AI-guided mitochondrial bioengineering

**Not intended for clinical or diagnostic use.**

## **5. Limitations**
- Entirely simulated data → performance metrics are proof-of-concept only.
- Experimental validation is required before any real-world application.

# Model Card for Mitofomer: AI-Guided Mitochondrial Optimization

**Model Name:** Mitofomer  
**Version:** 2.0  
**Maintainer:** Mark I.R. Petalcorin  
**Contact:** m.petalcorin@gmail.com
**Release Date:** September 2025  

## **1. Model Overview**
Mitofomer is a **transformer-based deep learning framework** trained to predict mitochondrial phenotypes — **ATP production**, **ROS accumulation**, and **OCR efficiency** — from combined DNA sequence encodings and multi-omics inputs.

## **2. Intended Use**
- Predicting mitochondrial bioenergetic performance from genomic and omics profiles.
- Ranking synthetic mitochondrial genome designs.
- Supporting **proof-of-concept** AI-guided engineering pipelines.

**Not approved for clinical decision-making or therapeutic use.**

## **3. Model Details**
- **Architecture:** 4-layer transformer encoder, 8 attention heads, 128-dimensional embeddings.
- **Inputs:**  
    - 300-bp DNA sequences encoded as 6-mers  
    - 50 multi-omics features  
- **Outputs:**  
    - ATP production rate  
    - ROS accumulation  
    - OCR efficiency
- **Training Setup:**  
    - Loss: Mean Squared Error (MSE)  
    - Optimizer: Adam  
    - Train/Test split: 80:20  
    - Hardware: CPU/GPU compatible

## **4. Performance Metrics (Simulated Data)**
| Phenotype         | R² Score | MAE      |
|------------------|----------|----------|
| ATP Prediction   | 0.91     | 2.5 AU   |
| ROS Prediction   | 0.89     | 2.7 AU   |
| OCR Prediction   | 0.87     | 3.1 AU   |

## **5. Ethical Considerations**
This model was trained on **fully simulated datasets**. Any results are **hypothetical** and must be validated in biological experiments before downstream applications.

## **6. Citation**
If you use Mitofomer, please cite:

> Petalcorin, M. I. R. (2025). *Mitofomer: AI-guided synthetic mitochondrial genome optimization using simulated multi-omics datasets*. GitHub Repository.
