[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](http://makeapullrequest.com)

# Awesome AI Drug Repurposing

A curated collection of AI and machine learning resources specifically for drug repurposing—identifying new therapeutic uses for existing drugs.

> Drug repurposing is the process of identifying new therapeutic uses for existing drugs (or drug candidates) that were originally developed for a different condition. AI and machine learning are transforming this field by revealing new therapeutic targets and mechanisms, with 30% of repurposed drugs making it to patients compared to just 10% success rate for traditional drug discovery.

## Table of Contents

1. [Knowledge Graph-Based Methods](#knowledge-graph-based-methods)
2. [Large Language Models & Transformers](#large-language-models--transformers)
3. [Data Resources & Knowledge Graphs](#data-resources--knowledge-graphs)
4. [Databases & Compound Libraries](#databases--compound-libraries)
5. [Clinical Successes](#clinical-successes)
6. [Reviews](#reviews)

---

## Knowledge Graph-Based Methods

Methods leveraging knowledge graphs to discover drug-disease relationships.

### Graph Neural Networks (GNNs)

* **TxGNN: A foundation model for clinician-centered drug repurposing**
  * Authors: Kexin Huang, Payal Chandak, Qianwen Wang, Shreyas Havaldar, Akhil Vaid, Jure Leskovec, Girish N. Nadkarni, Benjamin S. Glicksberg, Nils Gehlenborg, Marinka Zitnik
  * [Paper (Nature Medicine, 2024)](https://www.nature.com/articles/s41591-024-03233-x) | [Code](https://github.com/mims-harvard/TxGNN)
  * Organizations: Harvard Medical School

* **A Case-Based Explainable Graph Neural Network Framework for Mechanistic Drug Repositioning**
  * Authors: Andrew I Su, Meghamala Sinha, Roger Tu, Adriana Carolina Gonzalez-Cavazos
  * [Paper](https://www.biorxiv.org/content/10.1101/2025.04.28.651120v1)
  * [Code](https://github.com/SuLab/DBR-X)
  * Organizations: Scripps Research

* **Few shot learning for phenotype-driven diagnosis of patients with rare genetic diseases**
  * Authors: Emily Alsentzer, Michelle M Li, Shilpa N Kobren, Ayush Noori, Undiagnosed Diseases Network, Isaac S Kohane, Marinka Zitnik
  * [Paper](https://pubmed.ncbi.nlm.nih.gov/40542121/)
  * [Code](https://github.com/mims-harvard/SHEPHERD)
  * [Data](https://zitniklab.hms.harvard.edu/projects/SHEPHERD/)
  * Organizations: Harvard Medical School, Brigham and Women's Hospital

* **Enhancing link prediction in biomedical knowledge graphs with BioPathNet**
  * Authors: Emy Yue Hu, Svitlana Oleshko, Samuele Firmani, Hui Cheng, Zhaocheng Zhu, Maria Ulmer, Matthias Arnold, Maria Colomé-Tatché, Jian Tang, Sophie Xhonneux & Annalisa Marsico
  * [Paper](https://www.nature.com/articles/s41551-025-01598-z)
  * [Code](https://github.com/emyyue/BioPathNet)
  * [Code to get Data](https://github.com/emyyue/BioPathNet/blob/main/data/download.sh)

### Graph ML Methods

* **KGML-xDTD: Knowledge Graph Machine Learning Framework**
  * Authors: Chunyu Ma, Zhihan Zhou, Han Liu, David Koslicki
  * [Paper (GigaScience, 2023)](https://academic.oup.com/gigascience/article/doi/10.1093/gigascience/giad057/7246583) | [Code](https://github.com/chunyuma/KGML-xDTD)
  * Organizations: Oregon State University, Penn State University

* **DREAMwalk: Guilt-by-Association Multi-Layer Extension**
  * Authors: Dongmin Bang, Sangsoo Lim, Sangseon Lee, Sun Kim
  * [Paper (Nature Communications, 2023)](https://www.nature.com/articles/s41467-023-39301-y) | [Code](https://github.com/eugenebang/DREAMwalk)
  * Organizations: Seoul National University

* **Integrating biomedical research and electronic health records to create knowledge-based biologically meaningful machine-readable embeddings**
  * Authors: Charlotte A. Nelson, Atul J. Butte & Sergio E. Baranzini
  * [Paper (Nature Communications, 2019)](https://www.nature.com/articles/s41467-019-11069-0)
  * [Code](https://github.com/BaranziniLab/PSEV)
  * Organizations: UCSF


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

## Large Language Models & Transformers

Transformer-based approaches specifically applied to drug repurposing.

* **AI-Assisted Drug Re-Purposing for Human Liver Fibrosis**
  * Authors: Yuan Guan, Lu Cui, Jakkapong Inchai, Zhuoqing Fang, Jacky Law, Alberto Alonzo Garcia Brito, Annalisa Pawlosky, Juraj Gottweis, Alexander Daryin, Artiom Myaskovsky, Lakshmi Ramakrishnan, Anil Palepu, Kavita Kulkarni, Wei-Hung Weng, Zhuanfen Cheng, Vivek Natarajan, Alan Karthikesalingam, Keran Rong, Yunhan Xu, Tao Tu, Gary Peltz
  * [Paper (Advanced Science, 2025)](https://advanced.onlinelibrary.wiley.com/doi/10.1002/advs.202508751)
  * Organizations: Google Research

* **NetMedGPT - A network medicine foundation model for extensive disease mechanism mining and drug repurposing**
   * Authors: Farzaneh Firoozbakht, Simon Süwer, Maria Louise Elkjaer, Diane E. Handy, Andreas Maier, Jane Li, Lee Lancashire, Joseph Loscalzo, Jan Baumbach 
   * [Paper](https://www.biorxiv.org/content/10.64898/2026.01.04.697552v1)
   * [Code](https://github.com/faren-f/NetMedGPT)
   * [Data](https://cloud.uni-hamburg.de/s/r74Ro8rmQ2sHwsL)

* **K-Paths: Reasoning over Graph Paths for Drug Repurposing and Drug Interaction Prediction**
  * Authors: Tassallah Abdullahi, Ioanna Gemou†, Nihal V. Nayak, Ghulam Murtaza, Stephen H. Bach, Carsten Eickhoff, Ritambhara Singh
  * [Paper](https://arxiv.org/pdf/2502.13344)
  * [Code](https://github.com/rsinghlab/K-Paths)

* **DrugReAlign: a multisource prompt framework for drug repurposing based on large language models**
  * Authors: Jinhang Wei, Linlin Zhuo, Xiangzheng Fu, XiangXiang Zeng, Li Wang, Quan Zou, Dongsheng Cao
  * [Paper (BMC Biology, 2024)](https://link.springer.com/article/10.1186/s12915-024-02028-3)
  * [Code](https://github.com/jinhang23/DrugReAlign)
---

## Data Resources & Knowledge Graphs

Foundational knowledge graphs for drug repurposing research.

* **PrimeKG: Precision Medicine Knowledge Graph**
  * Authors: Payal Chandak, Kexin Huang, Marinka Zitnik
  * [Paper (Nature Scientific Data, 2023)](https://www.nature.com/articles/s41597-023-01960-3)
  * [Code](https://github.com/mims-harvard/PrimeKG)
  * [Data](https://doi.org/10.7910/DVN/IXA7BM) 
  * Organizations: Harvard Medical School, MIMS Harvard

* **RTX-KG2: Semantically Standardized Knowledge Graph**
  * Authors: E. C. Wood, Amy K. Glen, Lindsey G. Kvarfordt, Finn Womack, Liliana Acevedo, Timothy S. Yoon, Chunyu Ma, Veronica Flores, Meghamala Sinha, Yodsawalai Chodpathumwan, Arash Termehchy, Jared C. Roach, Luis Mendoza, Andrew S. Hoffman, Eric W. Deutsch, David Koslicki, Stephen A. Ramsey
  * [Paper (BMC Bioinformatics, 2022)](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/s12859-022-04932-3)
  * [Code](https://github.com/RTXteam/RTX-KG2)
  * [Data](http://rtx-kg2-public.s3-website-us-west-2.amazonaws.com/)
  * Organizations: Oregon State University, Institute for Systems Biology

* **Hetionet: Integrative Heterogeneous Network**
  * Authors: Daniel Scott Himmelstein, Antoine Lizee, Christine Hessler, Leo Brueggeman, Sabrina L Chen, Dexter Hadley, Ari Green, Pouya Khankhanian, Sergio E Baranzini
  * [Paper](https://elifesciences.org/articles/26726)
  * [Code](https://github.com/hetio/hetionet)
  * [Data](https://zenodo.org/records/268568)
  * Organizations: UCSF

* **Design and application of a knowledge network for automatic prioritization of drug mechanisms**
  * Authors: Michael Mayers, Roger Tu, Dylan Steinecke, Tong Shu Li, Nuria Queralt-Rosinach, Andrew I Su
  * [Paper](https://pubmed.ncbi.nlm.nih.gov/35561182/)
  * [Code](https://github.com/SuLab/MechRepoNet)
  * [Data](https://doi.org/10.5281/zenodo.6456335)
  * Organizations: Scripps Research

* **ROBOKOP: Reasoning Over Biomedical Objects linked in Knowledge Oriented Pathways**
  * Authors: Kenneth Morton, Patrick Wang, Chris Bizon, Steven Cox, James Balhoff, Yaphet Kebede, Karamarie Fecho, Alexander Tropsha
  * [Paper (JCIM, 2020)](https://pubs.acs.org/doi/abs/10.1021/acs.jcim.9b00683) 
  * [Platform](https://robokop.renci.org/) 
  * Organizations: RENCI, UNC Chapel Hill

* **The scalable precision medicine open knowledge engine (SPOKE): a massive knowledge graph of biomedical information**
  * Authors: John H. Morris, Karthik Soman, Rabia E. Akbas, Xiaoyuan Zhou, Brett Smith, Elaine C. Meng, Conrad C. Huang, Gabriel Cerono, Gundolf Schenk, Angela Rizk-Jackson, Adil Harroud, Lauren Sanders, Sylvain V. Costes, Krish Bharat, Arjun Chakraborty, Alexander R. Pico, Taline Mardirossian, Michael Keiser, Alice Tang, Josef Hardi, Yongmei Shi, Mark Musen, Sharat Israni, Sui Huang, Peter W. Rose, Charlotte A. Nelson, Sergio E. Baranzini
  * Open Access
  * [Paper (Bioinformatics, 2023)](https://academic.oup.com/bioinformatics/article/39/2/btad080/7033465)
  * [Platform](https://spoke.ucsf.edu/)
  * Organizations: UCSF, Lawrence Berkeley National Laboratory, Stanford University

* **Open Targets Platform: Genetics-driven target prioritization and drug repurposing**
  * Authors: Annalisa Buniello, Daniel Suveges, Carlos Cruz-Castillo, Manuel Bernal Llinares, Helena Cornu, et al.
  * [Paper (Nucleic Acids Research, 2025)](https://academic.oup.com/nar/article/53/D1/D1467/7917960)
  * [Platform](https://platform.opentargets.org/)
  * [Data](https://platform-docs.opentargets.org/data-access/datasets)
  * Organizations: Open Targets Consortium (EMBL-EBI, Wellcome Sanger Institute, and others)

---

## Databases & Compound Libraries

Curated databases, platforms, and compound collections for repurposing research.

* **Broad Institute Drug Repurposing Hub**
  * [Portal](https://www.broadinstitute.org/drug-repurposing-hub)
  * [Data Portal](https://repo-hub.broadinstitute.org/repurposing)
  * Organizations: Broad Institute

* **DrugMechDB: A Curated Database of Drug Mechanisms**
  * Authors: Adriana Carolina Gonzalez-Cavazos, Anna Tanska, Michael Mayers, Denise Carvalho-Silva, Brindha Sridharan, Patrick A. Rewers, Umasri Sankarlal, Lakshmanan Jagannathan & Andrew I. Su
  * [Paper](https://doi.org/10.1038/s41597-023-02534-z)
  * [Data](https://zenodo.org/records/8139357)
  * [Code](https://github.com/SuLab/DrugMechDB/tree/2.0.1)
  * Organization: Scripps

* **DrugBank Knowledgebase**
  * Authors: Craig Knox, Mike Wilson, Christen M Klinger, Mark Franklin, Eponine Oler, Alex Wilson, Allison Pon, Jordan Cox, Na Eun (Lucy) Chin, Seth A Strawbridge, Marysol Garcia-Patino, Ray Kruger, Aadhavya Sivakumaran, Selena Sanford, Rahil Doshi, Nitya Khetarpal, Omolola Fatokun, Daphnee Doucet, Ashley Zubkowski, Dorsa Yahya Rayat, Hayley Jackson, Karxena Harford, Afia Anjum, Mahi Zakir, Fei Wang, Siyang Tian, Brian Lee, Jaanus Liigand, Harrison Peters, Ruo Qi (Rachel) Wang, Tue Nguyen, Denise So, Matthew Sharp, Rodolfo da Silva, Cyrella Gabriel, Joshua Scantlebury, Marissa Jasinski, David Ackerman, Timothy Jewison, Tanvir Sajed, Vasuk Gautam, David S Wishart
  * [Paper](https://pmc.ncbi.nlm.nih.gov/articles/PMC10767804/)
  * [Platform](https://go.drugbank.com/)
  * Organizations: University of Alberta

* **Medicines, Diseases, Indications, and Contraindications (MeDIC): a foundational resource to support drug repurposing** 
  * Authors: Marcello DeLuca, Nico Matentzoglu, Elliott Sharp, Jane Li, Charlie Hempstead, May Lim, Piotr Kaniewski, E Kathleen Carter, Kushal Koirala, Elvin Ding, Laurens Vijnck, Pascal Brokmeier, Sabrina Toro, Kevin Schaper, Jacques Vergine, Olivia Li, Tudor I Oprea, David C Fajgenbaum, Christopher Bizon, Melissa Haendel, Alexander Tropsha
  * [Paper](https://doi.org/10.1093/nar/gkaf1312)
  * [Portal (RENCI)](https://medic.renci.org/)
  * Organizations: RENCI, UNC Chapel Hill, Every Cure

---

## Clinical Successes

Real-world validation of AI-driven drug repurposing with clinical impact.

* **Baricitinib for COVID-19 (BenevolentAI)** - First major AI-driven drug repurposing clinical success
  * [Paper (Frontiers in Pharmacology)](https://www.frontiersin.org/journals/pharmacology/articles/10.3389/fphar.2021.709856/full) | [Paper (The Lancet)](https://www.thelancet.com/journals/lancet/article/PIIS0140-6736(20)30304-4/fulltext)
  * Organizations: BenevolentAI, Eli Lilly

---

## Reviews

Essential review papers for understanding the drug repurposing field.

* **Knowledge Graphs for drug repurposing: a review of databases and methods** (2024)
  * Authors: Pablo Perdomo-Quinteiro, Alberto Belmonte-Hernández
  * [Paper (Briefings in Bioinformatics, 2024)](https://academic.oup.com/bib/article/25/6/bbae461/7774899)

* **The use of knowledge graphs for drug repurposing: From classical machine learning algorithms to graph neural networks** (2024)
  * Authors: Siqi Wei, Christo Sasi, Jelle Piepenbrock, Martijn A. Huynen, Peter A.C. ’t Hoen
  * [Paper (Computer Methods and Programs in Biomedicine, 2024)](https://www.sciencedirect.com/science/article/pii/S0010482525012247)

* **Pioneering Computational Pharmacophenomics** (2024)
  * Authors: David C Fajgenbaum, Sally Nijim, Grant Mitchell, Matej Macak, Chris Bizon, Alexander Tropsha, David Koslicki
  * Vision paper for unlocking life-saving potential of existing medicines
  * [Paper (PubMed)](https://pubmed.ncbi.nlm.nih.gov/39909662/)
---

## Contributing

Contributions are welcome! Please read the [contribution guidelines](CONTRIBUTING.md) first. We particularly welcome additions of:
- Novel AI/ML methods specifically for drug repurposing
- New repurposing-specific datasets and tools
- Updates to existing entries

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0)

To the extent possible under law, the contributors have waived all copyright and related rights to this work.
