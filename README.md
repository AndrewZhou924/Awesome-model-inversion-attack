# Awesome-model-inversion-attack

A curated list of resources for model inversion attack (MIA).

### What is the model inversion attack?
In model inversion attacks, a malicious user attempts to recover the private dataset used to train a supervised neural network. A successful model inversion attack should generate realistic and diverse samples that accurately describe each of the classes in the private dataset.

(by Variational Model Inversion Attacks, Wang et al, 2021.)

### Survey
Arxiv 2021 - A Survey of Privacy Attacks in Machine Learning.
[[paper]](https://arxiv.org/pdf/2007.07646.pdf)

Arxiv 2022 - A Comprehensive Survey on Trustworthy Graph Neural Networks: Privacy, Robustness, Fairness, and Explainability.
[[paper]](https://arxiv.org/pdf/2204.08570.pdf)

Arxiv 2022 - Trustworthy Graph Neural Networks: Aspects, Methods and Trends.
[[paper]](https://arxiv.org/pdf/2205.07424.pdf)

Arxiv 2022 - A Survey of Trustworthy Graph Learning: Reliability, Explainability, and Privacy Protection.
[[paper]](https://arxiv.org/pdf/2205.10014.pdf)


### General domain (including the computer vision)

USENIX Security 2014 - Privacy in Pharmacogenetics: An End-to-End Case Study of Personalized Warfarin Dosing.
[[paper]](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf)

CCS 2015 - Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677)
[[code1]](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip)
[[code2]](https://github.com/yashkant/Model-Inversion-Attack)
[[code3]](https://github.com/zhangzp9970/MIA)
[[code4]](https://github.com/sarahsimionescu/simple-model-inversion)

CSF 2016 - A Methodology for Formalizing Model-Inversion Attacks.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL)

CCS 2019 - Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA)
[[code]](https://github.com/zhangzp9970/TB-MIA)

Arxiv 2019 - Adversarial Neural Network Inversion via Auxiliary Knowledge Alignment.
[[paper]](https://arxiv.org/pdf/1902.08552.pdf)

CVPR 2020 - The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks.
[[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf)
[[code]](https://github.com/AI-secure/GMI-Attack)
[[video]](https://www.youtube.com/watch?v=_g-oXYMhz4M)

APSIPA ASC 2020 - Deep Face Recognizer Privacy Attack: Model Inversion Initialization by a Deep Generative Adversarial Data Space Discriminator.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9306253&casa_token=AWugOvIe0I0AAAAA:9wICCkMcfoljMqooM-lgl8m-6F6-cEl-ClHgNkE1SV8mZwqvBIaJ1HDjT1RWLyBz_P7tdB51jQVL&tag=1)

CCS 2021 - Membership Leakage in Label-Only Exposures.
[[paper]](https://yangzhangalmo.github.io/papers/CCS21-Label.pdf)
[[code]](https://github.com/zhenglisec/decision-based-mia)

CCS 2021 - Black-box adversarial attacks on commercial speech platforms with minimal information.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/3460120.3485383)

CCS 2021 - Unleashing the tiger: Inference attacks on split learning
[[paper]](https://dl.acm.org/doi/pdf/10.1145/3460120.3485259)
[[code]](https://github.com/pasquini-dario/SplitNN_FSHA)

CVPR 2021 - See through gradients: Image batch recovery via gradinversion.
[[paper]](http://openaccess.thecvf.com/content/CVPR2021/papers/Yin_See_Through_Gradients_Image_Batch_Recovery_via_GradInversion_CVPR_2021_paper.pdf)

CVPR 2021 - Soteria: Provable defense against privacy leakage in federated learning from representation perspective.
[[paper]](https://openaccess.thecvf.com/content/CVPR2021/papers/Sun_Soteria_Provable_Defense_Against_Privacy_Leakage_in_Federated_Learning_From_CVPR_2021_paper.pdf)
[[code]](https://github.com/jeremy313/Soteria)

CVPR 2021 - Imagine: Image synthesis by image-guided model inversion.
[[paper]](https://openaccess.thecvf.com/content/CVPR2021/papers/Wang_IMAGINE_Image_Synthesis_by_Image-Guided_Model_Inversion_CVPR_2021_paper.pdf)


NeurIPS 2021 - Variational Model Inversion Attacks.
[[paper]](https://proceedings.neurips.cc/paper/2021/file/50a074e6a8da4662ae0a29edde722179-Paper.pdf)
[[code]](https://github.com/wangkua1/vmi)

ICCV 2021 - Exploiting Explanations for Model Inversion Attacks.
[[paper]](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_Exploiting_Explanations_for_Model_Inversion_Attacks_ICCV_2021_paper.pdf)

ICCV 2021 - Knowledge-Enriched Distributional Model Inversion Attacks.
[[paper]](https://arxiv.org/pdf/2010.04092.pdf)
[[code]](https://github.com/SCccc21/Knowledge-Enriched-DMI)

AAAI 2021 - Improving Robustness to Model Inversion Attacks via Mutual Information Regularization.
[[paper]](https://arxiv.org/pdf/2009.05241.pdf)

ICML 2021 - Label-Only Membership Inference Attack.
[[paper]](http://proceedings.mlr.press/v139/choquette-choo21a/choquette-choo21a.pdf)
[[code]](https://github.com/cchoquette/membership-inference)

ICML 2021 - When Does Data Augmentation Help With Membership Inference Attacks?
[[paper]](When Does Data Augmentation Help With Membership Inference Attacks?)

ICLR 2021 workshop - PRACTICAL DEFENCES AGAINST MODEL INVERSION ATTACKS FOR SPLIT NEURAL NETWORKS.
[[paper]](https://arxiv.org/pdf/2104.05743.pdf)
[[code]](https://github.com/TTitcombe/Model-Inversion-SplitNN)
[[video]](https://crossminds.ai/video/practical-defences-against-model-inversion-attacks-for-split-neural-networks-60c3cee46af07cfaf7325850/)

ICDE 2021 Feature inference attack on model predictions in vertical federated learning.
[[paper]](https://arxiv.org/pdf/2010.10152)
[[code]](https://github.com/xj231/featureinference-vfl)

DAC 2021 - PRID: Model Inversion Privacy Attacks in Hyperdimensional Learning Systems
[[paper]](https://dl.acm.org/doi/abs/10.1109/DAC18074.2021.9586217)

ICSE 2021 - Robustness of on-device models: Adversarial attack to deep learning models on android apps.
[[paper]](https://arxiv.org/pdf/2101.04401)

ICML 2022 - Plug & Play Attacks: Towards Robust and Flexible Model Inversion Attacks.
[[paper]](https://arxiv.org/pdf/2201.12179.pdf)
[[code]](https://github.com/LukasStruppek/Plug-and-Play-Attacks)

CVPR 2022 - Label-Only Model Inversion Attacks via Boundary Repulsion.
[[paper]](https://arxiv.org/pdf/2203.01925.pdf)
[[code]](https://github.com/m-kahla/Label-Only-Model-Inversion-Attacks-via-Boundary-Repulsion)

CVPR 2022 - ResSFL: A Resistance Transfer Framework for Defending Model Inversion Attack in Split Federated Learning.
[[paper]](https://openaccess.thecvf.com/content/CVPR2022/html/Li_ResSFL_A_Resistance_Transfer_Framework_for_Defending_Model_Inversion_Attack_CVPR_2022_paper.html)
[[code]](https://github.com/zlijingtao/ResSFL)

KDD 2022 - Bilateral Dependency Optimization: Defending Against Model-inversion Attacks.
[[paper]](https://arxiv.org/pdf/2206.05483.pdf)
[[code]](https://github.com/xpeng9719/Defend_MI)

USENIX Security 2022 - ML-DOCTOR: Holistic Risk Assessment of Inference Attacks Against Machine Learning Models.
[[paper]](https://www.usenix.org/system/files/sec22summer_liu-yugeng.pdf)
[[code]](https://github.com/liuyugeng/ML-Doctor)

IEEE 2022 - An Approximate Memory based Defense against Model Inversion Attacks to Neural Networks.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9792582&casa_token=ymT57RhNhGEAAAAA:WsQHMpv77-4uyIp7l-p4hc7_Qmxvn5TeNpS5F7LHBFHyLay2O8Pe5eWqsKN2fu56v98NZsRrqeit)
[[code]](https://github.com/katekemu/model_inversion_defense)

TIFS 2022 - Model Inversion Attack by Integration of Deep Generative Models: Privacy-Sensitive Face Generation From a Face Recognition System
[[paper]](https://dl.acm.org/doi/abs/10.1109/TIFS.2022.3140687)


### Graph learning domain

USENIX Security 2020 - Stealing Links from Graph Neural Networks.
[[paper]](https://www.usenix.org/system/files/sec21-he-xinlei.pdf)

IJCAI 2021 - GraphMI: Extracting Private Graph Data from Graph Neural Networks.
[[paper]](https://arxiv.org/pdf/2106.02820)
[[code]](https://github.com/zaixizhang/GraphMI)

Arxiv 2021 - Node-Level Membership Inference Attacks Against Graph Neural Networks.
[[paper]](https://arxiv.org/pdf/2102.05429.pdf)

WWW 2022 - Learning Privacy-Preserving Graph Convolutional Network with Partially Observed Sensitive Attributes.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/3485447.3511975?casa_token=Xsle4t9cLdcAAAAA:Gmij-qWaTJ2esGVa-yzKNHqVOMzYyaIgdNcgGmEzHrVyMdwwf9idn3qBjkhCcQeRTvbAkaT6OxiwXsk)

USENIX Security 2022 - Inference Attacks Against Graph Neural Networks
[[paper]](https://www.usenix.org/system/files/sec22summer_zhang-zhikun.pdf)
[[code]](https://github.com/Zhangzhk0819/GNN-Embedding-Leaks)

IEEE S&P 2022 - Model Stealing Attacks Against Inductive Graph Neural Networks.
[[paper]](https://arxiv.org/pdf/2112.08331.pdf)
[[code]](https://github.com/xinleihe/GNNStealing)

Arxiv 2022 - DIFFERENTIALLY PRIVATE GRAPH CLASSIFICATION WITH GNNS.
[[paper]](https://arxiv.org/pdf/2202.02575.pdf)

Arxiv 2022 - GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation.
[[paper]](https://arxiv.org/pdf/2203.00949.pdf)

Arxiv 2022 - SOK: DIFFERENTIAL PRIVACY ON GRAPH-STRUCTURED DATA.
[[paper]](https://arxiv.org/pdf/2203.09205.pdf)

Arxiv 2022 - Degree-Preserving Randomized Response for Graph Neural Networks under Local Differential Privacy.
[[paper]](https://arxiv.org/pdf/2202.10209.pdf)

Arxiv 2022 - Private Graph Extraction via Feature Explanations.
[[paper]](https://arxiv.org/pdf/2206.14724.pdf)

### NLP domain

USENIX Security 2021 - Extracting training data from large language models.
[[paper]](https://www.usenix.org/system/files/sec21-carlini-extracting.pdf)

### Tools
[AIJack](https://github.com/Koukyosyumei/AIJack): Implementation of algorithms for AI security.

[Privacy-Attacks-in-Machine-Learning](https://github.com/shrebox/Privacy-Attacks-in-Machine-Learning): Membership Inference, Attribute Inference and Model Inversion attacks implemented using PyTorch.

[ml-attack-framework](https://github.com/Pilladian/ml-attack-framework): Universität des Saarlandes - Privacy Enhancing Technologies 2021 - Semester Project.


### Others
2021 - ML and DP.
[[slides]](https://www.cs.toronto.edu/~toni/Courses/Fairness/Lectures/ML-and-DP-v2.pdf)
