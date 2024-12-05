<h1 align="center"><b>Awesome-model-inversion-attack</b></h1>
<p align="center">
    <a href="https://github.com/AndrewZhou924/Awesome-model-inversion-attack/pulls"><img src="https://img.shields.io/badge/PRs-Welcome-green" alt="PRs"></a>
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="awesome"></a>
    <img src="https://img.shields.io/github/stars/AndrewZhou924/Awesome-model-inversion-attack?color=yellow&label=Star" alt="Stars" >
</p>

A curated list of resources for model inversion attack (MIA).

Please star or watch this repository to keep tracking the latest updates! Contributions are welcome!

## NEWS

- **[Nov/2024]** We release a comprehensive survey of model inversion attacks. Check the [paper](https://arxiv.org/pdf/2411.10023).

**Outlines:**

- [NEWS](#news)
- [What is the model inversion attack?](#what-is-the-model-inversion-attack)
- [Survey](#survey)
- [Computer vision domain](#computer-vision-domain)
- [Graph learning domain](#graph-learning-domain)
- [Natural language processing domain](#natural-language-processing-domain)
- [Tools](#tools)
- [Others](#others)
- [Related repositories](#related-repositories)
- [Star History](#star-history)

## What is the model inversion attack?

A model inversion attack is a privacy attack where the attacker is able to reconstruct the original samples that were used to train the synthetic model from the generated synthetic data set. (Mostly.ai)

The goal of model inversion attacks is to recreate training data or sensitive attributes.
(Chen et al, 2021.)

In model inversion attacks, a malicious user attempts to recover the private dataset used to train a supervised neural network. A successful model inversion attack should generate realistic and diverse samples that accurately describe each of the classes in the private dataset. (Wang et al, 2021.)

## Survey

- [arXiv 2024] Model Inversion Attacks: A Survey of Approaches and Countermeasures. [[paper]](https://arxiv.org/pdf/2411.10023)

- [Physical and Engineering Sciences 2024] Algorithms that remember: model inversion attacks and data protection law. [[paper]](https://royalsocietypublishing.org/doi/pdf/10.1098/rsta.2018.0083)

- [CSF 2023] SoK: Model Inversion Attack Landscape: Taxonomy, Challenges, and Future Roadmap [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10221914)

- [arXiv 2022] Trustworthy Graph Neural Networks: Aspects, Methods and Trends. [[paper]](https://arxiv.org/pdf/2205.07424.pdf)

- [arXiv 2022] A Survey of Trustworthy Graph Learning: Reliability, Explainability, and Privacy Protection. [[paper]](https://arxiv.org/pdf/2205.10014.pdf)

- [arXiv 2022] A Comprehensive Survey on Trustworthy Graph Neural Networks: Privacy, Robustness, Fairness, and Explainability. [[paper]](https://arxiv.org/pdf/2204.08570.pdf)

- [arXiv 2022] Federated Learning Attacks Revisited: A Critical Discussion of Gaps, Assumptions, and Evaluation Setups [[paper]](https://arxiv.org/pdf/2111.03363)

- [arXiv 2022] I Know What You Trained Last Summer: A Survey on Stealing Machine Learning Models and Defences [[paper]](https://arxiv.org/pdf/2206.08451)

- [arXiv 2021] Survey: Leakage and Privacy at Inference Time [[paper]](https://arxiv.org/pdf/2107.01614)

- [arXiv 2021] A Review of Confidentiality Threats Against Embedded Neural Network Models [[paper]](https://arxiv.org/pdf/2105.01401)

- [arXiv 2021] Membership Inference Attacks on Machine Learning: A Survey [[paper]](https://arxiv.org/pdf/2103.07853)

- [arXiv 2021] ML-Doctor: Holistic Risk Assessment of Inference Attacks Against Machine Learning Models [[paper]](https://arxiv.org/pdf/2102.02551)

- [IEEE Access 2020] Privacy and Security Issues in Deep Learning: A Survey [[paper]](https://ieeexplore.ieee.org/abstract/document/9294026)

- [arXiv 2020] A Survey of Privacy Attacks in Machine Learning [[paper]](https://arxiv.org/pdf/2007.07646)
- [arXiv 2020] Rethinking Privacy Preserving Deep Learning: How to Evaluate and Thwart Privacy Attacks [[paper]](https://arxiv.org/pdf/2006.11601)
- [arXiv 2020] An Overview of Privacy in Machine Learning [[paper]](https://arxiv.org/pdf/2005.08679)

## Computer vision domain

- [ICLR 2014] Intriguing properties of neural networks [[paper]](https://arxiv.org/pdf/1312.6199)

- [ICLR 2014] Deep Inside Convolutional Networks: Visualising Image Classification Models and Saliency Maps [[paper]](https://arxiv.org/pdf/1312.6034)
- [CVPR 2015] Understanding Deep Image Representations by Inverting Them [[paper]](https://openaccess.thecvf.com/content_cvpr_2015/papers/Mahendran_Understanding_Deep_Image_2015_CVPR_paper.pdf)
- [CVPR 2016] Inverting visual representations with convolutional networks [[paper]](https://arxiv.org/pdf/1506.02753)

- [NIPS 2016] Generating Images with Perceptual Similarity Metrics based on Deep Networks [[paper]](https://proceedings.neurips.cc/paper/2016/file/371bce7dc83817b7893bcdeed13799b5-Paper.pdf)

- [ICML 2022] Plug-In Inversion: Model-Agnostic Inversion for Vision with Data Augmentations [[paper]](https://proceedings.mlr.press/v162/ghiasi22a/ghiasi22a.pdf)

- [CVPR 2020] Dreaming to Distill: Data-free Knowledge Transfer via DeepInversion [[paper]](https://arxiv.org/pdf/1912.08795) [[code]](https://github.com/NVlabs/DeepInversion)

- [USENIX Security 2014] (black & white-box) Privacy in Pharmacogenetics: An End-to-End Case Study of Personalized Warfarin Dosing [[paper]](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf)

- [CCS 2015] (black & white-box) Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures [[paper]](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677) [[code1]](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip) [[code2]](https://github.com/yashkant/Model-Inversion-Attack) [[code3]](https://github.com/zhangzp9970/MIA) [[code4]](https://github.com/sarahsimionescu/simple-model-inversion)

- [IJCAI 2015] (white-box (defense)) Regression Model Fitting under Differential Privacy and Model Inversion Attack [[paper]](http://www.csce.uark.edu/~xintaowu/publ/ijcai15.pdf) [[code]](https://github.com/cxs040/Regression-Model-Fitting-under-Differential-Privacy-and-Model-Inversion-Attack-Source-Code)

- [CSF 2016] (black & white-box) A Methodology for Formalizing Model-Inversion Attacks [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL)

- [CCS 2017] (white-box) Machine Learning Models that Remember Too Much [[paper]](https://arxiv.org/pdf/1709.07886.pdf) [[code]](https://github.com/csong27/ml-model-remember)

- [PST 2017] (white-box) Model Inversion Attacks for Prediction Systems: Without knowledge of Non-Sensitive Attributes [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476925)

- [CSF 2018] (white-box) Privacy Risk in Machine Learning: Analyzing the Connection to Overfitting [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429311)

- [arXiv 2019] (white-box) An Attack-Based Evaluation Method for Differentially Private Learning Against Model Inversion Attack [[paper]](https://ieeexplore.ieee.org/document/8822435)

- [CVPR 2019] A style-based generator architecture for generative adversarial networks [[paper]](https://arxiv.org/pdf/2411.10023)

- [GLSVLSI 2019] (black-box (defense)) MLPrivacyGuard: Defeating Confidence Information based Model Inversion Attacks on Machine Learning Systems [[paper]](https://www.researchgate.net/profile/Tiago-Alves-13/publication/333136362_MLPrivacyGuard_Defeating_Confidence_Information_based_Model_Inversion_Attacks_on_Machine_Learning_Systems/links/5cddb94d92851c4eaba682d7/MLPrivacyGuard-Defeating-Confidence-Information-based-Model-Inversion-Attacks-on-Machine-Learning-Systems.pdf)

- [ACSAC 2019] (black & white-box) Model Inversion Attacks Against Collaborative Inference [[paper]](http://palms.ee.princeton.edu/system/files/Model+Inversion+Attack+against+Collaborative+Inference.pdf)

- [CCS 2019] (black-box) Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment [[paper]](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA) [[code]](https://github.com/zhangzp9970/TB-MIA)

- [arXiv 2019] (black-box) GAMIN: An Adversarial Approach to Black-Box Model Inversion [[paper]](https://arxiv.org/pdf/1909.11835.pdf)

- [CVPR 2020] (white-box) The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks [[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf) [[code]](https://github.com/AI-secure/GMI-Attack) [[video]](https://www.youtube.com/watch?v=_g-oXYMhz4M)

- [ICLR 2020] (white-box) Overlearning Reveals Sensitive Attributes [[paper]](https://arxiv.org/pdf/1905.11742.pdf)

- [APSIPA ASC 2020] (white-box) Deep Face Recognizer Privacy Attack: Model Inversion Initialization by a Deep Generative Adversarial Data Space Discriminator [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9306253&casa_token=AWugOvIe0I0AAAAA:9wICCkMcfoljMqooM-lgl8m-6F6-cEl-ClHgNkE1SV8mZwqvBIaJ1HDjT1RWLyBz_P7tdB51jQVL&tag=1)

- [USENIX Security 2020] (black-box) Updates-Leak: Data Set Inference and Reconstruction Attacks in Online Learning [[paper]](https://www.usenix.org/system/files/sec20-salem.pdf)

- [IoT-J 2020] (black-box) Attacking and Protecting Data Privacy in Edge-Cloud Collaborative Inference Systems [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9187880) [[code]](https://github.com/zechenghe/Inverse_Collaborative_Inference)

- [ECCV Workshop 2020] (black-box) Black-Box Face Recovery from Identity Features [[paper]](https://arxiv.org/pdf/2007.13635.pdf)

- [arXiv 2020] (white-box) MixCon: Adjusting the Separability of Data Representations for Harder Data Recovery [[paper]](https://arxiv.org/abs/2010.11463)

- [Globecom 2020] (white-box (defense)) Privacy Preserving Facial Recognition Against Model Inversion Attacks [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9322508)

- [Big Data 2020] (white-box (defense)) Broadening Differential Privacy for Deep Learning Against Model Inversion Attacks [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9378274)

- [AdvML 2020] (metric) Evaluation Indicator for Model Inversion Attack [[paper]](https://drive.google.com/file/d/1rl77BGtGHzZ8obWUEOoqunXCjgvpzE8d/view)

- [NeurIPS 2021] (white-box) Variational Model Inversion Attacks [[paper]](https://proceedings.neurips.cc/paper/2021/file/50a074e6a8da4662ae0a29edde722179-Paper.pdf) [[code]](https://github.com/wangkua1/vmi)

- [ICCV 2021] (white-box) Exploiting Explanations for Model Inversion Attacks [[paper]](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_Exploiting_Explanations_for_Model_Inversion_Attacks_ICCV_2021_paper.pdf)

- [ICCV 2021] (white-box) Knowledge-Enriched Distributional Model Inversion Attacks [[paper]](https://arxiv.org/pdf/2010.04092.pdf) [[code]](https://github.com/SCccc21/Knowledge-Enriched-DMI)

- [AAAI 2021] (white-box (defense)) Improving Robustness to Model Inversion Attacks via Mutual Information Regularization [[paper]](https://arxiv.org/pdf/2009.05241.pdf)

- [ICLR Workshop 2021] (black-box (defense)) Practical Defences Against Model Inversion Attacks for Split Neural Networks [[paper]](https://arxiv.org/pdf/2104.05743.pdf) [[code]](https://github.com/TTitcombe/Model-Inversion-SplitNN)

- [ICDE 2021] (white-box) Feature inference attack on model predictions in vertical federated learning [[paper]](https://arxiv.org/pdf/2010.10152) [[code]](https://github.com/xj231/featureinference-vfl)

- [DAC 2021] (black & white-box) PRID: Model Inversion Privacy Attacks in Hyperdimensional Learning Systems [[paper]](https://dl.acm.org/doi/abs/10.1109/DAC18074.2021.9586217)

- [CSR Workshops 2021] (black-box (defense)) Defending Against Model Inversion Attack by Adversarial Examples [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9527945)

- [ECML PKDD 2021] (black-box) Practical Black Box Model Inversion Attacks Against Neural Nets [[paper]](https://link.springer.com/chapter/10.1007/978-3-030-93733-1_3)

- [APSIPA 2021] (black-box) Model Inversion Attack against a Face Recognition System in a Black-Box Setting [[paper]](http://www.apsipa.org/proceedings/2021/pdfs/0001800.pdf)

- [ICML 2022] (white-box) Plug & Play Attacks: Towards Robust and Flexible Model Inversion Attacks [[paper]](https://arxiv.org/pdf/2201.12179.pdf) [[code]](https://github.com/LukasStruppek/Plug-and-Play-Attacks)

- [CVPR 2022] (black-box) Label-Only Model Inversion Attacks via Boundary Repulsion [[paper]](https://arxiv.org/pdf/2203.01925.pdf) [[code]](https://github.com/m-kahla/Label-Only-Model-Inversion-Attacks-via-Boundary-Repulsion)

- [CVPR 2022] (white-box (defense)) ResSFL: A Resistance Transfer Framework for Defending Model Inversion Attack in Split Federated Learning [[paper]](https://openaccess.thecvf.com/content/CVPR2022/html/Li_ResSFL_A_Resistance_Transfer_Framework_for_Defending_Model_Inversion_Attack_CVPR_2022_paper.html) [[code]](https://github.com/zlijingtao/ResSFL)

- [KDD 2022] (white-box (defense)) Bilateral Dependency Optimization: Defending Against Model-inversion Attacks [[paper]](https://arxiv.org/pdf/2206.05483.pdf) [[code]](https://github.com/xpeng9719/Defend_MI)

- [USENIX Security 2022] (holistic risk assessment) ML-DOCTOR: Holistic Risk Assessment of Inference Attacks Against Machine Learning Models [[paper]](https://www.usenix.org/system/files/sec22summer_liu-yugeng.pdf) [[code]](https://github.com/liuyugeng/ML-Doctor)

- [TIFS 2022] (white-box) Model Inversion Attack by Integration of Deep Generative Models: Privacy-Sensitive Face Generation From a Face Recognition System [[paper]](https://dl.acm.org/doi/abs/10.1109/TIFS.2022.3140687)

- [TIFS 2022] (black-box (defense)) One Parameter Defense—Defending Against Data Inference Attacks via Differential Privacy [[paper]](https://arxiv.org/pdf/2203.06580.pdf)

- [WACV 2022] (white-box) Reconstructing Training Data from Diverse ML Models by Ensemble Inversion [[paper]](https://arxiv.org/pdf/2111.03702.pdf)

- [ECCV 2022] (white-box) SecretGen: Privacy Recovery on Pre-trained Models via Distribution Discrimination [[paper]](https://arxiv.org/pdf/2207.12263.pdf)

- [WPES 2022] (black-box) UnSplit: Data-Oblivious Model Inversion, Model Stealing, and Label Inference Attacks Against Split Learning [[paper]](https://arxiv.org/pdf/2108.09033.pdf) [[code]](https://github.com/ege-erdogan/unsplit)

- [NDSS 2022] (white-box) MIRROR: Model Inversion for Deep Learning Network with High Fidelity [[paper]](https://www.cs.purdue.edu/homes/an93/static/papers/ndss2022_model_inversion.pdf) [[code]](https://github.com/njuaplusplus/mirror)

- [SP 2022] (white-box) Reconstructing Training Data with Informed Adversaries [[paper]](https://arxiv.org/abs/2201.04845)

- [BMVC 2022] (white-box) Privacy Vulnerability of Split Computing to Data-Free Model Inversion Attacks [[paper]](https://arxiv.org/abs/2107.06304)

- [NeurIPS 2022] (white-box) Reconstructing Training Data from Trained Neural Networks [[paper]](https://arxiv.org/abs/2206.07758)

- [ICASSP 2023] (black-box) Sparse Black-Box Inversion Attack with Limited Information [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10095514) [[code]](https://github.com/Tencent/TFace/tree/master/recognition)

- [CVPR 2023] (black-box) Breaching FedMD: Image Recovery via Paired-Logits Inversion Attack [[paper]](https://arxiv.org/pdf/2304.11436.pdf) [[code]](https://github.com/FLAIR-THU/PairedLogitsInversion)

- [AAAI 2023] (white-box) Pseudo Label-Guided Model Inversion Attack via Conditional Generative Adversarial Network [[paper]](https://arxiv.org/pdf/2302.09814.pdf) [[code]](https://github.com/lethesec/plg-mi-attack)

- [TDSC 2023] (black-box) C2FMI: Coarse-to-Fine Black-box Model Inversion Attack [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148574)

- [TDSC 2023] (black-box) Boosting Model Inversion Attacks with Adversarial Examples [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148576)

- [CVPR 2023] (black-box) Reinforcement Learning-Based Black-Box Model Inversion Attacks [[paper]](https://arxiv.org/pdf/2304.04625.pdf) [[code]](https://github.com/HanGyojin/RLB-MI)

- [CVPR 2023] (white-box) Re-thinking Model Inversion Attacks Against Deep Neural Networks [[paper]](https://arxiv.org/pdf/2304.01669.pdf) [[code]](https://github.com/sutd-visual-computing-group/Re-thinking_MI)

- [AAAI 2023] (black-box (defense)) Purifier: Defending Data Inference Attacks via Transforming Confidence Scores [[paper]](https://arxiv.org/pdf/2005.03915.pdf)

- [CCS 2023] (black-box) Unstoppable Attack: Label-Only Model Inversion via Conditional Diffusion Model [[paper]](https://arxiv.org/pdf/2307.08424.pdf)

- [TDSC 2023] C2FMI: Corse-to-Fine Black-Box Model Inversion Attack [[paper]](https://ieeexplore.ieee.org/document/10148574) [[code]](https://github.com/MiLabHITSZ/2022YeC2FMI)

- [ACSAC 2019] Model Inversion Attacks Against Collaborative Inference [[paper]](https://www.acsac.org/2019/program/final/1/167.pdf) [[code]](https://github.com/zechenghe/Inverse_Collaborative_Inference)

- [CCS 2021] Unleashing the tiger: Inference attacks on split learning [[paper]](https://arxiv.org/pdf/2012.02670) [[code]](https://github.com/pasquini-dario/SplitNN_FSHA)

- [USENIX Security 2014] Privacy in Pharmacogenetics: An End-to-End Case Study of Personalized Warfarin Dosing [[paper]](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf)

- [CVPR 2020] The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks [[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf)

- [IEEE Transactions on Information Forensics and Security 2023] A GAN-Based Defense Framework Against Model Inversion Attacks [[paper]](https://ieeexplore.ieee.org/document/10184476)

- [CVPR 2024] Model Inversion Robustness: Can Transfer Learning Help? [[paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Ho_Model_Inversion_Robustness_Can_Transfer_Learning_Help_CVPR_2024_paper.pdf) [[code]](https://hosytuyen.github.io/projects/TL-DMI)

- [KDD 2022] Bilateral Dependency Optimization: Defending Against Model-inversion Attacks [[paper]](https://arxiv.org/pdf/2206.05483)

- [ICLR 2024] Be Careful What You Smooth For: Label Smoothing Can Be a Privacy Shield but Also a Catalyst for Model Inversion Attacks [[paper]](https://arxiv.org/pdf/2310.06549) [[code]](https://github.com/LukasStruppek/Plug-and-Play-Attacks)

- [AAAI 2020] (black & white-box) Improving Robustness to Model Inversion Attacks via Mutual Information Regularization [[paper]](https://arxiv.org/pdf/2009.05241v1.pdf)

- [arXiv 2020] Defending Model Inversion and Membership Inference Attacks via Prediction Purification [[paper]](https://arxiv.org/pdf/2005.03915)

- [CSR 2021] Defending Against Model Inversion Attack by Adversarial Examples [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9527945)

## Graph learning domain

- [USENIX Security 2020] Stealing Links from Graph Neural Networks [[paper]](https://www.usenix.org/system/files/sec21-he-xinlei.pdf) [[code]](https://github.com/xinleihe/link_stealing_attack)

- [arXiv 2020] (black & white-box) Reducing Risk of Model Inversion Using Privacy-Guided Training [[paper]](https://arxiv.org/pdf/2006.15877.pdf)

- [MobiQuitous 2020] Quantifying Privacy Leakage in Graph Embedding [[paper]](https://arxiv.org/pdf/2010.00906.pdf) [[code]](https://github.com/vasishtduddu/GraphLeaks)

- [IJCAI 2021] (white-box) A Survey on Gradient Inversion: Attacks, Defenses and Future Directions [[paper]](https://arxiv.org/pdf/2206.07284.pdf)

- [ICDE 2021] (black-box) NetFense: Adversarial Defenses against Privacy Attacks on Neural Networks for Graph Data [[paper]](https://arxiv.org/pdf/2106.11865.pdf) [[code]](https://github.com/ICHproject/NetFense)

- [ICML 2021] DeepWalking Backwards: From Node Embeddings Back to Graphs [[paper]](http://proceedings.mlr.press/v139/chanpuriya21a/chanpuriya21a.pdf) [[code]](https://github.com/konsotirop/Invert_Embeddings)

- [IJCAI 2021] (white-box) GraphMI: Extracting Private Graph Data from Graph Neural Networks [[paper]](https://arxiv.org/pdf/2106.02820v1.pdf) [[code]](https://github.com/zaixizhang/GraphMI)

- [arXiv 2021] Node-Level Membership Inference Attacks Against Graph Neural Networks [[paper]](https://arxiv.org/pdf/2102.05429.pdf)

- [ICML 2021] DeepWalking Backwards: From Embeddings Back to Graphs [[paper]](https://proceedings.mlr.press/v139/chanpuriya21a/chanpuriya21a.pdf)

- [arXiv 2022] (black & white-box) A Comprehensive Survey on Trustworthy Graph Neural Networks: Privacy, Robustness, Fairness, and Explainability [[paper]](https://arxiv.org/pdf/2204.08570.pdf)

- [WWW 2022] Learning Privacy-Preserving Graph Convolutional Network with Partially Observed Sensitive Attributes [[paper]](https://dl.acm.org/doi/pdf/10.1145/3485447.3511975?casa_token=Xsle4t9cLdcAAAAA:Gmij-qWaTJ2esGVa-yzKNHqVOMzYyaIgdNcgGmEzHrVyMdwwf9idn3qBjkhCcQeRTvbAkaT6OxiwXsk)

- [USENIX Security 2022] Inference Attacks Against Graph Neural Networks [[paper]](https://www.usenix.org/system/files/sec22summer_zhang-zhikun.pdf) [[code]](https://github.com/Zhangzhk0819/GNN-Embedding-Leaks)

- [IEEE S&P 2022] Model Stealing Attacks Against Inductive Graph Neural Networks [[paper]](https://arxiv.org/pdf/2112.08331.pdf) [[code]](https://github.com/xinleihe/GNNStealing)

- [arXiv 2022] Differentially Private Graph Classification With GNNs [[paper]](https://arxiv.org/pdf/2202.02575.pdf)

- [arXiv 2022] GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation [[paper]](https://arxiv.org/pdf/2203.00949.pdf)

- [arXiv 2022] Sok: Differential Privacy on Graph-Structured Data[[paper]](https://arxiv.org/pdf/2203.09205.pdf)

- [arXiv 2022] Degree-Preserving Randomized Response for Graph Neural Networks under Local Differential Privacy [[paper]](https://arxiv.org/pdf/2202.10209.pdf)

- [arXiv 2022] Private Graph Extraction via Feature Explanations [[paper]](https://arxiv.org/pdf/2206.14724.pdf)

- [arXiv 2022] Privacy and Transparency in Graph Machine Learning: A Unified Perspective [[paper]](https://arxiv.org/pdf/2207.10896.pdf)

- [CCS 2022] Finding MNEMON: Reviving Memories of Node Embeddings [[paper]](https://arxiv.org/pdf/2204.06963.pdf)

- [IJIS 2022] Defense Against Membership Inference Attack in Graph Neural Networks Through Graph Perturbation [[paper]](https://link.springer.com/article/10.1007/s10207-022-00646-y)

- [TKDE 2022] Model Inversion Attacks against Graph Neural Networks [[paper]](https://arxiv.org/pdf/2209.07807.pdf)

- [ICML 2023] (white-box) On Strengthening and Defending Graph Reconstruction Attack with Markov Chain Approximation [[paper]](https://openreview.net/pdf?id=Vcl3qckVyh) [[code]](https://github.com/tmlr-group/MC-GRA)

- [SecureComm 2023] (white-box) Model Inversion Attacks on Homogeneous and Heterogeneous Graph Neural Networks [[paper]](https://arxiv.org/pdf/2310.09800)

## Natural language processing domain

- [USENIX Security 2019] The Secret Sharer: Evaluating and Testing Unintended Memorization in Neural Networks [[paper]](https://www.usenix.org/system/files/sec19-carlini.pdf)

- [USENIX Security 2020] (black-box) Extracting Training Data from Large Language Models [[paper]](https://arxiv.org/pdf/2012.07805.pdf) [[code]](https://arxiv.org/pdf/2012.07805.pdf)

- [S&P 2020] (black & white-box) Privacy Risks of General-Purpose Language Models [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9152761)

- [arXiv 2018] Privacy-preserving Neural Representations of Text [[paper]](https://arxiv.org/pdf/1808.09408)

- [arXiv 2015] Censoring Representations with an Adversary [[paper]](https://arxiv.org/pdf/1511.05897)

- [arXiv 2018] Adversarial Removal of Demographic Attributes from Text Data [[paper]](https://arxiv.org/pdf/1808.06640)

- [arXiv 2018] Towards Robust and Privacy-preserving Text Representations [[paper]](https://arxiv.org/pdf/1805.06093)

- [NIPS 2017] Controllable Invariance through Adversarial Feature Learning [[paper]](https://proceedings.neurips.cc/paper_files/paper/2017/file/8cb22bdd0b7ba1ab13d742e22eed8da2-Paper.pdf)

- [CCS 2020] (black & white-box) Information Leakage in Embedding Models [[paper]](https://arxiv.org/pdf/2004.00053.pdf)

- [EMNLP 2021] (white-box) TAG: Gradient Attack on Transformer-based Language Models [[paper]](https://arxiv.org/pdf/2103.06819.pdf)

- [CEUR Workshop 2021] (black-box) Dataset Reconstruction Attack against Language Models [[paper]](https://ceur-ws.org/Vol-2942/paper1.pdf)

- [arXiv 2022] (black-box) KART: Parameterization of Privacy Leakage Scenarios from Pre-trained Language Models [[paper]](https://arxiv.org/pdf/2101.00036v1.pdf) [[code]](https://github.com/yutanakamura-tky/kart)

- [arXiv 2022] (white-box) Text Revealer: Private Text Reconstruction via Model Inversion Attacks against Transformers [[paper]](https://arxiv.org/pdf/2209.10505.pdf)

- [ACL 2022] (white-box) Canary Extraction in Natural Language Understanding Models [[paper]](https://arxiv.org/pdf/2203.13920.pdf)

- [NAACL 2022] (white-box) Are Large Pre-Trained Language Models Leaking Your Personal Information? [[paper]](https://aclanthology.org/2022.findings-emnlp.148.pdf) [[code]](https://github.com/jeffhj/LM_PersonalInfoLeak)

- [NeurIPS 2022] (white-box) Recovering Private Text in Federated Learning of Language Models [[paper]](https://arxiv.org/pdf/2205.08514.pdf) [[code]](https://github.com/princeton-sysml/film)

- [ACL 2023] (black-box) Sentence Embedding Leaks More Information than You Expect: Generative Embedding Inversion Attack to Recover the Whole Sentence [[paper]](https://arxiv.org/pdf/2305.03010.pdf) [[code]](https://github.com/hkust-knowcomp/geia)

- [arXiv 2023] (white-box) Deconstructing Classifiers: Towards A Data Reconstruction Attack Against Text Classification Models [[paper]](https://arxiv.org/pdf/2306.13789.pdf)

- [SaTML 2023] (black-box) Model Inversion Attack with Least Information and an In-depth Analysis of its Disparate Vulnerability [[paper]](https://openreview.net/pdf?id=x42Lo6Mkcrf)

- [EMNLP 2023] (black-box) Text Embeddings Reveal (Almost) As Much As Text [[paper]](https://arxiv.org/abs/2311.13647) [[code]](https://github.com/jxmorris12/vec2text)

- [ACL 2024] (black-box) Text Embedding Inversion Security for Multilingual Language Models [[paper]](https://arxiv.org/abs/2401.12192) [[code]](https://github.com/siebeniris/multivec2text)

- [EMNLP 2024] (black-box) Extracting Prompts by Inverting LLM Outputs [[paper]](https://arxiv.org/pdf/2405.15012) [[code]](https://github.com/collinzrj/output2prompt)

- [arXiv 2024] (white-box) Do Membership Inference Attacks Work on Large Language Models? [[paper]](https://arxiv.org/pdf/2402.07841.pdf)

- [ICLR 2024] (black-box) Language Model Inversion [[paper]](https://arxiv.org/abs/2311.13647) [[code]](https://github.com/jxmorris12/vec2text)

- [ACL 2024] (black-box) Transferable Embedding Inversion Attack: Uncovering Privacy Risks in Text Embeddings without Model Queries [[paper]](https://aclanthology.org/2024.acl-long.230/)

- [COLM 2024] Effective Prompt Extraction from Language Models [[paper]](https://openreview.net/forum?id=0o95CVdNuz#discussion)

## Tools

- [AIJack](https://github.com/Koukyosyumei/AIJack): Implementation of algorithms for AI security.

- [Privacy-Attacks-in-Machine-Learning](https://github.com/shrebox/Privacy-Attacks-in-Machine-Learning): Membership Inference, Attribute Inference and Model Inversion attacks implemented using PyTorch.

- [ml-attack-framework](https://github.com/Pilladian/ml-attack-framework): Universität des Saarlandes - Privacy Enhancing Technologies 2021 - Semester Project.

- (Trail of Bits) PrivacyRaven [[GitHub]](https://github.com/trailofbits/PrivacyRaven)

- (TensorFlow) TensorFlow Privacy [[GitHub]](https://github.com/tensorflow/privacy/tree/master/tensorflow_privacy/privacy/membership_inference_attack)

- (NUS Data Privacy and Trustworthy Machine Learning Lab) Machine Learning Privacy Meter [[GitHub]](https://github.com/privacytrustlab/ml_privacy_meter)

- (IQT Labs/Lab 41) CypherCat (archive-only) [[GitHub]](https://github.com/Lab41/cyphercat)

- (IBM) Adversarial Robustness Toolbox (ART) [[GitHub]](https://github.com/Trusted-AI/adversarial-robustness-toolbox)

## Attacks against synthetic data

- [arXiv 2023] A Linear Reconstruction Approach for Attribute Inference Attacks against Synthetic Data [[paper]](https://arxiv.org/pdf/2301.10053) [[code]](https://github.com/synthetic-society/recon-synth)
- [USENIX 2022] Synthetic Data - Anonymisation of Groundhog Day [[paper]](https://www.usenix.org/system/files/sec22summer_stadler.pdf) [[code]](https://github.com/spring-epfl/synthetic_data_release)

## Others

- [Blog 2020] Uncovering a model's secrets [[blog1]](https://gab41.lab41.org/uncovering-a-models-secrets-model-inversion-part-i-ce460eab93d6) [[blog2]](https://gab41.lab41.org/robust-or-private-model-inversion-part-ii-94d54fd8d4a5)
- [Blog 2020] Attacks against Machine Learning Privacy (Part 1): Model Inversion Attacks with the IBM-ART Framework [[blog]](https://franziska-boenisch.de/posts/2020/12/model-inversion/)
- [Slides 2020] ML and DP [[slides]](https://www.cs.toronto.edu/~toni/Courses/Fairness/Lectures/ML-and-DP-v2.pdf)

## Related repositories

- awesome-ml-privacy-attacks [[repo]](https://github.com/stratosphereips/awesome-ml-privacy-attacks#reconstruction)

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=AndrewZhou924/Awesome-model-inversion-attack&type=Date)](https://star-history.com/#AndrewZhou924/Awesome-model-inversion-attack&Date)
