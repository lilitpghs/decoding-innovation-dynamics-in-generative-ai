# Decoding Innovation Dynamics in Generative AI
## A Patent-Based Topic Modelling and Diffusion Analysis

### Overview

This project analyzes the innovation landscape of Generative Artificial Intelligence (GenAI) using large-scale patent data. The goal is to uncover latent technological themes, track their evolution over time, and interpret their innovation maturity using the Diffusion of Innovations (DoI) framework.

The study applies and compares multiple topic modeling approaches on GenAI patent abstracts and claims, supported by a domain-specific, fully reproducible preprocessing pipeline designed for patent text.

### Research Questions

The project addresses three core questions:

Which topic modeling methods produce the most coherent and interpretable themes when applied to GenAI patent data?

What are the dominant and emerging innovation themes in Generative AI, and how do they evolve over time?

How can these thematic patterns inform strategic innovation decisions when interpreted through the Diffusion of Innovations framework?

### Data

Source: European Patent Office (Espacenet)

Scope: GenAI patents filed between 2021–2025

Final dataset: 1,570 high-quality patent records

Text fields used: title, abstract, claims

Metadata: publication year, IPC/CPC codes, applicants

A transparent, query-based retrieval strategy was used to ensure precision, recall, and reproducibility.

### Methodology

#### Preprocessing

A multi-stage, domain-adapted preprocessing pipeline was developed, including:

normalization and noise reduction

domain-specific stopword and entity filtering

lemmatization and phrase detection

removal of legal boilerplate common in patent language

This pipeline was specifically designed to improve interpretability in unsupervised topic modeling.

#### Topic Modeling

Four topic modeling approaches were evaluated and compared:

LDA (Latent Dirichlet Allocation)

LSI (Latent Semantic Indexing)

NMF (Non-negative Matrix Factorization)

BERTopic (chunk-based and summary-based variants)

Models were systematically tuned and evaluated using:

topic coherence

topic diversity

composite topic quality metrics

### Key Findings

LDA provided the most interpretable and stable topic structure for innovation analysis, despite BERTopic achieving higher numerical scores.

Six distinct GenAI innovation themes were identified, including:

Language modeling and prompt-based learning

Representation learning and autoencoding

Medical imaging and diagnostic AI

Embedded and signal-based AI systems

Topic lifecycle analysis revealed clear differences between emerging, mature, and declining innovation themes.

Mapping topics to the Diffusion of Innovations framework enabled identification of early-stage versus saturated technological areas and highlighted strategic gaps.

### Contribution

This project contributes by:

providing a comparative evaluation of topic modeling methods on patent data

offering a longitudinal, theme-based view of GenAI innovation

demonstrating how topic modeling can be integrated with diffusion theory to support strategic innovation analysis

Repository Structure
```text
├── README.md          #Project overview
├── notebooks/         # Topic modeling and analysis notebooks
├── preprocessing/     # Text cleaning and preprocessing pipeline
├── results/           # Topic outputs and evaluation metrics
```

Note: raw patent data is not included.

Keywords

Generative AI · Patent Analytics · Topic Modelling · Innovation Dynamics · Diffusion of Innovations · Text Mining · Strategic Technology Analysis
