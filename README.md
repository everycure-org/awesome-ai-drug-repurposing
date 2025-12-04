[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# Awesome AI Drug Repurposing

A comprehensive collection of AI and machine learning achievements in drug repurposing—identifying new therapeutic uses for existing drugs.

> Drug repurposing is the process of identifying new therapeutic uses for existing drugs (or drug candidates) that were originally developed for a different condition. AI and machine learning are transforming this field by revealing new therapeutic targets and mechanisms, with 30% of repurposed drugs making it to patients compared to just 10% success rate for traditional drug discovery.

**Note:** This list is organized by importance and impact (top-down) rather than alphabetically, highlighting the most significant contributions first within each section.

## Table of Contents

1. [Clinical Successes & Real-World Impact](#clinical-successes--real-world-impact)
2. [Landmark Methods & Foundation Models](#landmark-methods--foundation-models)
3. [Knowledge Graph-Based Methods](#knowledge-graph-based-methods)
4. [Deep Learning & Generative AI](#deep-learning--generative-ai)
5. [Natural Language Processing & Text Mining](#natural-language-processing--text-mining)
6. [Network Medicine & Systems Biology](#network-medicine--systems-biology)
7. [Single-Cell & Transcriptomics Approaches](#single-cell--transcriptomics-approaches)
8. [Data Resources & Knowledge Graphs](#data-resources--knowledge-graphs)
9. [Databases & Compound Libraries](#databases--compound-libraries)
10. [Benchmarks & Challenges](#benchmarks--challenges)
11. [Tools & Software Libraries](#tools--software-libraries)
12. [Key Research Organizations & Labs](#key-research-organizations--labs)
13. [Comprehensive Reviews](#comprehensive-reviews)

---

## Clinical Successes & Real-World Impact

Real-world validation of AI-driven drug repurposing showing clinical impact and FDA approvals.

* **Baricitinib for COVID-19 (BenevolentAI)** - First major AI-driven drug repurposing clinical success
  * Originally approved for rheumatoid arthritis, repurposed for COVID-19 using knowledge graph and ML
  * Identified in 48 hours, received FDA Emergency Use Authorization
  * Clinical trials (ACTT-2, CoV-BARRIER) confirmed significant mortality reduction
  * [Paper (Frontiers in Pharmacology)](https://www.frontiersin.org/journals/pharmacology/articles/10.3389/fphar.2021.709856/full) | [Paper (The Lancet)](https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)30304-4/fulltext)
  * Organizations: BenevolentAI, Eli Lilly

* **ISM001-055/Rentosertib for Idiopathic Pulmonary Fibrosis (Insilico Medicine)** - First AI-designed drug with positive Phase IIa results
  * First-in-class TNIK inhibitor discovered using end-to-end generative AI
  * AI-discovered novel target AND novel molecule
  * Phase IIa (2024): 98.4 mL improvement in lung function vs -62.3 mL decline in placebo
  * From target discovery to Phase 1 in under 30 months (half the traditional time)
  * Received USAN name - landmark achievement for AI drug discovery
  * [Paper/News (Insilico Medicine)](https://insilico.com/news/tnik-ipf-phase2a) | [Paper (PR Newswire)](https://www.prnewswire.com/news-releases/insilico-medicine-reports-positive-phase-iia-results-for-ism001-055-a-novel-first-in-class-drug-treatment-for-idiopathic-pulmonary-fibrosis-ipf-designed-using-generative-ai-302251732.html)
  * Organizations: Insilico Medicine

* **Sulindac for Fragile X Syndrome (HealX)** - AI-discovered repurposing with IND approval
  * NSAID repurposed for rare genetic disease
  * FDA IND approval for Phase 2a clinical trial (2021)
  * Organizations: HealX

* **REC-994 for Cerebral Cavernous Malformation (Recursion Pharmaceuticals)** - Phenomics-driven drug rescue
  * Previously "shelved" compound identified by AI phenomics platform
  * Advanced to Phase II trial
  * Organizations: Recursion Pharmaceuticals

* **ARPA-H MATRIX Project** - $48M investment in AI drug repurposing for rare diseases
  * Led by Every Cure (non-profit)
  * Systematic evaluation of approved drugs across rare diseases
  * [News (ARPA-H)](https://arpa-h.gov/news-and-events/arpa-h-awards-ai-driven-project-repurpose-approved-medications)
  * Organizations: Every Cure, ARPA-H

---

## Landmark Methods & Foundation Models

Breakthrough approaches and foundation models that are reshaping drug repurposing.

* **TxGNN: Zero-Shot Drug Repurposing Foundation Model**
  * Authors: Kexin Huang, Payal Chandak, Qianwen Wang, Shreyas Havaldar, Akhil Vaid, Jure Leskovec, Girish N. Nadkarni, Benjamin S. Glicksberg, Nils Gehlenborg, Marinka Zitnik
  * Graph neural network foundation model trained on medical knowledge graph covering 17,080 diseases
  * First model developed specifically for rare diseases and conditions with no treatments
  * Improves prediction accuracy by 49.2% for indications and 35.1% for contraindications
  * Zero-shot learning enables predictions for diseases with limited treatment options
  * [Paper (Nature Medicine, 2024)](https://www.nature.com/articles/s41591-024-03233-x) | [Code](https://github.com/mims-harvard/TxGNN) | [Project Page](https://zitniklab.hms.harvard.edu/projects/TxGNN/)
  * Organizations: Harvard Medical School, MIMS Harvard, Mount Sinai

* **AlphaFold 2 & 3 for Structure-Based Drug Repurposing**
  * Revolutionary protein structure prediction enabling structure-based drug repurposing
  * AlphaFold 3 extends to protein-ligand, protein-DNA/RNA, and post-translational modifications
  * Enables identification of novel targets for known drugs via structural similarity
  * Accelerates identification of new therapeutic applications through pocket-fitting ligand generation
  * [Review (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC11292590/) | [Paper (Isomorphic Labs)](https://www.isomorphiclabs.com/articles/rational-drug-design-with-alphafold-3)
  * Organizations: DeepMind/Google, Isomorphic Labs

* **Hetionet: Systematic Biomedical Knowledge Integration**
  * Authors: Daniel Scott Himmelstein, Antoine Lizee, Christine Hessler, Leo Brueggeman, Sabrina L Chen, Dexter Hadley, Ari Green, Pouya Khankhanian, Sergio E Baranzini
  * Integrative network connecting drugs, diseases, genes, anatomies, pathways, and more
  * Pioneering work in computational drug repurposing using heterogeneous networks
  * Open science approach with full data and code availability
  * [Paper (eLife, 2017)](https://elifesciences.org/articles/26726) | [Code](https://github.com/hetio/hetionet)
  * Organizations: University of California San Francisco

* **mediKanren: Precision Medicine for Rare Diseases**
  * Authors: Aleksandra Foksinska, Camerron M Crowder, Andrew B Crouse, Jeff Henrikson, William E Byrd, Gregory Rosenblatt, Michael J Patton, Kaiwen He, Thi K Tran-Nguyen, Marissa Zheng, Stephen A Ramsey, Nada Amin, John Osborne, UAB Precision Medicine Institute, Matthew Might
  * Biomedical reasoning system for ultra-rare diseases
  * Combines knowledge graphs with logical reasoning
  * [Paper (PubMed)](https://pubmed.ncbi.nlm.nih.gov/36248623/) | [Code](https://github.com/webyrd/mediKanren)
  * Organizations: University of Alabama at Birmingham, Oregon State University

---

## Knowledge Graph-Based Methods

Methods leveraging knowledge graphs to discover drug-disease relationships.

### Graph Neural Networks (GNNs)

* **TxGNN: A foundation model for clinician-centered drug repurposing**
  * Authors: Kexin Huang, Payal Chandak, Qianwen Wang, Shreyas Havaldar, Akhil Vaid, Jure Leskovec, Girish N. Nadkarni, Benjamin S. Glicksberg, Nils Gehlenborg, Marinka Zitnik
  * [Paper (Nature Medicine, 2024)](https://www.nature.com/articles/s41591-024-03233-x) | [Code](https://github.com/mims-harvard/TxGNN)
  * Organizations: Harvard Medical School

* **DBR-X: Case-Based Explainable GNN Framework**
  * Provides mechanistic explanations for drug repositioning predictions
  * Combines prediction accuracy with interpretability
  * [Paper (bioRxiv, 2025)](https://www.biorxiv.org/content/10.1101/2025.04.28.651120v1) | [Code](https://github.com/SuLab/DBR-X)
  * Organizations: Scripps Research

* **DeepDrug: Expert-led AI-Driven Drug Repurposing**
  * Authors: Focus on Alzheimer's Disease
  * Signed directed heterogeneous biomedical graph with node/edge weighting
  * Graph Neural Network encoding into new embedding space
  * [Paper (medRxiv, 2024)](https://www.medrxiv.org/content/10.1101/2024.07.06.24309990v1)

* **EDGAR: Explainable Enrichment-Driven GrAph Reasoner** (2024)
  * Uses enrichment analysis to identify statistically significant patterns in biomedical KGs
  * Demonstrated on ROBOKOP KG for Alzheimer's disease drug repurposing
  * Interactive, explainable predictions ensuring transparent repurposing process
  * Identifies biological pathways connecting drugs to diseases
  * [Paper (arXiv, 2024)](https://arxiv.org/html/2409.18659v2)
  * Organizations: RENCI, UNC Chapel Hill

### Random Walk & Embedding Methods

* **KGML-xDTD: Knowledge Graph Machine Learning Framework**
  * Authors: Chunyu Ma, Zhihan Zhou, Han Liu, David Koslicki
  * Combines knowledge graphs with machine learning for drug treatment prediction
  * Provides mechanistic descriptions of predicted treatments
  * [Paper (GigaScience, 2023)](https://academic.oup.com/gigascience/article/doi/10.1093/gigascience/giad057/7246583) | [Code](https://github.com/chunyuma/KGML-xDTD)
  * Organizations: Oregon State University, Penn State University

* **DREAMwalk: Guilt-by-Association Multi-Layer Extension**
  * Authors: Dongmin Bang, Sangsoo Lim, Sangseon Lee, Sun Kim
  * Extends guilt-by-association to multiple knowledge graph layers
  * Biomedical knowledge graph learning for drug repurposing
  * [Paper (Nature Communications, 2023)](https://www.nature.com/articles/s41467-023-39301-y) | [Code](https://github.com/eugenebang/DREAMwalk)
  * Organizations: Seoul National University

### Methodology: Negative Sampling & Evaluation

* **Node-Degree Aware Negative Sampling (DANS)**
  * Mitigates inflated classification performance from degree bias in biomedical KGs
  * Addresses lack of experimentally validated negative samples
  * Important for proper evaluation of random walk-based graph representation learning
  * Used in drug repositioning, drug-target interactions, and DDI prediction
  * [Paper (Bioinformatics Advances, 2024)](https://academic.oup.com/bioinformaticsadvances/article/4/1/vbae036/7619101) | [Code](https://github.com/monarch-initiative/negativeExampleSelection)
  * Organizations: Monarch Initiative

### Rule-Based & Logic Methods

* **Hetionet: Systematic integration of biomedical knowledge**
  * Authors: Daniel Scott Himmelstein, Antoine Lizee, Christine Hessler, Leo Brueggeman, Sabrina L Chen, Dexter Hadley, Ari Green, Pouya Khankhanian, Sergio E Baranzini
  * [Paper (eLife, 2017)](https://elifesciences.org/articles/26726) | [Code](https://github.com/hetio/hetionet)
  * Organizations: UCSF

* **mediKanren: Precision medicine process using AI**
  * Authors: Aleksandra Foksinska, Camerron M Crowder, Andrew B Crouse, Jeff Henrikson, William E Byrd, Gregory Rosenblatt, Michael J Patton, Kaiwen He, Thi K Tran-Nguyen, Marissa Zheng, Stephen A Ramsey, Nada Amin, John Osborne, UAB Precision Medicine Institute, Matthew Might
  * [Paper (PubMed)](https://pubmed.ncbi.nlm.nih.gov/36248623/) | [Code](https://github.com/webyrd/mediKanren)
  * Organizations: UAB, Oregon State

---

## Deep Learning & Generative AI

Modern deep learning architectures for molecular generation and drug-target interaction.

### Large Language Models & Transformers

* **AI-Assisted Drug Re-Purposing for Human Liver Fibrosis** - LLM-based approach
  * Authors: Yuan Guan, Lu Cui, Jakkapong Inchai, Zhuoqing Fang, Jacky Law, Alberto Alonzo Garcia Brito, Annalisa Pawlosky, Juraj Gottweis, Alexander Daryin, Artiom Myaskovsky, Lakshmi Ramakrishnan, Anil Palepu, Kavita Kulkarni, Wei-Hung Weng, Zhuanfen Cheng, Vivek Natarajan, Alan Karthikesalingam, Keran Rong, Yunhan Xu, Tao Tu, Gary Peltz
  * [Paper (Advanced Science, 2025)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202508751)
  * Organizations: Google Research

* **Repurformer: Transformers for Repurposing-Aware Molecule Generation** (2024)
  * Integrates bi-directional pretraining with FFT and low-pass filtering
  * Addresses sample bias problem in molecule generation
  * [Paper (arXiv, 2024)](https://arxiv.org/html/2407.11439)

* **PCMol: AlphaFold2-Conditioned Multitarget Transformer** (2024)
  * Leverages AlphaFold2 protein embeddings to condition molecular generation
  * Multitarget transformer model for de novo drug design
  * [Paper (JCIM, 2024)](https://pubs.acs.org/doi/10.1021/acs.jcim.4c00309)

* **GraphRAG: LLM-Based Knowledge Graph Construction** (Microsoft Research)
  * Uses LLMs to create knowledge graphs from unstructured biomedical data
  * Vastly improves retrieval for question-answering in drug discovery
  * Addresses limitations of baseline RAG by using LLM-generated KGs for context
  * Enables integration of smaller, specialized KGs using natural language queries
  * [Paper (Microsoft Research)](https://www.microsoft.com/en-us/research/blog/graphrag-unlocking-llm-discovery-on-narrative-private-data/)
  * Organizations: Microsoft Research

### Diffusion Models

* **Diffusion Models for De Novo Drug Design** - Comprehensive framework (2024)
  * Applications: structure-based design, molecular docking, conformation generation
  * Excels at 3D molecular structure generation with desired physicochemical properties
  * Pharmacophore-oriented approaches with explicit constraints
  * [Paper (JCIM, 2024)](https://pubs.acs.org/doi/10.1021/acs.jcim.4c01107) | [Review Paper (arXiv)](https://arxiv.org/html/2406.08511v1)

* **GenMol: Drug Discovery Generalist with Discrete Diffusion** (2025)
  * Unified framework for structure-based drug discovery
  * Dual diffusion model for de novo generation and lead optimization
  * [Paper (arXiv, 2025)](https://arxiv.org/pdf/2501.06158)

### Variational Autoencoders (VAE)

* **TransVAE-DTA: Transformer + VAE for Drug-Target Affinity** (2024)
  * VAE for drug structure encoding, transformer for target features
  * Computational drug-target binding affinity prediction
  * [Paper (ScienceDirect, 2024)](https://www.sciencedirect.com/science/article/abs/pii/S0169260723006697)

* **Transformer Graph VAE (TGVAE)** (2025)
  * Combines transformer, GNN, and VAE for molecular generation
  * Broader range of unique molecular structures than traditional methods
  * [Paper (Biophysical Journal, 2025)](https://www.cell.com/biophysj/fulltext/S0006-3495(25)00035-9)

* **VAE-Transformer Hybrid for Diverse Molecules** (2024)
  * Structural and parameter optimization for handling diverse molecules
  * [Paper (arXiv, 2024)](https://arxiv.org/abs/2402.11950)

### Reinforcement Learning

* **Deep Reinforcement Learning for Multiparameter Optimization** (2024)
  * Treats molecular optimization as sequential decision-making
  * Multi-objective optimization: kinase activity, drug-likeness, patent landscape
  * REINVENT algorithm for generating novel small molecules
  * [Paper (JCIM)](https://pubs.acs.org/doi/10.1021/acs.jcim.9b00325) | [Review (Nature Communications)](https://www.nature.com/articles/s42004-022-00733-0)

* **Evaluation of RL in Transformer-Based Molecular Design** (2024)
  * RL as tuning phase to steer pre-trained models toward desirable properties
  * Systematic evaluation of on-policy and off-policy RL algorithms
  * [Paper (Journal of Cheminformatics, 2024)](https://jcheminf.biomedcentral.com/articles/10.1186/s13321-024-00887-0)

---

## Natural Language Processing & Text Mining

Leveraging biomedical literature and text data for drug repurposing insights.

### BERT-Based Models for Biomedical Text

* **BioBERT: Pre-trained Biomedical Language Representation Model**
  * Domain-specific BERT pre-trained on PubMed abstracts and PMC full-text articles
  * Significantly outperforms BERT on biomedical NER (0.62% improvement), relation extraction (2.80% improvement), and QA (12.24% improvement)
  * Critical for mining drug-disease relationships from literature
  * [Paper (Bioinformatics, 2020)](https://academic.oup.com/bioinformatics/article/36/4/1234/5566506) | [Code](https://github.com/dmis-lab/biobert)
  * Organizations: Korea University

* **PubMedBERT: Biomedical Language Model for Drug Repurposing**
  * Pre-trained solely on PubMed abstracts (not general text like BioBERT)
  * Achieves F1 = 0.854 for semantic predication classification in COVID-19 drug repurposing
  * Used for node attribute embeddings in biomedical knowledge graphs
  * Produces higher quality embeddings than generalized models for medical literature
  * [Model (HuggingFace)](https://huggingface.co/NeuML/pubmedbert-base-embeddings) | [Paper (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC7869625/)
  * Applications: COVID-19 drug repurposing via KG completion, DrugReX system

### Chemical Language Models

* **ChemBERTa: Large-Scale Self-Supervised Pretraining**
  * BERT-like models for chemical SMILES data
  * Pre-trained on PubChem using masked language modeling
  * Competitive performance on MoleculeNet for toxicity, solubility, drug-likeness
  * [Paper (arXiv, 2020)](https://arxiv.org/abs/2010.09885) | [Code](https://github.com/seyonechithrananda/bert-loves-chemistry) | [HuggingFace](https://huggingface.co/seyonec/ChemBERTa-zinc-base-v1)

* **ChemBERTa-2: Towards Chemical Foundation Models** (2022)
  * Enhanced version with improved pre-training strategies
  * [Paper (arXiv, 2022)](https://arxiv.org/pdf/2209.01712)

### Literature Mining Applications

* **Drug Repurposing via Knowledge Graph Completion for COVID-19**
  * BERT variant for accuracy classification of semantic triples
  * Successfully predicted baricitinib repurposing (later validated clinically)
  * Named entity recognition using BioBERT
  * [Paper (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC7869625/)

* **Using BERT to Identify Drug-Target Interactions from Whole PubMed**
  * Novel method identifying 0.6 million articles not in public DTI databases
  * Expands knowledge beyond structured databases
  * [Paper (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC9214985/)

* **DrugAgent: Explainable Drug Repurposing with LLM Reasoning** (2024)
  * Large language model-based reasoning for drug repurposing
  * Extracts drug-target interactions from DrugBank, DGIdb, CTD, STITCH
  * [Paper (arXiv, 2024)](https://arxiv.org/html/2408.13378v3)

* **DrugReX: Explainable Drug Repurposing System with LLMs and Literature KG** (2024)
  * Combines PubMedBERT (F1 = 0.808) with literature-based knowledge graphs
  * Enriches KG with semantic relationships via SemRep and PubMedBERT
  * For Alzheimer's disease: identified 25 promising candidates (9 clustering with FDA-approved drugs, 10 in clinical trials)
  * Enables nuanced understanding of drug-disease interactions
  * [Paper (PMC, 2024)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12204371/)

---

## Network Medicine & Systems Biology

Approaches using protein-protein interactions and biological networks.

* **PIONEER: Protein-Protein Interaction Interface Prediction** (2024)
  * Integrates 100,000 individual genomes, 16,000+ protein structures, 300,000 PPI pairs
  * Identifies drug targets for dozens of cancers and complex diseases
  * Computational tool for predicting mutation effects on PPIs
  * [News (ScienceDaily, Oct 2024)](https://www.sciencedaily.com/releases/2024/10/241024131819.htm)

* **DeepDrug: AI-Driven Platform with Signed Directed Graph** (2024)
  * Signed directed heterogeneous biomedical graph with node/edge weighting
  * Incorporates protein-protein interaction data from STRING
  * Focus on Alzheimer's disease drug combinations
  * [Paper (medRxiv, 2024)](https://www.medrxiv.org/content/10.1101/2024.07.06.24309990v1)

* **Network-Based Drug Repurposing with Population Validation**
  * Network proximity approaches for predicting drug-disease relationships
  * Population-based validation of in silico predictions
  * [Paper (Nature Communications, 2018)](https://www.nature.com/articles/s41467-018-05116-5)

* **Drug and Protein Interaction Network for Alzheimer's Disease** (2023)
  * Network construction and analysis for drug repurposing
  * [Paper (MDPI, 2023)](https://www.mdpi.com/2673-9879/3/4/45)

---

## Single-Cell & Transcriptomics Approaches

Using single-cell RNA sequencing and transcriptomics for drug repurposing.

* **CRISP: Cell-Type-Specific Drug Perturbation Response Predictor** (2025)
  * Foundation model predicting drug responses in unseen cell types at single-cell resolution
  * Transfer learning from control to perturbed states
  * Advances drug repurposing and screening capabilities
  * [Paper (Nature Computational Science, 2025)](https://www.nature.com/articles/s43588-025-00887-6)

* **scDrug+: Single-Cell Transcriptomics + Molecular Structure** (2024)
  * Comprehensive pipeline integrating scRNA-seq with drug-response prediction
  * Predicts response of new drugs by analyzing molecular structures
  * [Paper (ScienceDirect, 2024)](https://www.sciencedirect.com/science/article/pii/S0753332224009545)

* **scDrug: From Single-Cell RNA-seq to Drug Response**
  * Original framework for predicting drug responses from scRNA-seq data
  * [Paper (ScienceDirect, 2022)](https://www.sciencedirect.com/science/article/pii/S2001037022005505)

* **Single-Cell Transcriptional Signatures in Colorectal Cancer** (2024)
  * Analysis of 91,103 scRNA-seq samples from 29 colorectal cancer patients
  * Identified drugs reversing cancer-to-normal gene signature patterns
  * [Paper (BMC Cancer, 2024)](https://bmccancer.biomedcentral.com/articles/10.1186/s12885-024-12142-8)

* **Connectivity Map (CMAP/CLUE) - Transcriptomics-Based Platform**
  * Over 1 million expression signatures (1,000-fold scale-up from 2006)
  * L1000 reduced representation expression profiling method
  * Identifies molecules generating gene expression profiles negatively correlating with disease signatures
  * [Platform (Broad Institute)](https://www.broadinstitute.org/connectivity-map-cmap) | [Website](https://clue.io)
  * Organizations: Broad Institute

---

## Data Resources & Knowledge Graphs

Foundational knowledge graphs integrating biomedical data for drug repurposing.

* **PrimeKG: Precision Medicine Knowledge Graph** - Most comprehensive medical KG
  * Authors: Payal Chandak, Kexin Huang, Marinka Zitnik
  * Integrates 20+ biomedical data sources
  * Foundation for TxGNN and other precision medicine applications
  * [Paper (Nature Scientific Data, 2023)](https://www.nature.com/articles/s41597-023-01960-3) | [Code](https://github.com/mims-harvard/PrimeKG)
  * Organizations: Harvard Medical School, MIMS Harvard

* **RTX-KG2: Semantically Standardized Knowledge Graph**
  * Authors: E. C. Wood, Amy K. Glen, Lindsey G. Kvarfordt, Finn Womack, Liliana Acevedo, Timothy S. Yoon, Chunyu Ma, Veronica Flores, Meghamala Sinha, Yodsawalai Chodpathumwan, Arash Termehchy, Jared C. Roach, Luis Mendoza, Andrew S. Hoffman, Eric W. Deutsch, David Koslicki, Stephen A. Ramsey
  * Built for translational biomedicine
  * Standardized semantic framework
  * [Paper (BMC Bioinformatics, 2022)](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-022-04932-3) | [Code](https://github.com/RTXteam/RTX-KG2)
  * Organizations: Oregon State University, Institute for Systems Biology

* **Hetionet: Integrative Heterogeneous Network**
  * Authors: Daniel Scott Himmelstein, Antoine Lizee, Christine Hessler, Leo Brueggeman, Sabrina L Chen, Dexter Hadley, Ari Green, Pouya Khankhanian, Sergio E Baranzini
  * Connects diseases, drugs, genes, anatomies, pathways, and biological processes
  * Pioneering open science approach
  * [Paper (eLife, 2017)](https://elifesciences.org/articles/26726) | [Code](https://github.com/hetio/hetionet)
  * Organizations: UCSF

* **ROBOKOP: Reasoning Over Biomedical Objects linked in Knowledge Oriented Pathways**
  * Open question-answering platform leveraging 30+ biomedical databases
  * ~10 million nodes and 250 million edges from federated sources
  * Finds biological pathways connecting drugs to diseases
  * Clinical Outcome Pathways (COPs) concept for accelerating drug repurposing
  * Used by EDGAR framework for explainable Alzheimer's drug repurposing
  * [Paper (JCIM, 2020)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00683) | [News (RENCI)](https://renci.org/blog/new-concept-poised-to-accelerate-drug-discovery-through-data-mining/)
  * Organizations: RENCI, UNC Chapel Hill, Institute for Systems Biology

---

## Databases & Compound Libraries

Curated databases and compound collections for computational screening.

* **Broad Institute Drug Repurposing Hub** - Gold standard compound library
  * Nearly 7,000 FDA-approved drugs, clinical trial drugs, and preclinical compounds
  * Heavily used for COVID-19 research (172 strongly active molecules identified)
  * Applications in rare diseases, cancer, infectious diseases
  * [Portal](https://www.broadinstitute.org/drug-repurposing-hub) | [Data Portal](https://repo-hub.broadinstitute.org/repurposing)
  * Organizations: Broad Institute

* **DrugBank: Comprehensive Drug Data Resource**
  * AI-ready datasets for machine learning
  * Structured indication datasets for drug repurposing ML models
  * Machine-readable pharmacology data
  * Widely used as training data source (PubChem, BindingDB, etc.)
  * [Platform](https://go.drugbank.com/) | [ML Resources](https://www.drugbank.com/ai)
  * Organizations: University of Alberta

* **DrugRepoBank: Comprehensive Drug Repositioning Database** (2024)
  * Discovery platform accelerating drug repositioning
  * [Paper (Database, Oxford Academic, 2024)](https://academic.oup.com/database/article/doi/10.1093/database/baae051/7712639)

* **Connectivity Map (CMAP) / CLUE Platform**
  * Over 1 million transcriptomic signatures
  * L1000 expression profiling across perturbations
  * Cloud-based platform with web applications
  * [Platform](https://www.broadinstitute.org/connectivity-map-cmap) | [GitHub](https://github.com/cmap)
  * Organizations: Broad Institute, NIH LINCS

* **MeDIC: Medicines, Diseases, Indications, and Contraindications Database**
  * Curated collection of tabulated data sources for drug repurposing
  * Sources: American drug labels, FDA Orange Book and Purple Book documents
  * Used in Every Cure's MATRIX project and ROBOKOP collaborations
  * [Portal (RENCI)](https://medic.renci.org/) | [MATRIX Project](https://renci.org/project/matrix/)
  * Organizations: RENCI, UNC Chapel Hill, Every Cure

---

## Benchmarks & Challenges

Standardized benchmarks and community challenges for evaluating methods.

* **MoleculeNet: Large-Scale Molecular ML Benchmark**
  * 17 datasets, 700,000+ compounds
  * Physical chemistry and physiology categories (ADMET experiments)
  * Standard benchmark for molecular property prediction
  * [Systematic Study (Nature Communications, 2023)](https://www.nature.com/articles/s41467-023-41948-6)

* **PharmaBench: Enhanced ADMET Benchmarks with LLMs** (2024)
  * 156,618 entries using multi-agent data mining with LLMs
  * Addresses small dataset sizes and lack of drug discovery compound representation
  * [Paper (Nature Scientific Data, 2024)](https://www.nature.com/articles/s41597-024-03793-0)

* **ADMET-AI: Machine Learning ADMET Platform** (2024)
  * Fastest publicly available web server (45% faster than alternatives for 1000 molecules)
  * Available as website and Python package
  * [Paper (Bioinformatics, 2024)](https://academic.oup.com/bioinformatics/article/40/7/btae416/7698030)

* **ChemXTree: Feature-Enhanced GNN-Neural Decision Tree** (2024)
  * SOTA performance on MoleculeNet and 8 drug discovery datasets
  * Outperforms top models on 8 out of 12 datasets
  * [Paper (JCIM, 2024)](https://pubs.acs.org/doi/10.1021/acs.jcim.4c01186)

* **CTD2 PANcancer Drug Activity DREAM Challenge**
  * 21 teams, 86 models predicting drug polypharmacology
  * Dose-response and RNA-seq profiles across 400+ oncology drugs
  * 45% of models showed significant enrichment of true off-targets
  * [Paper (ScienceDirect, 2022)](https://www.sciencedirect.com/science/article/pii/S2666379121003694) | [Synapse Platform](https://www.synapse.org/Synapse:syn21996275)
  * Organizations: Columbia University, NIH/NCI CTD2

* **Therapeutics Data Commons (TDC)**
  * Standardized drug-target interaction benchmarks
  * Community-driven resource for ML in drug discovery
  * [Platform](https://tdcommons.ai/)

---

## Tools & Software Libraries

Practical implementations and software for drug repurposing research.

* **DeepPurpose: Deep Learning Library for DTI Prediction**
  * Authors: Kexin Huang, Tianfan Fu, Lucas M Glass, Marinka Zitnik, Cao Xiao, Jimeng Sun
  * 15 compound and protein encoders, 50+ neural architectures
  * State-of-the-art DTI prediction performance
  * Applications: drug repurposing, virtual screening, compound property prediction
  * Easy-to-use (several lines of code)
  * [Paper (Bioinformatics, 2020)](https://academic.oup.com/bioinformatics/article/36/22-23/5545/6020256) | [Code](https://github.com/kexinhuang12345/DeepPurpose)
  * Organizations: University of Illinois, Harvard Medical School

* **TxGNN Software Package**
  * Implementation of TxGNN foundation model
  * Zero-shot drug repurposing across 17,080 diseases
  * [Code](https://github.com/mims-harvard/TxGNN)
  * Organizations: MIMS Harvard

* **mediKanren Reasoning System**
  * Biomedical reasoning for precision medicine
  * Logical inference over knowledge graphs
  * [Code](https://github.com/webyrd/mediKanren)

* **ADMET-AI Platform**
  * Fast ADMET property predictions
  * Website and Python package
  * [Paper (Bioinformatics, 2024)](https://academic.oup.com/bioinformatics/article/40/7/btae416/7698030)

---

## Key Research Organizations & Labs

Leading institutions and research groups advancing AI drug repurposing.

### Academic Institutions

* **Harvard Medical School - MIMS (Machine Intelligence in Medicine and Science)**
  * PI: Marinka Zitnik
  * Key Contributions: TxGNN, PrimeKG, DeepPurpose
  * [Lab Website](https://zitniklab.hms.harvard.edu/)

* **Broad Institute**
  * Key Contributions: Drug Repurposing Hub, Connectivity Map/CLUE, Cancer Dependency Map
  * [Website](https://www.broadinstitute.org/)

* **Oregon State University - Computational Biology Lab**
  * PIs: Stephen A. Ramsey, David Koslicki
  * Key Contributions: RTX-KG2, KGML-xDTD, mediKanren
  * Focus: Knowledge graphs, computational pharmacophenomics

* **University of California San Francisco (UCSF)**
  * PI: Sergio E Baranzini
  * Key Contributions: Hetionet
  * Focus: Network medicine, systems biology

* **Stanford University**
  * PI: Jure Leskovec
  * Key Contributions: TxGNN, graph learning methods

* **Korea University - DMIS Lab**
  * Key Contributions: BioBERT
  * Focus: Biomedical NLP

* **RENCI (Renaissance Computing Institute) - UNC Chapel Hill**
  * Key Contributions: ROBOKOP, MeDIC, EDGAR, Clinical Outcome Pathways
  * Collaborative partner in Every Cure's MATRIX project
  * Focus: Biomedical knowledge graphs, drug repurposing infrastructure
  * [Website](https://renci.org/)

### Industry & AI Companies

* **BenevolentAI**
  * First major clinical success: Baricitinib for COVID-19
  * Knowledge graph-driven drug discovery
  * [Website](https://www.benevolent.com/)

* **Insilico Medicine**
  * First AI-designed drug with positive Phase IIa results (ISM001-055)
  * End-to-end generative AI platform
  * [Website](https://insilico.com/)

* **Recursion Pharmaceuticals**
  * Phenomics-first drug discovery platform
  * 65 petabytes of biological data
  * 7+ programs in/entering clinical trials (2025)
  * [Website](https://www.recursion.com/)

* **DeepMind/Isomorphic Labs**
  * AlphaFold 2 & 3 for structure-based drug discovery
  * [Website](https://www.isomorphiclabs.com/)

### Non-Profits & Government

* **Every Cure**
  * ARPA-H MATRIX project ($48M)
  * Systematic drug repurposing for rare diseases
  * [News](https://arpa-h.gov/news-and-events/arpa-h-awards-ai-driven-project-repurpose-approved-medications)

* **ARPA-H (Advanced Research Projects Agency for Health)**
  * Funding major AI drug repurposing initiatives
  * Focus on translational impact

---

## Comprehensive Reviews

Essential review papers for understanding the field (ordered by recency and comprehensiveness).

* **Applications of Artificial Intelligence in Drug Repurposing** (2025)
  * Most comprehensive recent review of AI frameworks and multimodal datasets
  * [Paper (Advanced Science, Wiley, 2025)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202411325)

* **AI-Driven Drug Discovery: A Critical Review** (2025)
  * Critical analysis of advancements (2019-2024) across entire drug discovery pipeline
  * Deep learning, GNNs, transformers, and more
  * [Paper (ACS Omega, 2025)](https://pubs.acs.org/doi/pdf/10.1021/acsomega.5c00549)

* **Leading AI-Driven Drug Discovery Platforms: 2025 Landscape and Global Outlook** (2025)
  * Compares five leading platforms: generative chemistry, phenomics, integrated pipelines, knowledge-graph repurposing, physics-ML design
  * [Paper (ScienceDirect, 2025)](https://www.sciencedirect.com/science/article/abs/pii/S0031699725075118)

* **Towards a More Inductive World for Drug Repurposing** (2025)
  * Focus on drug-target interaction prediction challenges
  * [Paper (Nature Machine Intelligence, 2025)](https://www.nature.com/articles/s42256-025-00987-y)

* **The Potential of AI in Pharmaceutical Innovation: From Drug Discovery to Clinical Trials** (2024)
  * Broad overview of AI applications across pharmaceutical development
  * [Paper (PMC, 2024)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12195710/)

* **Artificial Intelligence in Drug Repurposing for Rare Diseases: A Mini-Review** (2024)
  * Focused review on rare disease applications
  * [Paper (Frontiers in Medicine, 2024)](https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2024.1404338/full)

* **Machine Learning and AI in Drug Repurposing—Challenges and Perspectives** (2024)
  * Critical perspective on current challenges
  * [Paper (Drug Repurposing Central, 2024)](https://drugrepocentral.scienceopen.com/hosted-document?doi=10.58647/DRUGREPO.24.1.0004)

* **Generative and Reinforcement Learning Approaches for De Novo Design** (2022)
  * Comprehensive coverage of RL and generative methods
  * [Paper (Nature Communications Chemistry, 2022)](https://www.nature.com/articles/s42004-022-00733-0)

* **Pioneering Computational Pharmacophenomics** (2024)
  * Authors: David C Fajgenbaum, Sally Nijim, Grant Mitchell, Matej Macak, Chris Bizon, Alexander Tropsha, David Koslicki
  * Vision paper for unlocking life-saving potential of existing medicines
  * [Paper (PubMed)](https://pubmed.ncbi.nlm.nih.gov/39909662/)

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. We particularly welcome additions of:
- New clinical successes and validations
- Novel AI/ML methods with published papers
- New datasets and tools
- Updates to existing entries

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
