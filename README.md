<h1 align="center"><b>Awesome-model-inversion-attack</b></h1>
<p align="center">
    <a href="https://github.com/AndrewZhou924/Awesome-model-inversion-attack/pulls"><img src="https://img.shields.io/badge/PRs-Welcome-green" alt="PRs"></a>
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="awesome"></a>
    <img src="https://img.shields.io/github/stars/AndrewZhou924/Awesome-model-inversion-attack?color=yellow&label=Star" alt="Stars" >
</p>
A curated list of resources for model inversion attack (MIA).
If some related papers are missing, please contact us via pull requests.

**Outlines:**

[TOC]

## What is the model inversion attack?

A model inversion attack is a privacy attack where the attacker is able to reconstruct the original samples that were used to train the synthetic model from the generated synthetic data set. (Mostly.ai)

The goal of model inversion attacks is to recreate training data or sensitive attributes.
(Chen et al, 2021.)

In model inversion attacks, a malicious user attempts to recover the private dataset used to train a supervised neural network. A successful model inversion attack should generate realistic and diverse samples that accurately describe each of the classes in the private dataset. (Wang et al, 2021.)

## Survey
Arxiv 2021 - A Survey of Privacy Attacks in Machine Learning.
[[paper]](https://arxiv.org/pdf/2007.07646.pdf)

Arxiv 2022 - A Comprehensive Survey on Trustworthy Graph Neural Networks: Privacy, Robustness, Fairness, and Explainability.
[[paper]](https://arxiv.org/pdf/2204.08570.pdf)

Arxiv 2022 - Trustworthy Graph Neural Networks: Aspects, Methods and Trends.
[[paper]](https://arxiv.org/pdf/2205.07424.pdf)

Arxiv 2022 - A Survey of Trustworthy Graph Learning: Reliability, Explainability, and Privacy Protection.
[[paper]](https://arxiv.org/pdf/2205.10014.pdf)

Philosophical Transactions of the Royal Society A 2018. Algorithms that remember: model inversion attacks and data protection law.

[[paper]](https://royalsocietypublishing.org/doi/pdf/10.1098/rsta.2018.0083)


## Computer vision domain
| Year | Title | Adversarial Knowledge | Venue | Paper Link | Code Link |
| ---- | ----- | -------------------- | ----- | ---------- | --------- |
| 2014 | Privacy in pharmacogenetics: An end-to-end case study of personalized warfarin dosing | white-box | Security | [Paper](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf) | |
| 2015 | Model inversion attacks that exploit confidence information and basic countermeasures | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677) | [Code1](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip), [Code2](https://github.com/yashkant/Model-Inversion-Attack), [Code3](https://github.com/zhangzp9970/MIA), [Code4](https://github.com/sarahsimionescu/simple-model-inversion) |
| 2015 | Regression Model Fitting under Differential Privacy and Model Inversion Attack | | IJCAI | [Paper](http://www.csce.uark.edu/~xintaowu/publ/ijcai15.pdf) | [Code](https://github.com/cxs040/Regression-Model-Fitting-under-Differential-Privacy-and-Model-Inversion-Attack-Source-Code) |
| 2016 | A Methodology for Formalizing Model Inversion Attacks | | CSF | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL) | |
| 2017 | Machine Learning Models that Remember Too Much | | CCS | [Paper](https://arxiv.org/pdf/1709.07886.pdf) | [Code](https://github.com/csong27/ml-model-remember) |
| 2017 | Model inversion attacks for prediction systems: Without knowledge of non-sensitive attributes | | PST | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476925) | |
| 2018 | Privacy Risk in Machine Learning: Analyzing the Connection to Overfitting | | CSF | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429311) | |
| 2019 | MLPrivacyGuard: Defeating Confidence Information based Model Inversion Attacks on Machine Learning Systems | | GLSVLSI | [Paper](https://www.researchgate.net/profile/Tiago-Alves-13/publication/333136362_MLPrivacyGuard_Defeating_Confidence_Information_based_Model_Inversion_Attacks_on_Machine_Learning_Systems/links/5cddb94d92851c4eaba682d7/MLPrivacyGuard-Defeating_Confidence-Information-based-Model-Inversion-Attacks-on-Machine-Learning-Systems.pdf) | |
| 2019 | Model inversion attacks against collaborative inference | | ACSAC | [Paper](https://par.nsf.gov/servlets/purl/10208164) | [Code](https://github.com/zechenghe/Inverse_Collaborative_Inference) |
| 2019 | Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA) | [Code](https://github.com/zhangzp9970/TB-MIA) |
| 2019 | Exploiting Unintended Feature Leakage in Collaborative Learning | | S&P | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8835269) | [Code](https://github.com/csong27/property-inference-collaborative-ml) |
| 2019 | Adversarial Neural Network Inversion via Auxiliary Knowledge Alignment | | Arxiv | [Paper](https://arxiv.org/pdf/1902.08552.pdf) | |
| 2019 | GAMIN: An Adversarial Approach to Black-Box Model Inversion | | Arxiv | [Paper](https://arxiv.org/pdf/1909.11835.pdf) | |
| 2020 | The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks | | CVPR | [Paper](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf) | [Code](https://github.com/AI-secure/GMI-Attack), [Video](https://www.youtube.com/watch?v=_g-oXYMhz4M) |
| 2020 | Overlearning Reveals Sensitive Attributes | | ICLR | [Paper](https://arxiv.org/pdf/1905.11742.pdf) | |
| 2020 | Deep Face Recognizer Privacy Attack: Model Inversion Initialization by a Deep Generative Adversarial Data Space Discriminator | | APSIPA ASC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9306253&casa_token=AWugOvIe0I0AAAAA:9wICCkMcfoljMqooM-lgl8m-6F6-cEl-ClHgNkE1SV8mZwqvBIaJ1HDjT1RWLyBz_P7tdB51jQVL&tag=1) | |
| 2020 | Updates-Leak: Data Set Inference and Reconstruction Attacks in Online Learning | | USENIX Security | [Paper](https://www.usenix.org/system/files/sec20-salem.pdf) | |
| 2020 | Attacking and Protecting Data Privacy in Edge-Cloud Collaborative Inference Systems | | IoTJ | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9187880) | [Code](https://github.com/zechenghe/Inverse_Collaborative_Inference) |
| 2020 | Black-Box Face Recovery from Identity Features | | ECCV Workshop | [Paper](https://arxiv.org/pdf/2007.13635.pdf) | |
| 2020 | Defending model inversion and membership inference attacks via prediction purification | | Arxiv | [Paper](https://arxiv.org/pdf/2005.03915.pdf) | |
| 2020 | Generative model-inversion attacks against deep neural networks | white-box | CVPR | [Paper](https://arxiv.org/pdf/1911.07135.pdf) | [code](https://github.com/AI-secure/GMI-Attack) |
| 2020 | Privacy Preserving Facial Recognition Against Model Inversion Attacks | white-box | Globecom  | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9322508) |  |
| 2020 | Broadening Differential Privacy for Deep LearningAgainst Model Inversion Attacks  | white-box | Big Data | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9378274) |  |
| 2021 | Black-box adversarial attacks on commercial speech platforms with minimal information | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3460120.3485383) | |
| 2021 | Unleashing the tiger: Inference attacks on split learning | | CCS | [Paper](https://dl.acm.org/doi/pdf/10.1145/3460120.3485259) | [Code](https://github.com/pasquini-dario/SplitNN_FSHA) |
| 2021 | Soteria: Provable defense against privacy leakage in federated learning from representation perspective | | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2021/papers/Sun_Soteria_Provable_Defense_Against_Privacy_Leakage_in_Federated_Learning_From_CVPR_2021_paper.pdf) | [Code](https://github.com/jeremy313/Soteria) |
| 2021 | Variational Model Inversion Attacks | | NeurIPS | [Paper](https://proceedings.neurips.cc/paper/2021/file/50a074e6a8da4662ae0a29edde722179-Paper.pdf) | [Code](https://github.com/wangkua1/vmi) |
| 2021 | Exploiting Explanations for Model Inversion Attacks | | ICCV | [Paper](https://openaccess.thecvf.com/content/ICCV2021/papers/Zhao_Exploiting_Explanations_for_Model_Inversion_Attacks_ICCV_2021_paper.pdf) | |
| 2021 | Knowledge-Enriched Distributional Model Inversion Attacks | | ICCV | [Paper](https://arxiv.org/pdf/2010.04092.pdf) | [Code](https://github.com/SCccc21/Knowledge-Enriched-DMI) |
| 2021 | Improving Robustness to Model Inversion Attacks via Mutual Information Regularization | | AAAI | [Paper](https://arxiv.org/pdf/2009.05241.pdf) | |
| 2021 | Practical Defences Against Model Inversion Attacks for Split Neural Networks | | ICLR Workshop | [Paper](https://arxiv.org/pdf/2104.05743.pdf) | [Code](https://github.com/TTitcombe/Model-Inversion-SplitNN), [Video](https://crossminds.ai/video/practical-defences-against-model-inversion-attacks-for-split-neural-networks-60c3cee46af07cfaf7325850/) |
| 2021 | Feature Inference Attack on Model Predictions in Vertical Federated Learning | | ICDE | [Paper](https://arxiv.org/pdf/2010.10152) | [Code](https://github.com/xj231/featureinference-vfl) |
| 2021 | PRID: Model Inversion Privacy Attacks in Hyperdimensional Learning Systems | | DAC | [Paper](https://dl.acm.org/doi/abs/10.1109/DAC18074.2021.9586217) | |
| 2021 | Robustness of On-Device Models: Adversarial Attack to Deep Learning Models on Android Apps | | ICSE | [Paper](https://arxiv.org/pdf/2101.04401) | |
| 2021 | Defending Against Model Inversion Attack by Adversarial Examples | | CSR Workshops | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9527945) | |
| 2021 | Practical Black Box Model Inversion Attacks Against Neural Nets | black-box | ECML PKDD | [Paper](https://link.springer.com/content/pdf/10.1007/978-3-030-93733-1.pdf?pdf=button) |  |
| 2021 | Model Inversion Attack against a Face Recognition System in a Black-Box Setting | black-box | APSIPA | [Paper](http://www.apsipa.org/proceedings/2021/pdfs/0001800.pdf) |  |
| 2022 | Plug & Play Attacks: Towards Robust and Flexible Model Inversion Attacks | | ICML | [Paper](https://arxiv.org/pdf/2201.12179.pdf) | [Code](https://github.com/LukasStruppek/Plug-and-Play-Attacks) |
| 2022 | Label-Only Model Inversion Attacks via Boundary Repulsion | | CVPR | [Paper](https://arxiv.org/pdf/2203.01925.pdf) | [Code](https://github.com/m-kahla/Label-Only-Model-Inversion-Attacks-via-Boundary-Repulsion) |
| 2022 | ResSFL: A Resistance Transfer Framework for Defending Model Inversion Attack in Split Federated Learning | | CVPR | [Paper](https://openaccess.thecvf.com/content/CVPR2022/html/Li_ResSFL_A_Resistance_Transfer_Framework_for_Defending_Model_Inversion_Attack_CVPR_2022_paper.html) | [Code](https://github.com/zlijingtao/ResSFL) |
| 2022 | Bilateral Dependency Optimization: Defending Against Model-Inversion Attacks | | KDD | [Paper](https://arxiv.org/pdf/2206.05483.pdf) | [Code](https://github.com/xpeng9719/Defend_MI) |
| 2022 | ML-DOCTOR: Holistic Risk Assessment of Inference Attacks Against Machine Learning Models | | USENIX Security | [Paper](https://www.usenix.org/system/files/sec22summer_liu-yugeng.pdf) | [Code](https://github.com/liuyugeng/ML-Doctor) |
| 2022 | An Approximate Memory Based Defense Against Model Inversion Attacks to Neural Networks | | IEEE | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9792582&casa_token=ymT57RhNhGEAAAAA:WsQHMpv77-4uyIp7l-p4hc7_Qmxvn5TeNpS5F7LHBFHyLay2O8Pe5eWqsKN2fu56v98NZsRrqeit) | [Code](https://github.com/katekemu/model_inversion_defense) |
| 2022 | Model Inversion Attack by Integration of Deep Generative Models: Privacy-Sensitive Face Generation From a Face Recognition System | | TIFS | [Paper](https://dl.acm.org/doi/abs/10.1109/TIFS.2022.3140687) | |
| 2022 | Defending Against Reconstruction Attacks Through Differentially Private Federated Learning for Classification of Heterogeneous Chest X-Ray Data | | Arxiv | [Paper](https://arxiv.org/pdf/2205.03168.pdf) | |
| 2022 | One Parameter Defense—Defending Against Data Inference Attacks via Differential Privacy | black-box | TIFS | [Paper](https://arxiv.org/pdf/2203.06580.pdf) |  |
| 2022 | Reconstructing Training Data from Diverse ML Models by Ensemble Inversion | white-box | WACV | [Paper](https://arxiv.org/pdf/2111.03702.pdf) |  |
| 2022 | SecretGen: Privacy Recovery on Pre-trained Models via Distribution Discrimination | white-box | ECCV | [Paper](https://arxiv.org/pdf/2207.12263.pdf) |  |
| 2022 | UnSplit: Data-Oblivious Model Inversion, Model Stealing, andLabel Inference Attacks Against Split Learning | S | WPES | [Paper](https://arxiv.org/pdf/2108.09033.pdf) | [code](https://github.com/ege-erdogan/unsplit) |
| 2022 | MIRROR: Model Inversion for Deep LearningNetwork with High Fidelity | white-box | NDSS | [Paper](https://www.cs.purdue.edu/homes/an93/static/papers/ndss2022_model_inversion.pdf) | [code](https://github.com/njuaplusplus/mirror) |
| 2023 | Sparse Black-Box Inversion Attack with Limited Information | black-box | ICASSP | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10095514) | [code](https://github.com/Tencent/TFace/tree/master/recognition) |
| 2023 | Breaching FedMD: Image Recovery via Paired-Logits Inversion Attack | black-box | CVPR | [Paper](https://arxiv.org/pdf/2304.11436.pdf) | [code](https://github.com/FLAIR-THU/PairedLogitsInversion) |
| 2023 | Pseudo Label-Guided Model Inversion Attack via Conditional Generative Adversarial Network | white-box | AAAI | [Paper](https://arxiv.org/pdf/2302.09814.pdf) | [code](https://github.com/lethesec/plg-mi-attack) |
| 2023 | C2FMI: Corse-to-Fine Black-box Model Inversion Attack | black-box | TDSC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148574) |  |
| 2023 | Boosting Model Inversion Attacks with Adversarial Examples | black-box | TDSC | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148576) |  |
| 2023 | Reinforcement Learning-Based Black-Box Model Inversion Attacks | black-box | CVPR | [Paper](https://arxiv.org/pdf/2304.04625.pdf) | [code](https://github.com/HanGyojin/RLB-MI) |
| 2023 | Re-thinking Model Inversion Attacks Against Deep Neural Networks | white-box | CVPR | [Paper](https://arxiv.org/pdf/2304.01669.pdf) | [code](https://github.com/sutd-visual-computing-group/Re-thinking_MI) |

USENIX Security 2014 - Privacy in Pharmacogenetics: An End-to-End Case Study of Personalized Warfarin Dosing.
[[paper]](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf)

CCS 2015 - Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677)
[[code1]](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip)
[[code2]](https://github.com/yashkant/Model-Inversion-Attack)
[[code3]](https://github.com/zhangzp9970/MIA)
[[code4]](https://github.com/sarahsimionescu/simple-model-inversion)

IJCAI 2015 - Regression model fitting under differential privacy and model inversion attack.
[[paper]](http://www.csce.uark.edu/~xintaowu/publ/ijcai15.pdf)
[[code]](https://github.com/cxs040/Regression-Model-Fitting-under-Differential-Privacy-and-Model-Inversion-Attack-Source-Code)

CSF 2016 - A Methodology for Formalizing Model-Inversion Attacks.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL)

CCS 2017 - Machine Learning Models that Remember Too Much.
[[paper]](https://arxiv.org/pdf/1709.07886.pdf)
[[code]](https://github.com/csong27/ml-model-remember)

PST 2017 - Model inversion attacks for prediction systems: Without knowledge of non-sensitive attributes.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476925)

CSF 2018 - Privacy Risk in Machine Learning: Analyzing the Connection to Overfitting.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429311)

GLSVLSI 2019 - MLPrivacyGuard: Defeating Confidence Information based Model Inversion Attacks on Machine Learning Systems.
[[paper]](https://www.researchgate.net/profile/Tiago-Alves-13/publication/333136362_MLPrivacyGuard_Defeating_Confidence_Information_based_Model_Inversion_Attacks_on_Machine_Learning_Systems/links/5cddb94d92851c4eaba682d7/MLPrivacyGuard-Defeating-Confidence-Information-based-Model-Inversion-Attacks-on-Machine-Learning-Systems.pdf)

ACSAC  2019 - Model inversion attacks against collaborative inference.
[[paper]](https://par.nsf.gov/servlets/purl/10208164)
[[code]](https://github.com/zechenghe/Inverse_Collaborative_Inference)

CCS 2019 - Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA)
[[code]](https://github.com/zhangzp9970/TB-MIA)

IEEE S&P 2019 - Exploiting Unintended Feature Leakage in Collaborative Learning.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8835269)
[[code]](https://github.com/csong27/property-inference-collaborative-ml)

Arxiv 2019 - Adversarial Neural Network Inversion via Auxiliary Knowledge Alignment.
[[paper]](https://arxiv.org/pdf/1902.08552.pdf)

Arxiv 2019 - GAMIN: An Adversarial Approach to Black-Box Model Inversion.
[[paper]](https://arxiv.org/pdf/1909.11835.pdf)

CVPR 2020 - The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks.
[[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf)
[[code]](https://github.com/AI-secure/GMI-Attack)
[[video]](https://www.youtube.com/watch?v=_g-oXYMhz4M)

ICLR 2020 - OVERLEARNING REVEALS SENSITIVE ATTRIBUTES.
[[paper]](https://arxiv.org/pdf/1905.11742.pdf)

APSIPA ASC 2020 - Deep Face Recognizer Privacy Attack: Model Inversion Initialization by a Deep Generative Adversarial Data Space Discriminator.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9306253&casa_token=AWugOvIe0I0AAAAA:9wICCkMcfoljMqooM-lgl8m-6F6-cEl-ClHgNkE1SV8mZwqvBIaJ1HDjT1RWLyBz_P7tdB51jQVL&tag=1)

USENIX Security 2020 - Updates-Leak: Data Set Inference and Reconstruction Attacks in Online Learning.
[[paper]](https://www.usenix.org/system/files/sec20-salem.pdf)

IoTJ 2020 - Attacking and Protecting Data Privacy in Edge-Cloud Collaborative Inference Systems.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9187880)
[[code]](https://github.com/zechenghe/Inverse_Collaborative_Inference)

ECCV 2020 Workshop - Black-Box Face Recovery from Identity Features.
[[paper]](https://arxiv.org/pdf/2007.13635.pdf)

Arxiv 2020 - Defending model inversion and membership inference attacks via prediction purification.
[[paper]](https://arxiv.org/pdf/2005.03915.pdf)

CVPR 2020 - Generative model-inversion attacks against deep neural networks
[[paper]](https://arxiv.org/pdf/1911.07135.pdf)
[[code]](https://github.com/AI-secure/GMI-Attack)

Globecom 2020 - Privacy Preserving Facial Recognition Against Model Inversion Attacks
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9322508)

Big Data 2020 - Broadening Differential Privacy for Deep LearningAgainst Model Inversion Attacks 
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9378274)

IJCAI 2021 - Contrastive Model Inversion for Data-Free Knowledge Distillation.
[[paper]](https://www.ijcai.org/proceedings/2021/0327.pdf)
[[code]](https://github.com/zju-vipa/CMI)

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

CSR Workshops 2021 - Defending Against Model Inversion Attack by Adversarial Examples.
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=9527945)

ECML PKDD 2021 - Practical Black Box Model Inversion Attacks Against Neural Nets
[[paper]](https://link.springer.com/content/pdf/10.1007/978-3-030-93733-1.pdf?pdf=button)

APSIPA 2021 - Model Inversion Attack against a Face Recognition System in a Black-Box Setting
[[paper]](http://www.apsipa.org/proceedings/2021/pdfs/0001800.pdf)

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

Arxiv 2022 - Defending against Reconstruction Attacks through Differentially Private Federated Learning for Classification of Heterogeneous Chest X-Ray Data.
[[paper]](https://arxiv.org/pdf/2205.03168.pdf)

TIFS 2022 - One Parameter Defense—Defending Against Data Inference Attacks via Differential Privacy
[[paper]](https://arxiv.org/pdf/2203.06580.pdf)

WACV 2022 - Reconstructing Training Data from Diverse ML Models by Ensemble Inversion
[[paper]](https://arxiv.org/pdf/2111.03702.pdf)

ECCV 2022 - SecretGen: Privacy Recovery on Pre-trained Models via Distribution Discrimination
[[paper]](https://arxiv.org/pdf/2207.12263.pdf)

WPES 2022- UnSplit: Data-Oblivious Model Inversion, Model Stealing, andLabel Inference Attacks Against Split Learning
[[paper]](https://arxiv.org/pdf/2108.09033.pdf)
[[code]](https://github.com/ege-erdogan/unsplit)

NDSS 2022 - MIRROR: Model Inversion for Deep LearningNetwork with High Fidelity
[[paper]](https://www.cs.purdue.edu/homes/an93/static/papers/ndss2022_model_inversion.pdf)
[[code]](https://github.com/njuaplusplus/mirror) |

ICASSP 2023 - Sparse Black-Box Inversion Attack with Limited Information
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10095514)
[[code]](https://github.com/Tencent/TFace/tree/master/recognition)

CVPR 2023 - Breaching FedMD: Image Recovery via Paired-Logits Inversion Attack
[[paper]](https://arxiv.org/pdf/2304.11436.pdf)
[[code]](https://github.com/FLAIR-THU/PairedLogitsInversion)

AAAI 2023 - Pseudo Label-Guided Model Inversion Attack via Conditional Generative Adversarial Network
[[paper]](https://arxiv.org/pdf/2302.09814.pdf)
[[code]](https://github.com/lethesec/plg-mi-attack)

TDSC 2023 - C2FMI: Corse-to-Fine Black-box Model Inversion Attack
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148574)

TDSC 2023 - Boosting Model Inversion Attacks with Adversarial Examples
[[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148576)

CVPR 2023 - Reinforcement Learning-Based Black-Box Model Inversion Attacks
[[paper]](https://arxiv.org/pdf/2304.04625.pdf)
[[code]](https://github.com/HanGyojin/RLB-MI)

CVPR 2023 - Re-thinking Model Inversion Attacks Against Deep Neural Networks
[[paper]](https://arxiv.org/pdf/2304.01669.pdf) 
[[code]](https://github.com/sutd-visual-computing-group/Re-thinking_MI) |

## Graph learning domain
| Year | Title | Adversarial Knowledge | Venue | Paper Link | Code Link |
| ---- | ----- | -------------------- | ----- | ---------- | --------- |
| 2020 | Improving Robustness to Model Inversion Attacks via Mutual Information Regularization |  black & white-box | AAAI | [Paper](https://arxiv.org/pdf/2009.05241v1.pdf) |  |
| 2020 | Reducing Risk of Model Inversion Using Privacy-Guided Training |  black & white-box | Arxiv | [Paper](https://arxiv.org/pdf/2006.15877.pdf) |  |
| 2021 | A Survey on Gradient Inversion: Attacks, Defenses and Future Directions |  white-box | IJCAI | [Paper](https://arxiv.org/pdf/2206.07284.pdf) |  |
| 2021 | GraphMI: Extracting Private Graph Data from Graph Neural Networks |  white-box | IJCAI | [Paper](https://arxiv.org/pdf/2106.02820v1.pdf) | [code](https://github.com/zaixizhang/GraphMI) |
| 2021 | NetFense: Adversarial Defenses against Privacy Attacks on Neural Networks for Graph Data |  black-box | ICDE | [Paper](https://arxiv.org/pdf/2106.11865.pdf) | [code](https://github.com/ICHproject/NetFense) |
| 2022 | A Comprehensive Survey on Trustworthy Graph Neural Networks: Privacy, Robustness, Fairness, and Explainability |  black & white-box | Arxiv | [Paper](https://arxiv.org/pdf/2204.08570.pdf) |  |

USENIX Security 2020 - Stealing Links from Graph Neural Networks.
[[paper]](https://www.usenix.org/system/files/sec21-he-xinlei.pdf)
[[code]](https://github.com/xinleihe/link_stealing_attack)

MobiQuitous 2020 - Quantifying Privacy Leakage in Graph Embedding.
[[paper]](https://arxiv.org/pdf/2010.00906.pdf)
[[code]](https://github.com/vasishtduddu/GraphLeaks)

ICML 2021 - DeepWalking Backwards: From Node Embeddings Back to Graphs.
[[paper]](http://proceedings.mlr.press/v139/chanpuriya21a/chanpuriya21a.pdf)
[[code]](https://github.com/konsotirop/Invert_Embeddings)

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

Arxiv 2022 - Privacy and Transparency in Graph Machine Learning: A Unified Perspective.
[[paper]](https://arxiv.org/pdf/2207.10896.pdf)

CCS 2022 - Finding MNEMON: Reviving Memories of Node Embeddings.
[[paper]](https://arxiv.org/pdf/2204.06963.pdf)

IJIS 2022 - Defense against membership inference attack in graph neural networks through graph perturbation.
[[paper]](https://link.springer.com/article/10.1007/s10207-022-00646-y)

TKDE 2022 - Model Inversion Attacks against Graph Neural Networks.
[[paper]](https://arxiv.org/pdf/2209.07807.pdf)

ICML 2023 - On Strengthening and Defending Graph Reconstruction Attack with Markov Chain Approximation.
[[paper]](https://openreview.net/pdf?id=Vcl3qckVyh)
[[code]](https://github.com/tmlr-group/MC-GRA)

## Natural language processing domain
| Year | Title | Adversarial Knowledge | Venue | Paper Link | Code Link |
| ---- | ----- | -------------------- | ----- | ---------- | --------- |
| 2020 | Extracting Training Data from Large Language Models |  black-box | USENIX Security | [Paper](https://arxiv.org/pdf/2012.07805.pdf) | [code](https://arxiv.org/pdf/2012.07805.pdf) |
| 2020 | Privacy Risks of General-Purpose Language Models | black & white-box | S&P | [Paper](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9152761) |  |
| 2018 | Privacy-preserving Neural Representations of Text | white-box | EMNLP | [Paper](https://arxiv.org/pdf/1808.09408.pdf) | [code](https://github.com/mcoavoux/pnet) |
| 2021 | TAG: Gradient Attack on Transformer-based Language Models | white-box | EMNLP | [Paper](https://arxiv.org/pdf/2103.06819.pdf) |  |
| 2020 | Information Leakage in Embedding Models | black & white-box | CCS | [Paper](https://arxiv.org/pdf/2004.00053.pdf) |  |
| 2022 | Text Revealer: Private Text Reconstruction via Model Inversion Attacks against Transformers| white-box| Arxiv | [Paper](https://arxiv.org/pdf/2209.10505.pdf) |  |

CCS 2020 - Information Leakage in Embedding Models.
[[paper]](https://dl.acm.org/doi/pdf/10.1145/3372297.3417270?casa_token=0ltuTKcG5cIAAAAA:YcpnOm4WlV0UnSS2dOWdtcnFh6DqSygG9MuS31gGQEgMxOBHQKeXsoNGkFhEw8gvlqY78gTkaRn9gUo)

USENIX Security 2021 - Extracting training data from large language models.
[[paper]](https://www.usenix.org/system/files/sec21-carlini-extracting.pdf)

Arxiv 2022 - Text Revealer: Private Text Reconstruction via Model Inversion Attacks against Transformers.
[[paper]](https://arxiv.org/pdf/2209.10505.pdf)


## Tools
[AIJack](https://github.com/Koukyosyumei/AIJack): Implementation of algorithms for AI security.

[Privacy-Attacks-in-Machine-Learning](https://github.com/shrebox/Privacy-Attacks-in-Machine-Learning): Membership Inference, Attribute Inference and Model Inversion attacks implemented using PyTorch.

[ml-attack-framework](https://github.com/Pilladian/ml-attack-framework): Universität des Saarlandes - Privacy Enhancing Technologies 2021 - Semester Project.


## Others
2019 - Uncovering a model’s secrets.
[[blog1]](https://gab41.lab41.org/uncovering-a-models-secrets-model-inversion-part-i-ce460eab93d6)
[[blog2]](https://gab41.lab41.org/robust-or-private-model-inversion-part-ii-94d54fd8d4a5)

2019 - Model Inversion Attacks Against Collaborative Inference.
[[slides]](https://www.acsac.org/2019/program/final/1/167.pdf)

2020 - Attacks against Machine Learning Privacy (Part 1): Model Inversion Attacks with the IBM-ART Framework.
[[blog]](https://franziska-boenisch.de/posts/2020/12/model-inversion/)

2021 - ML and DP.
[[slides]](https://www.cs.toronto.edu/~toni/Courses/Fairness/Lectures/ML-and-DP-v2.pdf)


## Related repositories
awesome-ml-privacy-attacks
[[repo]](https://github.com/stratosphereips/awesome-ml-privacy-attacks#reconstruction)

