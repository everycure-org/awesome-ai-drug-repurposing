[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# Awesome AI Drug Repurposing

A curated collection of AI and machine learning resources specifically for drug repurposing—identifying new therapeutic uses for existing drugs.

> Drug repurposing is the process of identifying new therapeutic uses for existing drugs (or drug candidates) that were originally developed for a different condition. AI and machine learning are transforming this field by revealing new therapeutic targets and mechanisms, with 30% of repurposed drugs making it to patients compared to just 10% success rate for traditional drug discovery.

## Table of Contents

1. [Clinical Successes](#clinical-successes)
2. [Landmark Methods & Foundation Models](#landmark-methods--foundation-models)
3. [Knowledge Graph-Based Methods](#knowledge-graph-based-methods)
4. [Large Language Models for Repurposing](#large-language-models-for-repurposing)
5. [Network Medicine & Systems Biology](#network-medicine--systems-biology)
6. [Transcriptomics-Based Repurposing](#transcriptomics-based-repurposing)
7. [Data Resources & Knowledge Graphs](#data-resources--knowledge-graphs)
8. [Databases & Compound Libraries](#databases--compound-libraries)
9. [Tools & Software](#tools--software)
10. [Key Research Organizations](#key-research-organizations)
11. [Reviews](#reviews)

---

## Clinical Successes

Real-world validation of AI-driven drug repurposing with clinical impact.

* **Baricitinib for COVID-19 (BenevolentAI)** - First major AI-driven drug repurposing clinical success
  * Originally approved for rheumatoid arthritis, repurposed for COVID-19 using knowledge graph and ML
  * Identified in 48 hours, received FDA Emergency Use Authorization
  * Clinical trials (ACTT-2, CoV-BARRIER) confirmed significant mortality reduction
  * [Paper (Frontiers in Pharmacology)](https://www.frontiersin.org/journals/pharmacology/articles/10.3389/fphar.2021.709856/full) | [Paper (The Lancet)](https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)30304-4/fulltext)
  * Organizations: BenevolentAI, Eli Lilly

* **ISM001-055/Rentosertib for Idiopathic Pulmonary Fibrosis (Insilico Medicine)**
  * First-in-class TNIK inhibitor discovered using end-to-end generative AI
  * Phase IIa (2024): 98.4 mL improvement in lung function vs -62.3 mL decline in placebo
  * From target discovery to Phase 1 in under 30 months
  * [News (Insilico Medicine)](https://insilico.com/news/tnik-ipf-phase2a)
  * Organizations: Insilico Medicine

* **Sulindac for Fragile X Syndrome (HealX)** - AI-discovered repurposing with IND approval
  * NSAID repurposed for rare genetic disease
  * FDA IND approval for Phase 2a clinical trial (2021)
  * Organizations: HealX

* **REC-994 for Cerebral Cavernous Malformation (Recursion Pharmaceuticals)**
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

Breakthrough approaches specifically designed for drug repurposing.

* **TxGNN: Zero-Shot Drug Repurposing Foundation Model**
  * Authors: Kexin Huang, Payal Chandak, Qianwen Wang, Shreyas Havaldar, Akhil Vaid, Jure Leskovec, Girish N. Nadkarni, Benjamin S. Glicksberg, Nils Gehlenborg, Marinka Zitnik
  * Graph neural network foundation model trained on medical knowledge graph covering 17,080 diseases
  * First model developed specifically for rare diseases and conditions with no treatments
  * Improves prediction accuracy by 49.2% for indications and 35.1% for contraindications
  * Zero-shot learning enables predictions for diseases with limited treatment options
  * [Paper (Nature Medicine, 2024)](https://www.nature.com/articles/s41591-024-03233-x) | [Code](https://github.com/mims-harvard/TxGNN) | [Project Page](https://zitniklab.hms.harvard.edu/projects/TxGNN/)
  * Organizations: Harvard Medical School, MIMS Harvard, Mount Sinai

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
  * Signed directed heterogeneous biomedical graph with node/edge weighting
  * Graph Neural Network encoding into new embedding space
  * Focus on Alzheimer's Disease
  * [Paper (medRxiv, 2024)](https://www.medrxiv.org/content/10.1101/2024.07.06.24309990v1)

* **EDGAR: Explainable Enrichment-Driven GrAph Reasoner** (2024)
  * Uses enrichment analysis to identify statistically significant patterns in biomedical KGs
  * Demonstrated on ROBOKOP KG for Alzheimer's disease drug repurposing
  * Interactive, explainable predictions ensuring transparent repurposing process
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

### Methodology: Negative Sampling

* **Node-Degree Aware Negative Sampling (DANS)**
  * Mitigates inflated classification performance from degree bias in biomedical KGs
  * Important for proper evaluation of drug repositioning predictions
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

## Large Language Models for Repurposing

LLM-based approaches specifically applied to drug repurposing.

* **AI-Assisted Drug Re-Purposing for Human Liver Fibrosis**
  * Authors: Yuan Guan, Lu Cui, Jakkapong Inchai, Zhuoqing Fang, Jacky Law, Alberto Alonzo Garcia Brito, Annalisa Pawlosky, Juraj Gottweis, Alexander Daryin, Artiom Myaskovsky, Lakshmi Ramakrishnan, Anil Palepu, Kavita Kulkarni, Wei-Hung Weng, Zhuanfen Cheng, Vivek Natarajan, Alan Karthikesalingam, Keran Rong, Yunhan Xu, Tao Tu, Gary Peltz
  * [Paper (Advanced Science, 2025)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202508751)
  * Organizations: Google Research

* **Repurformer: Transformers for Repurposing-Aware Molecule Generation** (2024)
  * Integrates bi-directional pretraining with FFT and low-pass filtering
  * Addresses sample bias problem in molecule generation for repurposing
  * [Paper (arXiv, 2024)](https://arxiv.org/html/2407.11439)

* **DrugAgent: Explainable Drug Repurposing with LLM Reasoning** (2024)
  * Large language model-based reasoning for drug repurposing
  * Extracts drug-target interactions from DrugBank, DGIdb, CTD, STITCH
  * [Paper (arXiv, 2024)](https://arxiv.org/html/2408.13378v3)

* **DrugReX: Explainable Drug Repurposing System with LLMs and Literature KG** (2024)
  * Combines PubMedBERT (F1 = 0.808) with literature-based knowledge graphs
  * For Alzheimer's disease: identified 25 promising candidates (9 clustering with FDA-approved drugs, 10 in clinical trials)
  * [Paper (PMC, 2024)](https://pmc.ncbi.nlm.nih.gov/articles/PMC12204371/)

### Biomedical NLP for Drug-Disease Extraction

* **BioBERT: Pre-trained Biomedical Language Representation Model**
  * Domain-specific BERT pre-trained on PubMed abstracts and PMC full-text articles
  * Critical for mining drug-disease relationships from literature
  * [Paper (Bioinformatics, 2020)](https://academic.oup.com/bioinformatics/article/36/4/1234/5566506) | [Code](https://github.com/dmis-lab/biobert)
  * Organizations: Korea University

* **PubMedBERT for Drug Repurposing**
  * Pre-trained solely on PubMed abstracts
  * Achieves F1 = 0.854 for semantic predication classification in COVID-19 drug repurposing
  * [Model (HuggingFace)](https://huggingface.co/NeuML/pubmedbert-base-embeddings) | [Paper (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC7869625/)

* **Drug Repurposing via Knowledge Graph Completion for COVID-19**
  * BERT variant for accuracy classification of semantic triples
  * Successfully predicted baricitinib repurposing (later validated clinically)
  * [Paper (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC7869625/)

* **Using BERT to Identify Drug-Target Interactions from Whole PubMed**
  * Novel method identifying 0.6 million articles not in public DTI databases
  * Expands knowledge beyond structured databases
  * [Paper (PMC)](https://pmc.ncbi.nlm.nih.gov/articles/PMC9214985/)

---

## Network Medicine & Systems Biology

Approaches using protein-protein interactions and biological networks for repurposing.

* **PIONEER: Protein-Protein Interaction Interface Prediction** (2024)
  * Integrates 100,000 individual genomes, 16,000+ protein structures, 300,000 PPI pairs
  * Identifies drug targets for dozens of cancers and complex diseases
  * [News (ScienceDaily, Oct 2024)](https://www.sciencedaily.com/releases/2024/10/241024131819.htm)

* **Network-Based Drug Repurposing with Population Validation**
  * Network proximity approaches for predicting drug-disease relationships
  * Population-based validation of in silico predictions
  * [Paper (Nature Communications, 2018)](https://www.nature.com/articles/s41467-018-05116-5)

* **Drug and Protein Interaction Network for Alzheimer's Disease** (2023)
  * Network construction and analysis for drug repurposing
  * [Paper (MDPI, 2023)](https://www.mdpi.com/2673-9879/3/4/45)

---

## Transcriptomics-Based Repurposing

Using transcriptomics and gene expression signatures for drug repurposing.

* **Connectivity Map (CMAP/CLUE) - Transcriptomics-Based Platform**
  * Over 1 million expression signatures (1,000-fold scale-up from 2006)
  * L1000 reduced representation expression profiling method
  * Identifies molecules generating gene expression profiles negatively correlating with disease signatures
  * [Platform (Broad Institute)](https://www.broadinstitute.org/connectivity-map-cmap) | [Website](https://clue.io)
  * Organizations: Broad Institute

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
  * Framework for predicting drug responses from scRNA-seq data
  * [Paper (ScienceDirect, 2022)](https://www.sciencedirect.com/science/article/pii/S2001037022005505)

* **Single-Cell Transcriptional Signatures in Colorectal Cancer** (2024)
  * Analysis of 91,103 scRNA-seq samples from 29 colorectal cancer patients
  * Identified drugs reversing cancer-to-normal gene signature patterns
  * [Paper (BMC Cancer, 2024)](https://bmccancer.biomedcentral.com/articles/10.1186/s12885-024-12142-8)

---

## Data Resources & Knowledge Graphs

Foundational knowledge graphs for drug repurposing research.

* **PrimeKG: Precision Medicine Knowledge Graph**
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
  * [Paper (JCIM, 2020)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00683) | [News (RENCI)](https://renci.org/blog/new-concept-poised-to-accelerate-drug-discovery-through-data-mining/)
  * Organizations: RENCI, UNC Chapel Hill, Institute for Systems Biology

---

## Databases & Compound Libraries

Curated databases and compound collections for repurposing research.

* **Broad Institute Drug Repurposing Hub**
  * Nearly 7,000 FDA-approved drugs, clinical trial drugs, and preclinical compounds
  * Heavily used for COVID-19 research (172 strongly active molecules identified)
  * Applications in rare diseases, cancer, infectious diseases
  * [Portal](https://www.broadinstitute.org/drug-repurposing-hub) | [Data Portal](https://repo-hub.broadinstitute.org/repurposing)
  * Organizations: Broad Institute

* **DrugBank: Comprehensive Drug Data Resource**
  * AI-ready datasets for machine learning
  * Structured indication datasets for drug repurposing ML models
  * Machine-readable pharmacology data
  * [Platform](https://go.drugbank.com/) | [ML Resources](https://www.drugbank.com/ai)
  * Organizations: University of Alberta

* **DrugRepoBank: Comprehensive Drug Repositioning Database** (2024)
  * Discovery platform accelerating drug repositioning
  * [Paper (Database, Oxford Academic, 2024)](https://academic.oup.com/database/article/doi/10.1093/database/baae051/7712639)

* **MeDIC: Medicines, Diseases, Indications, and Contraindications Database**
  * Curated collection of tabulated data sources for drug repurposing
  * Sources: American drug labels, FDA Orange Book and Purple Book documents
  * Used in Every Cure's MATRIX project
  * [Portal (RENCI)](https://medic.renci.org/) | [MATRIX Project](https://renci.org/project/matrix/)
  * Organizations: RENCI, UNC Chapel Hill, Every Cure

* **Therapeutics Data Commons (TDC)**
  * Standardized drug-target interaction benchmarks
  * Community-driven resource for ML in drug repurposing
  * [Platform](https://tdcommons.ai/)

---

## Tools & Software

Practical implementations for drug repurposing research.

* **DeepPurpose: Deep Learning Library for DTI Prediction**
  * Authors: Kexin Huang, Tianfan Fu, Lucas M Glass, Marinka Zitnik, Cao Xiao, Jimeng Sun
  * 15 compound and protein encoders, 50+ neural architectures
  * State-of-the-art DTI prediction performance
  * Applications: drug repurposing, virtual screening, compound property prediction
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

---

## Key Research Organizations

Leading institutions advancing AI drug repurposing.

### Academic Labs

* **Harvard Medical School - MIMS (Machine Intelligence in Medicine and Science)**
  * PI: Marinka Zitnik
  * Key Contributions: TxGNN, PrimeKG, DeepPurpose
  * [Lab Website](https://zitniklab.hms.harvard.edu/)

* **Oregon State University - Computational Biology Lab**
  * PIs: Stephen A. Ramsey, David Koslicki
  * Key Contributions: RTX-KG2, KGML-xDTD, mediKanren
  * Focus: Knowledge graphs, computational pharmacophenomics

* **University of California San Francisco (UCSF)**
  * PI: Sergio E Baranzini
  * Key Contributions: Hetionet

* **RENCI (Renaissance Computing Institute) - UNC Chapel Hill**
  * Key Contributions: ROBOKOP, MeDIC, EDGAR, Clinical Outcome Pathways
  * Collaborative partner in Every Cure's MATRIX project
  * [Website](https://renci.org/)

* **Broad Institute**
  * Key Contributions: Drug Repurposing Hub, Connectivity Map/CLUE
  * [Website](https://www.broadinstitute.org/)

### Industry

* **BenevolentAI** - First major clinical success: Baricitinib for COVID-19
  * [Website](https://www.benevolent.com/)

* **Insilico Medicine** - First AI-designed drug with positive Phase IIa results
  * [Website](https://insilico.com/)

* **Recursion Pharmaceuticals** - Phenomics-first platform with multiple clinical programs
  * [Website](https://www.recursion.com/)

* **HealX** - AI platform for rare disease drug repurposing
  * [Website](https://healx.io/)

### Non-Profits

* **Every Cure** - ARPA-H MATRIX project ($48M) for systematic drug repurposing
  * [News](https://arpa-h.gov/news-and-events/arpa-h-awards-ai-driven-project-repurpose-approved-medications)

---

## Reviews

Essential review papers for understanding the drug repurposing field.

* **Applications of Artificial Intelligence in Drug Repurposing** (2025)
  * Comprehensive review of AI frameworks and multimodal datasets for repurposing
  * [Paper (Advanced Science, Wiley, 2025)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202411325)

* **Towards a More Inductive World for Drug Repurposing** (2025)
  * Focus on drug-target interaction prediction challenges
  * [Paper (Nature Machine Intelligence, 2025)](https://www.nature.com/articles/s42256-025-00987-y)

* **Artificial Intelligence in Drug Repurposing for Rare Diseases: A Mini-Review** (2024)
  * Focused review on rare disease applications
  * [Paper (Frontiers in Medicine, 2024)](https://www.frontiersin.org/journals/medicine/articles/10.3389/fmed.2024.1404338/full)

* **Machine Learning and AI in Drug Repurposing—Challenges and Perspectives** (2024)
  * Critical perspective on current challenges
  * [Paper (Drug Repurposing Central, 2024)](https://drugrepocentral.scienceopen.com/hosted-document?doi=10.58647/DRUGREPO.24.1.0004)

* **Pioneering Computational Pharmacophenomics** (2024)
  * Authors: David C Fajgenbaum, Sally Nijim, Grant Mitchell, Matej Macak, Chris Bizon, Alexander Tropsha, David Koslicki
  * Vision paper for unlocking life-saving potential of existing medicines
  * [Paper (PubMed)](https://pubmed.ncbi.nlm.nih.gov/39909662/)

---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. We particularly welcome additions of:
- New clinical successes and validations
- Novel AI/ML methods specifically for drug repurposing
- New repurposing-specific datasets and tools
- Updates to existing entries

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
