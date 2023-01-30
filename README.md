# Research-Papers
These are the papers I find interesting, mostly focused around the intersection of **security, privacy, and ML**.
I may also list papers relating to the fundamentals of ML/FL infrastructure, or topics involving AI alignment and fairness.

My current focus is the burgeoning field of FL.

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
  - [FL Systems from big tech companies](#fl-systems-from-big-tech-companies)
    - [Paper](#paper)
  - [Data Center Architecture](#data-center-architecture)
  - [Surveys](#surveys)
  - [Other FL Paper Lists](other-fl-paper-lists)

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

## Surveys
- A survey on security and privacy of federated learning [`URL`](https://www.sciencedirect.com/science/article/abs/pii/S0167739X20329848)
- Survey on Federated Learning Threats: concepts, taxonomy on attacks and defences, experimental study and challenges [`PDF`](https://arxiv.org/pdf/2201.08135.pdf)


## Other FL paper lists
- https://github.com/AmberLJC/FLsystem-paper/
- ***https://github.com/innovation-cat/Awesome-Federated-Machine-Learning
- https://github.com/chaoyanghe/Awesome-Federated-Learning
- https://github.com/weimingwill/awesome-federated-learning#resource-allocation
- https://github.com/youngfish42/Awesome-Federated-Learning-on-Graph-and-Tabular-Data#federated-learning-framework
