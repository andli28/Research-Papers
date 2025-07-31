# Research-Papers
These are the papers I find interesting, mostly focused around the intersection of **security, privacy, and ML**.
I may also list papers relating to the fundamentals of ML/FL infrastructure, or topics involving AI alignment and fairness.
There also might be non-papers in here! I am including whatever helps me grasp the concepts the easiest.

See [OpenMined](https://blog.openmined.org/federated-learning-types/) for a brief overview of the types of FL.

This list will be organized by topic and attack model (if applicable).

## Table of Contents
- [Research Papers](#research-papers)
    - [Table of Contents](#table-of-contents)
  - [Privacy](#privacy)
    - [Defenses](#defenses)
  - [Security](#security)
    - [Attacks](#attacks)
    - [Defenses](#defenses)
  - [Vertical FL](#vertical-fl)  
  - [FL Optimization](#fl-optimization)
  - [FL Systems from big tech companies](#fl-systems-from-big-tech-companies)
    - [Paper](#paper)
  - [Data Center Architecture](#data-center-architecture)
  - [Surveys](#surveys)
  - [LLMs](#llms)
  - [MLSys](#mlsys)
  - [Other FL Paper Lists](other-fl-paper-lists)
  - [Other Lists](other-lists)

## Privacy 

### Defenses
- **IBM (Cloud'22)**: DeTrust-FL: Privacy-Preserving Federated Learning in Decentralized Trust Setting [`PDF`](https://arxiv.org/pdf/2207.07779.pdf)


## Security

### Attacks

>Model Poisoning
- **(ICML'19)**: Analyzing Federated Learning through an Adversarial Lens [`PDF`](https://arxiv.org/pdf/1811.12470.pdf) [`Github`](https://github.com/inspire-group/ModelPoisoning)
    - **Attack Model**: "Single, non-colluding malicious agent where the adversarial objective is to cause the model to mis-classify a set of chosen inputs with high confidence." 

### Defenses

>Model Poisoning
- Federated Learning based on Defending Against Data Poisoning Attacks in IoT [`PDF`](https://arxiv.org/pdf/2209.06397.pdf)
    - **Attack Model**: "A group of p<n/2 malicious label-flipping poisoning attackers, where n is the total amount of participants’ clients." 
    
- **(NeurIPS'21)**: FL-WBC: Enhancing Robustness against Model Poisoning Attacks in Federated Learning from a Client Perspective [`PDF`](https://arxiv.org/pdf/2110.13864.pdf) [`Github`](https://github.com/jeremy313/FL-WBC)
   - **Attack Model**: "Clients mitigate **model poisoning attacks that have already polluted the global model**"



## Vertical FL
- Vertical Federated Learning: Challenges, Methodologies and Experiments [`PDF`](https://arxiv.org/pdf/2202.04309.pdf)

## FL Optimization
- Oort: Efficient Federated Learning via Guided Participant Selection[`PDF`](https://www.usenix.org/conference/osdi21/presentation/lai) | OSDI 21 🎓
- **(ICML'22)**: Neural Tangent Kernel Empowered Federated Learning [`PDF`](https://arxiv.org/pdf/2110.03681.pdf)
    - Reduces communication rounds, addresses statistical heterogeneity by transmitting update data that is more expressive than simple model weights/gradients
- Fed-SNN: Federated Learning with Spiking Neural Networks [`PDF`](https://arxiv.org/pdf/2106.06579v1.pdf) [`Github`](https://github.com/Intelligent-Computing-Lab-Yale/FedSNN)
    - Optimizes for energy efficiency
- Swan: A Neural Engine for Efficient DNN Training on Smartphone SoCs [`PDF`](https://arxiv.org/pdf/2206.04687.pdf)
- **(ICLR 2021)**: Federated Learning via Posterior Averaging: A New Perspective and Practical Algorithms [`PDF`](https://arxiv.org/pdf/2010.05273.pdf) [`Github`](https://github.com/alshedivat/fedpa)


## FL Systems from big tech companies
### Paper

>Cross-device
- **Apple**:  Federated Evaluation and Tuning for On-Device Personalization: System Design & Applications | [`PDF`](https://arxiv.org/pdf/2102.08503.pdf), [`PDF`](https://docs-assets.developer.apple.com/ml-research/papers/learning-with-privacy-at-scale.pdf)
- **Google**: Towards Federated Learning at Scale: System Design | [`MLSys21`](https://arxiv.org/abs/1902.01046), [`Github`](https://www.tensorflow.org/federated)🎓
- **Meta**: Papaya: Practical, Private, and Scalable Federated Learning | [`MLSys22`](https://arxiv.org/abs/2111.04877) 🎓

## Data Center Architecture
- Yarn: [`PDF`](https://www.cse.ust.hk/~weiwa/teaching/Fall15-COMP6611B/reading_list/YARN.pdf)
    - Also see: [`GFG`](https://www.geeksforgeeks.org/hadoop-yarn-architecture/), [`Cloudera`](https://docs.cloudera.com/HDPDocuments/HDP3/HDP-3.0.0/data-operating-system/content/apache_yarn.html)
- Omega: [`PDF`](https://wiki.epfl.ch/edicpublic/documents/Candidacy%20exam/Schwarzkopf-1.pdf)
    - Also see: [`CS294`](https://people.eecs.berkeley.edu/~istoica/classes/cs294/15/notes/10-omega.pdf), [`CSUDH`](https://csc.csudh.edu/btang/seminar/slides/Omega-Matt_Levan.pdf)
- Tiresias: A GPU Cluster Manager for Distributed Deep Learning | [`PDF`](https://web.eecs.umich.edu/~mosharaf/Readings/Tiresias.pdf)
- Leap: Effectively Prefetching Remote Memory | [`PDF`](https://www.usenix.org/system/files/atc20-maruf.pdf), [`Github`](https://github.com/SymbioticLab/Leap) (USENIX'20)🎓
    - Two tricks: Prefetching pages wherever possible
    - Using more efficient data paths that allow them to discard the operating system’s irrelevant disk-access features.

## Surveys
- A survey on security and privacy of federated learning [`URL`](https://www.sciencedirect.com/science/article/abs/pii/S0167739X20329848)
- Survey on Federated Learning Threats: concepts, taxonomy on attacks and defences, experimental study and challenges [`PDF`](https://arxiv.org/pdf/2201.08135.pdf)

## LLMs
- In AI, is bigger always better? [`Nature`](https://doi.org/10.1038/d41586-023-00641-w)
- Voyager, An Open-Ended Embodied Agent with Large Language Models [`Website`](https://voyager.minedojo.org/)
    - Vector Database of skills (GPT-4 Generated Code). Keys are descriptions, while the Value is the code of "skills"
- MemGPT: Towards LLMs as Operating Systems [`PDF`](https://arxiv.org/pdf/2310.08560.pdf)
    - LLMs are constrained by limited context windows, hindering their utility in tasks like extended conversations and document analysis
    - MemGPT manages different memory tiers to provide the appearance of large memory resources through data movement between fast
and slow memory (similar to traditional OS virtual context management)

- Agent Hospital: A Simulacrum of Hospital with Evolvable Medical Agents [`arxiv`](https://arxiv.org/abs/2405.02957)
    - LLMs roleplay as doctors, nurses, patients
    - "After treating around ten thousand patients (real-world doctors may take over two years), the evolved doctor agent achieves a state-of-the-art accuracy of 93.06% on a subset of the MedQA dataset that covers major respiratory diseases."
- (Perhaps) Beyond Human Translation: Harnessing Multi-Agent Collaboration for Translating Ultra-Long Literary Texts [`arxiv`](https://arxiv.org/html/2405.11804v1)
- Titans: Learning to Memorize at Test Time [`arxiv`](https://arxiv.org/abs/2501.00663)
    - "We present a new neural long-term memory module that learns to memorize historical context and helps attention to attend to the current context while utilizing long past information"
    - Scales better than transformers for long context windows, maintains high accuracy
- Fairness through Difference Awareness: Measuring Desired Group Discrimination in LLMs [`arxiv`](https://arxiv.org/pdf/2502.01926)
    - "Our primary call to action in this work is to bring attention to the important notion of difference awareness."
- The Big LLM Architecture Comparison (July 2025) [`Substack`](https://magazine.sebastianraschka.com/p/the-big-llm-architecture-comparison)


## MLSys
- Hidden Technical Debt in Machine Learning Systems [`NeurIPS PDF`](https://proceedings.neurips.cc/paper/2015/file/86df7dcfd896fcaf2674f757a2463eba-Paper.pdf
- Autellix: An Efficient Serving Engine for LLM Agents as General Programs [`PDF`](https://arxiv.org/html/2502.13965v1)
    - Autellix's approach is to prioritizing calls based on total execution time. They introduce two non-clairvoyant scheduling algorithms that assume no prior workload knowledge of programs.
    - PLAS (Program-Level Attained Service) is for single-threaded programs and ATLAS (Adaptive Thread-Level Attained Service) is for multi-threaded programs represented as general, dynamic DAGs.
    - PLAS prioritizes LLM calls based on the current cumulative service, or execution times, of their source program. ATLAS generalizes that to the maximum cumulative service time across all threads in the same program.
    - The goal is to minimize waiting and enhance performance

## Other FL paper lists
- https://github.com/AmberLJC/FLsystem-paper/
- ***https://github.com/innovation-cat/Awesome-Federated-Machine-Learning
- https://github.com/chaoyanghe/Awesome-Federated-Learning
- https://github.com/weimingwill/awesome-federated-learning#resource-allocation
- https://github.com/youngfish42/Awesome-Federated-Learning-on-Graph-and-Tabular-Data#federated-learning-framework

## Other Lists
- [`UMich EECS 598: Systems for GenAI`](https://github.com/mosharaf/eecs598/tree/w24-genai)
