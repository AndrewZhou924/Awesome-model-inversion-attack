<h1 align="center"><b>Awesome Model Inversion Attacks</b></h1>
<p align="center">
    <a href="https://github.com/AndrewZhou924/Awesome-model-inversion-attack/pulls"><img src="https://img.shields.io/badge/PRs-Welcome-green" alt="PRs"></a>
    <a href="https://awesome.re"><img src="https://awesome.re/badge.svg" alt="awesome"></a>
    <a href="https://arxiv.org/abs/2411.10023"><img src="https://img.shields.io/badge/arXiv-2411.10023-b31b1b" alt="arXiv"></a>
    <img src="https://img.shields.io/github/stars/AndrewZhou924/Awesome-model-inversion-attack?color=yellow&label=Star" alt="Stars" >
</p>
A curated, cross-domain collection of research on **model inversion attacks (MIAs)**, defenses, evaluation, and closely related data-reconstruction problems.

Please star or watch this repository to keep tracking the latest updates! Contributions are welcome!

<a id="our-survey-model-inversion-attacks-a-survey-of-approaches-and-countermeasures"></a>

> [!IMPORTANT]
> ### Our survey: Model Inversion Attacks: A Survey of Approaches and Countermeasures
>
> **Zhanke Zhou, Jianing Zhu, Fengfei Yu, Xuan Li, Xiong Peng, Tongliang Liu, and Bo Han**
>
> Our survey provides a unified view of model inversion across **image, text, and graph data**, covering attack principles, threat models, defenses, datasets, evaluation metrics, practical deployment, and emerging foundation-model settings.
>
> **[Read the paper](https://arxiv.org/abs/2411.10023)** · **[Download PDF](https://arxiv.org/pdf/2411.10023)** · **[Jump to BibTeX](#citation)**

> [!NOTE]
> We distinguish post-training model inversion from gradient inversion, training-data extraction, and other adjacent reconstruction problems. See [Scope and labels](#scope-and-labels).

## News

- **[Aug/2026]** We refreshed the repository with recent work on foundation models and VLMs, diffusion priors, collaborative/split inference, defenses, and evaluation. See [Recent papers (2024–2026)](#recent-papers-20242026).
- **[Nov/2024]** We released our survey, *Model Inversion Attacks: A Survey of Approaches and Countermeasures*. [[arXiv]](https://arxiv.org/abs/2411.10023)

## Citation

If you find this repository helpful, please cite our [survey](https://arxiv.org/abs/2411.10023):

```
@article{zhou2024model,
  title={Model Inversion Attacks: A Survey of Approaches and Countermeasures},
  author={Zhou, Zhanke and Zhu, Jianing and Yu, Fengfei and Li, Xuan and Peng, Xiong and Liu, Tongliang and Han, Bo},
  journal={arXiv preprint arXiv:2411.10023},
  year={2024}
}
```

## Navigation

- [Scope and labels](#scope-and-labels)
- [Our survey](#our-survey-model-inversion-attacks-a-survey-of-approaches-and-countermeasures)
- [Recent papers (2024–2026)](#recent-papers-20242026)
- [Surveys and benchmarks](#surveys-and-benchmarks)
- [Computer vision domain](#computer-vision-domain)
- [Graph learning domain](#graph-learning-domain)
- [Natural language processing domain](#natural-language-processing-domain)
- [Tools](#tools)
- [Contributing](#contributing)
- [Others](#others)
- [Related repositories](#related-repositories)
- [Star History](#star-history)

## Scope and labels

A model inversion attack uses information exposed by a trained model—such as labels, confidence scores, embeddings, hidden representations, model parameters, or generated responses—to reconstruct private training information or sensitive characteristics represented by the model.

Each new entry should make the threat model explicit:

- **Access:** white-box, score-based black-box, label-only, embedding/feature interface, or generated-response interface.
- **Prior/resource:** auxiliary data, surrogate model, GAN/StyleGAN prior, diffusion prior, or no auxiliary data.
- **Target:** class representative, identity, individual input, prompt/text, graph topology, or sensitive attribute.
- **Status:** `peer-reviewed`, `accepted`, `preprint`, or `withdrawn submission`.

We list gradient inversion, federated-learning reconstruction, training-data extraction, and inversion for interpretability as **adjacent reconstruction** when they do not match the post-training MIA threat model.

## Surveys and benchmarks

- ⭐ **[Our survey, arXiv 2024] [Model Inversion Attacks: A Survey of Approaches and Countermeasures](https://arxiv.org/abs/2411.10023).** A unified cross-domain survey of attacks, defenses, evaluation, deployment considerations, and open problems across image, text, and graph data.
- [2025, Artificial Intelligence Review] **Deep Learning Model Inversion Attacks and Defenses: A Comprehensive Survey.** [[paper]](https://doi.org/10.1007/s10462-025-11248-0)
- [2024, arXiv] **Privacy Leakage on DNNs: A Survey of Model Inversion Attacks and Defenses.** [[paper]](https://arxiv.org/abs/2402.04013) [[toolbox]](https://github.com/ffhibnese/Model-Inversion-Attack-ToolBox)
- [2024, arXiv preprint] **MIBench: A Comprehensive Benchmark for Model Inversion Attack and Defense.** [[paper]](https://arxiv.org/abs/2410.05159)
- [2023, IEEE CSF] **SoK: Model Inversion Attack Landscape: Taxonomy, Challenges, and Future Roadmap.** [[paper]](https://doi.org/10.1109/CSF57540.2023.00017)
- [2021, IEEE TKDE] **Model Inversion Attacks: A Survey.** [[paper]](https://doi.org/10.1109/TKDE.2021.3065936)

Broader privacy, trustworthy-ML, and gradient-inversion surveys are retained in the domain lists below when useful, but are not presented as MIA-specific surveys.

## Recent papers (2024–2026)

This status-checked index highlights recent work that cuts across the historical image/text/graph organization below. Publication status was checked on **8 August 2026**.

Status labels: **peer-reviewed**, **accepted**, **preprint**, and **withdrawn submission**.

<details>
<summary><b>Show the 2024–2026 paper index</b></summary>

### Surveys, benchmarks, and evaluation

| Paper | Year / venue / status | Focus | Main contribution |
|---|---|---|---|
| ⭐ [Model Inversion Attacks: A Survey of Approaches and Countermeasures](https://arxiv.org/abs/2411.10023) | 2024, arXiv, **our survey** | Cross-domain survey | Unifies image, text, and graph MIAs with attacks, defenses, evaluation, deployment considerations, and an evolving repository. |
| [Privacy Leakage on DNNs: A Survey of Model Inversion Attacks and Defenses](https://arxiv.org/abs/2402.04013) | 2024, arXiv, **preprint** | Survey/toolbox | Cross-domain survey with an open-source MIA toolbox. |
| [Deep Learning Model Inversion Attacks and Defenses: A Comprehensive Survey](https://doi.org/10.1007/s10462-025-11248-0) | 2025, Artificial Intelligence Review 58:242, **peer-reviewed** | Survey | Reviews attacks, defenses, applications, datasets, metrics, and open problems. |
| [MIBench: A Comprehensive Benchmark for Model Inversion Attack and Defense](https://arxiv.org/abs/2410.05159) | 2024, arXiv, **preprint** | Benchmark/toolbox | Implements 16 attacks/defenses and nine evaluation protocols; the ICLR submission was withdrawn. |
| [Revisiting Model Inversion Evaluation: From Misleading Standards to Reliable Privacy Assessment](https://openaccess.thecvf.com/content/CVPR2026F/html/Ho_Revisiting_Model_Inversion_Evaluation_From_Misleading_Standards_to_Reliable_Privacy_CVPRF_2026_paper.html) | 2026, CVPR Findings, **peer-reviewed** | Evaluation | Identifies false positives caused by evaluation classifiers and proposes MLLM-based assessment. |
| [An Automated, Scalable Machine Learning Model Inversion Assessment Pipeline](https://arxiv.org/abs/2509.04214) | 2025, arXiv, **preprint** | Practical assessment | Automates visual leakage assessment with four risk dimensions. |

### Image, 3D, and diffusion-prior attacks

| Paper | Year / venue / status | Access / prior | Main contribution |
|---|---|---|---|
| [A Closer Look at GAN Priors: Exploiting Intermediate Features for Enhanced Model Inversion Attacks](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/4642_ECCV_2024_paper.php) | 2024, ECCV, **peer-reviewed** | White-box; GAN intermediate features | IF-GMI searches intermediate generator features under an L1-ball constraint. |
| [Prediction Exposes Your Face: Black-box Model Inversion via Prediction Alignment](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/5316_ECCV_2024_paper.php) | 2024, ECCV, **peer-reviewed** | Black-box prediction vectors; StyleGAN | P2I directly aligns prediction vectors with StyleGAN W+ to reduce queries. |
| [Pseudo-Private Data Guided Model Inversion Attacks](https://openreview.net/forum?id=pyqPUf36D2) | 2024, NeurIPS, **peer-reviewed** | White-box; public and pseudo-private images | Iteratively improves a generative prior with earlier reconstructions. |
| [Model Inversion Attacks Through Target-Specific Conditional Diffusion Models](https://arxiv.org/abs/2407.11424) | 2024, arXiv, **preprint** | Target-specific conditional diffusion | Diff-MI learns a diffusion prior guided by target predictions. |
| [Single-Step Diffusion Model-Based Generative Model Inversion Attacks](https://openreview.net/forum?id=TvhEoz1nim) | 2025, ICLR submission, **withdrawn submission** | Distilled diffusion prior; classifier/CLIP | Replaces GAN priors with a single-step diffusion generator and studies CLIP leakage. |
| [From Head to Tail: Efficient Black-box Model Inversion Attack via Long-tailed Learning](https://openaccess.thecvf.com/content/CVPR2025/html/Li_From_Head_to_Tail_Efficient_Black-box_Model_Inversion_Attack_via_CVPR_2025_paper.html) | 2025, CVPR, **peer-reviewed** | Confidence scores; surrogate and generator | SMILE combines long-tailed surrogate training with query-efficient derivative-free search. |
| [MEDUSA: Medical Data Under Shadow Attacks via Hybrid Model Inversion](https://proceedings.mlr.press/v258/azhar25a.html) | 2025, AISTATS, **peer-reviewed** | Gray-box; shadow model | Hybrid optimization and learned reconstruction for medical images. |
| [ConcreTizer: Model Inversion Attack via Occupancy Classification and Dispersion Control for 3D Point Cloud Restoration](https://openreview.net/forum?id=I4iZmsV4HM) | 2025, ICLR, **peer-reviewed** | 3D feature interface | Reconstructs voxelized point clouds using occupancy and dispersion objectives. |
| [Diffusion-Driven Universal Model Inversion Attack for Face Recognition](https://arxiv.org/abs/2504.18015) | 2025, arXiv, **preprint** | Face embeddings; fixed diffusion prior | Uses a reusable unconditional diffusion model without target-specific generator training. |
| [Model Inversion Attack Against Deep Hashing](https://arxiv.org/abs/2511.12233) | 2025, arXiv, **preprint** | Black-box deep hashing; diffusion | Reconstructs retrieval images without private training hash codes. |

### Foundation models and vision-language models

| Paper | Year / venue / status | Exposed interface | Main contribution |
|---|---|---|---|
| [Do Vision-Language Models Leak What They Learn? Adaptive Token-Weighted Model Inversion Attacks](https://openaccess.thecvf.com/content/CVPR2026/html/Nguyen_Do_Vision-Language_Models_Leak_What_They_Learn_Adaptive_Token-Weighted_Model_CVPR_2026_paper.html) | 2026, CVPR, **peer-reviewed** | VLM tokens and generated responses | Introduces token/sequence MIAs and SMI-AW for private visual training data. |
| [Data-Free Model-Related Attacks: Unleashing the Potential of Generative AI](https://www.usenix.org/conference/usenixsecurity25/presentation/ye-attacks) | 2025, USENIX Security, **peer-reviewed** | Black-box target; generative-AI prior | Studies data-free model extraction, membership inference, and model inversion. |
| [DRAG: Data Reconstruction Attack using Guided Diffusion](https://openreview.net/forum?id=z6GEZ2ogct) | 2025, ICML, **peer-reviewed** | CLIP/DINOv2 intermediate features | Uses guided latent diffusion to reconstruct inputs from deep foundation-model features. |

The single-step diffusion work listed in the preceding section also evaluates privacy leakage in CLIP.

### Collaborative and split inference

| Paper | Year / venue / status | Setting | Main contribution |
|---|---|---|---|
| [PATROL: Privacy-Oriented Pruning for Collaborative Inference Against Model Inversion Attacks](https://openaccess.thecvf.com/content/WACV2024/papers/Ding_PATROL_Privacy-Oriented_Pruning_for_Collaborative_Inference_Against_Model_Inversion_Attacks_WACV_2024_paper.pdf) | 2024, WACV, **peer-reviewed** | Collaborative inference defense | Privacy-aware pruning for resource-constrained edge deployment. |
| [A Stealthy Wrongdoer: Feature-Oriented Reconstruction Attack against Split Learning](https://arxiv.org/abs/2405.04115) | 2024, arXiv, **preprint** | Passive split-learning server | FORA transfers representation preferences from public auxiliary data. |
| [Theoretical Insights in Model Inversion Robustness and Conditional Entropy Maximization for Collaborative Inference Systems](https://openaccess.thecvf.com/content/CVPR2025/html/Xia_Theoretical_Insights_in_Model_Inversion_Robustness_and_Conditional_Entropy_Maximization_CVPR_2025_paper.html) | 2025, CVPR, **peer-reviewed** | Split-inference defense | Relates conditional entropy to reconstruction error and proposes CEM. |
| [Revisiting the Privacy Risks of Split Inference: A GAN-Based Data Reconstruction Attack via Progressive Feature Optimization](https://arxiv.org/abs/2508.20613) | 2025, arXiv, **preprint** | Split inference; StyleGAN | Progressive feature optimization improves deep-cut and OOD reconstruction. |
| [Ensembler: Protect Collaborative Inference Privacy from Model Inversion Attack via Selective Ensemble](https://doi.org/10.1109/DAC63849.2025.11132673) | 2025, DAC, **peer-reviewed** | Collaborative-inference defense | Selective ensembles confuse server-side reconstruction with low inference overhead. |
| [What Your Features Reveal: Data-Efficient Black-Box Feature Inversion Attack for Split DNNs](https://openaccess.thecvf.com/content/CVPR2026/papers/Ren_What_Your_Features_Reveal_Data-Efficient_Black-Box_Feature_Inversion_Attack_for_CVPR_2026_paper.pdf) | 2026, CVPR, **peer-reviewed** | Black-box feature interface | FIA-Flow learns from few image-feature pairs and performs one-step reconstruction. |
| [Prompt Inversion Attack against Collaborative Inference of Large Language Models](https://arxiv.org/abs/2503.09022) | 2025, arXiv, **preprint** | LLM inter-layer activations | Reconstructs prompts transmitted in collaborative LLM inference. |

### Defenses

| Paper | Year / venue / status | Defense axis | Main contribution |
|---|---|---|---|
| [On the Vulnerability of Skip Connections to Model Inversion Attacks](https://www.ecva.net/papers/eccv_2024/papers_ECCV/papers/10529.pdf) | 2024, ECCV, **peer-reviewed** | Architecture | Shows skip connections amplify leakage and proposes MI-resilient designs. |
| [Improving Robustness to Model Inversion Attacks via Sparse Coding Architectures](https://www.ecva.net/papers/eccv_2024/papers_ECCV/html/10339_ECCV_2024_paper.php) | 2024, ECCV, **peer-reviewed** | Architecture | Uses sparse-coding layers to limit irrelevant private information. |
| [Trap-MID: Trapdoor-based Defense against Model Inversion Attacks](https://openreview.net/forum?id=GNhrGRCerd) | 2024, NeurIPS, **peer-reviewed** | Misdirection/trapdoor | Makes inversion recover a trapdoor trigger instead of private samples. |
| [Defending against Model Inversion Attacks via Random Erasing](https://arxiv.org/abs/2409.01062) | 2024, arXiv, **preprint** | Data-centric training | Random erasing reduces recoverable visual detail while retaining task utility. |
| [Stealthy Shield Defense: A Conditional Mutual Information-Based Approach against Black-Box Model Inversion Attacks](https://openreview.net/forum?id=p0DjhjPXl3) | 2025, ICLR, **peer-reviewed** | Output post-processing | Reduces conditional mutual information without retraining the target model. |
| [Rank Matters: Understanding and Defending Model Inversion Attacks via Low-Rank Feature Filtering](https://doi.org/10.1145/3770854.3780328) | 2026, KDD, **peer-reviewed** | Low-rank feature filtering | Final version of the work previously titled CALoR; combines confidence adaptation and low-rank filtering. |
| [Model Inversion Attacks Meet Cryptographic Fuzzy Extractors](https://arxiv.org/abs/2510.25687) | 2025, arXiv, **preprint** | Cryptographic biometric defense | Studies inversion against fuzzy extractors and proposes L2FE-Hash. |

### Text and embedding inversion

| Paper | Year / venue / status | Interface | Main contribution |
|---|---|---|---|
| [An Inversion Attack Against Obfuscated Embedding Matrix in Language Model Inference](https://aclanthology.org/2024.emnlp-main.126/) | 2024, EMNLP, **peer-reviewed** | Obfuscated embedding matrix | Recovers text from glide-reflection-obfuscated embeddings. |
| [ALGEN: Few-shot Inversion Attacks on Textual Embeddings via Cross-Model Alignment and Generation](https://aclanthology.org/2025.acl-long.1185/) | 2025, ACL, **peer-reviewed** | Few-shot black-box embeddings | Cross-model alignment enables inversion with few paired samples. |
| [ObfusLM: Privacy-preserving Language Model Service against Embedding Inversion Attacks](https://aclanthology.org/2025.acl-long.58/) | 2025, ACL, **peer-reviewed** | Embedding-service defense | Obfuscates embeddings for both classification and generation services. |
| [PrivacyRestore: Privacy-Preserving Inference in Large Language Models via Privacy Removal and Restoration](https://aclanthology.org/2025.acl-long.532/) | 2025, ACL, **peer-reviewed** | LLM inference defense | Removes private spans client-side and restores task information through privacy-aware vectors. |
| [Towards Privacy-Preserving Large Language Model: Text-free Inference Through Alignment and Adaptation](https://aclanthology.org/2026.acl-long.1191/) | 2026, ACL, **peer-reviewed** | Noisy pooled embeddings | PPFT protects inference and private-domain fine-tuning without sending raw text. |

### Graph reconstruction

| Paper | Year / venue / status | Interface | Main contribution |
|---|---|---|---|
| [ReconXF: Graph Reconstruction Attack via Public Feature Explanations on Privatized Node Features and Labels](https://arxiv.org/abs/2506.02134) | 2025, arXiv, **preprint** | Feature explanations and privatized attributes | Denoises auxiliary node information and reconstructs graph topology. |
| [GraphToxin: Reconstructing Full Unlearned Graphs from Graph Unlearning](https://arxiv.org/abs/2511.10936) | 2025, arXiv, **preprint** | Graph-unlearning residue | Reconstructs deleted nodes, edges, and neighborhoods; adjacent to classical MIA. |

### Adjacent reconstruction problems

These papers are useful context but should not be presented as classical post-training MIAs without qualification.

| Paper | Year / venue / status | Why adjacent |
|---|---|---|
| [GRAIN: Exact Graph Reconstruction from Gradients](https://proceedings.iclr.cc/paper_files/paper/2025/hash/b88ccd2117cf61258e868a84145c94ca-Abstract-Conference.html) | 2025, ICLR, **peer-reviewed** | Reconstructs graph structure and features from shared training gradients. |
| [TINA: Text-Free Inversion Attack for Unlearned Text-to-Image Diffusion Models](https://openaccess.thecvf.com/content/CVPR2026/html/Xiang_TINA_Text-Free_Inversion_Attack_for_Unlearned_Text-to-Image_Diffusion_Models_CVPR_2026_paper.html) | 2026, CVPR, **peer-reviewed** | Attacks concept erasure rather than private classifier training data. |
| [MIMIC: Multimodal Inversion for Model Interpretation and Conceptualization](https://arxiv.org/abs/2508.07833) | 2025, arXiv, **preprint** | Representation inversion for interpretation rather than a privacy attack. |
| [Implicit Inversion Turns CLIP into a Decoder](https://openreview.net/forum?id=hvukI2ws5O) | 2025, OpenReview | Representation decoding/generation rather than private-data reconstruction. |

### Maintenance notes

- Merge preprint and final versions into one lineage. In particular, arXiv:2410.05814 (CALoR) became the KDD 2026 paper *Rank Matters*.
- Do not label MIBench as an ICLR publication; it remains an arXiv preprint and its ICLR submission was withdrawn.
- Do not label *Single-Step Diffusion Model-Based Generative Model Inversion Attacks* as an accepted ICLR 2025 paper.
- Distinguish diffusion models used as attack priors from diffusion models that are themselves the attack target.

</details>

## Computer vision domain

<details>
<summary><b>Show the complete computer-vision list</b></summary>

The entries below preserve the historical collection. For a status-checked cross-cutting view of recent work, use the [2024–2026 index](#recent-papers-20242026).

- [NDSS 2025] CENSOR: Defense Against Gradient Inversion via Orthogonal Subspace Bayesian Sampling [[paper]](https://arxiv.org/pdf/2501.15718) [[code]](https://github.com/KaiyuanZh/censor) [[project]](https://censor-gradient.github.io/)

- [ICML 2024] (white-box) Sparse Model Inversion: Efficient Inversion of Vision Transformers for Data-Free Applications [[paper]](https://openreview.net/pdf?id=T0lFfO8HaK) [[code]](https://github.com/Egg-Hu/SMI)

- [CVPR 2024] Model Inversion Robustness: Can Transfer Learning Help? [[paper]](https://openaccess.thecvf.com/content/CVPR2024/papers/Ho_Model_Inversion_Robustness_Can_Transfer_Learning_Help_CVPR_2024_paper.pdf) [[code]](https://hosytuyen.github.io/projects/TL-DMI)
  
- [ICLR 2024] Be Careful What You Smooth For: Label Smoothing Can Be a Privacy Shield but Also a Catalyst for Model Inversion Attacks [[paper]](https://arxiv.org/pdf/2310.06549) [[code]](https://github.com/LukasStruppek/Plug-and-Play-Attacks)

- [ICASSP 2023] (black-box) Sparse Black-Box Inversion Attack with Limited Information [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10095514) [[code]](https://github.com/Tencent/TFace/tree/master/recognition)

- [IEEE Transactions on Information Forensics and Security 2023] A GAN-Based Defense Framework Against Model Inversion Attacks [[paper]](https://ieeexplore.ieee.org/document/10184476)

- [CVPR 2023] (black-box) Breaching FedMD: Image Recovery via Paired-Logits Inversion Attack [[paper]](https://arxiv.org/pdf/2304.11436.pdf) [[code]](https://github.com/FLAIR-THU/PairedLogitsInversion)

- [AAAI 2023] (white-box) Pseudo Label-Guided Model Inversion Attack via Conditional Generative Adversarial Network [[paper]](https://arxiv.org/pdf/2302.09814.pdf) [[code]](https://github.com/lethesec/plg-mi-attack)

- [TDSC 2023] (black-box) C2FMI: Coarse-to-Fine Black-box Model Inversion Attack [[paper]](https://ieeexplore.ieee.org/document/10148574) [[code]](https://github.com/MiLabHITSZ/2022YeC2FMI)

- [TDSC 2023] (black-box) Boosting Model Inversion Attacks with Adversarial Examples [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10148576)

- [CVPR 2023] (black-box) Reinforcement Learning-Based Black-Box Model Inversion Attacks [[paper]](https://arxiv.org/pdf/2304.04625.pdf) [[code]](https://github.com/HanGyojin/RLB-MI)

- [CVPR 2023] (white-box) Re-thinking Model Inversion Attacks Against Deep Neural Networks [[paper]](https://arxiv.org/pdf/2304.01669.pdf) [[code]](https://github.com/sutd-visual-computing-group/Re-thinking_MI)

- [AAAI 2023] (black-box (defense)) Purifier: Defending Data Inference Attacks via Transforming Confidence Scores [[paper]](https://arxiv.org/pdf/2005.03915.pdf)

- [IEEE TIFS 2024] (label-only black-box) Unstoppable Attack: Label-Only Model Inversion via Conditional Diffusion Model [[paper]](https://arxiv.org/abs/2307.08424)

- [ICML 2022] Plug-In Inversion: Model-Agnostic Inversion for Vision with Data Augmentations [[paper]](https://proceedings.mlr.press/v162/ghiasi22a/ghiasi22a.pdf)

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

- [NDSS 2022] (white-box & black-box) MIRROR: Model Inversion for Deep Learning Network with High Fidelity [[paper]](https://www.cs.purdue.edu/homes/an93/static/papers/ndss2022_model_inversion.pdf) [[code]](https://github.com/njuaplusplus/mirror)

- [SP 2022] (white-box) Reconstructing Training Data with Informed Adversaries [[paper]](https://arxiv.org/abs/2201.04845)

- [BMVC 2022] (white-box) Privacy Vulnerability of Split Computing to Data-Free Model Inversion Attacks [[paper]](https://arxiv.org/abs/2107.06304)

- [NeurIPS 2022] (white-box) Reconstructing Training Data from Trained Neural Networks [[paper]](https://arxiv.org/abs/2206.07758)

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

- [CCS 2021] Unleashing the tiger: Inference attacks on split learning [[paper]](https://arxiv.org/pdf/2012.02670) [[code]](https://github.com/pasquini-dario/SplitNN_FSHA)

- [CSR 2021] Defending Against Model Inversion Attack by Adversarial Examples [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9527945)
  
- [CVPR 2020] Dreaming to Distill: Data-free Knowledge Transfer via DeepInversion [[paper]](https://arxiv.org/pdf/1912.08795) [[code]](https://github.com/NVlabs/DeepInversion)

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

- [CVPR 2020] The Secret Revealer: Generative Model-Inversion Attacks Against Deep Neural Networks [[paper]](https://openaccess.thecvf.com/content_CVPR_2020/papers/Zhang_The_Secret_Revealer_Generative_Model-Inversion_Attacks_Against_Deep_Neural_Networks_CVPR_2020_paper.pdf)

- [AAAI 2020] (black & white-box) Improving Robustness to Model Inversion Attacks via Mutual Information Regularization [[paper]](https://arxiv.org/pdf/2009.05241v1.pdf)

- [arXiv 2020] Defending Model Inversion and Membership Inference Attacks via Prediction Purification [[paper]](https://arxiv.org/pdf/2005.03915)

- [arXiv 2019] (black-box) GAMIN: An Adversarial Approach to Black-Box Model Inversion [[paper]](https://arxiv.org/pdf/1909.11835.pdf)

- [ACSAC 2019] Model Inversion Attacks Against Collaborative Inference [[paper]](https://www.acsac.org/2019/program/final/1/167.pdf) [[code]](https://github.com/zechenghe/Inverse_Collaborative_Inference)

- [CCS 2019] (black-box) Neural Network Inversion in Adversarial Setting via Background Knowledge Alignment [[paper]](https://dl.acm.org/doi/pdf/10.1145/3319535.3354261?casa_token=J81Ps-ZWXHkAAAAA:FYnXo7DQoHpdhqns8x2TclKFeHpAQlXVxMBW2hTrhJ5c20XKdsounqdT1Viw1g6Xsu9FtKj85elxQaA) [[code]](https://github.com/zhangzp9970/TB-MIA)

- [ACSAC 2019] (black & white-box) Model Inversion Attacks Against Collaborative Inference [[paper]](http://palms.ee.princeton.edu/system/files/Model+Inversion+Attack+against+Collaborative+Inference.pdf)

- [GLSVLSI 2019] (black-box (defense)) MLPrivacyGuard: Defeating Confidence Information based Model Inversion Attacks on Machine Learning Systems [[paper]](https://www.researchgate.net/profile/Tiago-Alves-13/publication/333136362_MLPrivacyGuard_Defeating_Confidence_Information_based_Model_Inversion_Attacks_on_Machine_Learning_Systems/links/5cddb94d92851c4eaba682d7/MLPrivacyGuard-Defeating-Confidence-Information-based-Model-Inversion-Attacks-on-Machine-Learning-Systems.pdf)

- [CVPR 2019] A Style-Based Generator Architecture for Generative Adversarial Networks [[paper]](https://arxiv.org/abs/1812.04948)

- [arXiv 2019] (white-box) An Attack-Based Evaluation Method for Differentially Private Learning Against Model Inversion Attack [[paper]](https://ieeexplore.ieee.org/document/8822435)

- [CSF 2018] (white-box) Privacy Risk in Machine Learning: Analyzing the Connection to Overfitting [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8429311)

- [CCS 2017] (white-box) Machine Learning Models that Remember Too Much [[paper]](https://arxiv.org/pdf/1709.07886.pdf) [[code]](https://github.com/csong27/ml-model-remember)

- [PST 2017] (white-box) Model Inversion Attacks for Prediction Systems: Without knowledge of Non-Sensitive Attributes [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=8476925)

- [NeurIPS 2016] Generating Images with Perceptual Similarity Metrics based on Deep Networks [[paper]](https://proceedings.neurips.cc/paper/2016/file/371bce7dc83817b7893bcdeed13799b5-Paper.pdf)

- [CVPR 2016] Inverting visual representations with convolutional networks [[paper]](https://arxiv.org/pdf/1506.02753)

- [CSF 2016] (black & white-box) A Methodology for Formalizing Model-Inversion Attacks [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=7536387&casa_token=ClIVAMYo6dcAAAAA:u75HHyFHj5lBRec9h5SqOZyAsL2dICcWIuQPCj6ltk8McREFCaM4ex42mv3S-oNPiGJLDfUqg0qL)

- [CVPR 2015] Understanding Deep Image Representations by Inverting Them [[paper]](https://openaccess.thecvf.com/content_cvpr_2015/papers/Mahendran_Understanding_Deep_Image_2015_CVPR_paper.pdf)

- [IJCAI 2015] (white-box (defense)) Regression Model Fitting under Differential Privacy and Model Inversion Attack [[paper]](http://www.csce.uark.edu/~xintaowu/publ/ijcai15.pdf) [[code]](https://github.com/cxs040/Regression-Model-Fitting-under-Differential-Privacy-and-Model-Inversion-Attack-Source-Code)

- [CCS 2015] (black & white-box) Model Inversion Attacks that Exploit Confidence Information and Basic Countermeasures [[paper]](https://dl.acm.org/doi/pdf/10.1145/2810103.2813677) [[code1]](http://www.cs.cmu.edu/~mfredrik/mi-2016.zip) [[code2]](https://github.com/yashkant/Model-Inversion-Attack) [[code3]](https://github.com/zhangzp9970/MIA) [[code4]](https://github.com/sarahsimionescu/simple-model-inversion)

- [ICLR 2014] Intriguing properties of neural networks [[paper]](https://arxiv.org/pdf/1312.6199)

- [ICLR 2014] Deep Inside Convolutional Networks: Visualising Image Classification Models and Saliency Maps [[paper]](https://arxiv.org/pdf/1312.6034)

- [USENIX Security 2014] (black & white-box) Privacy in Pharmacogenetics: An End-to-End Case Study of Personalized Warfarin Dosing [[paper]](https://www.usenix.org/system/files/conference/usenixsecurity14/sec14-paper-fredrikson-privacy.pdf)
  
</details>
  
## Graph learning domain

<details>
<summary><b>Show the complete graph-learning list</b></summary>

The entries below include both post-training graph inversion and adjacent graph-reconstruction settings. See each paper's threat model before comparing results.

- [SecureComm 2023] (white-box) Model Inversion Attacks on Homogeneous and Heterogeneous Graph Neural Networks [[paper]](https://arxiv.org/pdf/2310.09800)

- [ICML 2023] (white-box) On Strengthening and Defending Graph Reconstruction Attack with Markov Chain Approximation [[paper]](https://openreview.net/pdf?id=Vcl3qckVyh) [[code]](https://github.com/tmlr-group/MC-GRA)

- [TKDE 2022] Model Inversion Attacks against Graph Neural Networks [[paper]](https://arxiv.org/pdf/2209.07807.pdf)

- [IJIS 2022] Defense Against Membership Inference Attack in Graph Neural Networks Through Graph Perturbation [[paper]](https://link.springer.com/article/10.1007/s10207-022-00646-y)

- [CCS 2022] Finding MNEMON: Reviving Memories of Node Embeddings [[paper]](https://arxiv.org/pdf/2204.06963.pdf)

- [arXiv 2022] Privacy and Transparency in Graph Machine Learning: A Unified Perspective [[paper]](https://arxiv.org/pdf/2207.10896.pdf)

- [arXiv 2022] Private Graph Extraction via Feature Explanations [[paper]](https://arxiv.org/pdf/2206.14724.pdf)

- [arXiv 2022] Degree-Preserving Randomized Response for Graph Neural Networks under Local Differential Privacy [[paper]](https://arxiv.org/pdf/2202.10209.pdf)

- [arXiv 2022] Sok: Differential Privacy on Graph-Structured Data[[paper]](https://arxiv.org/pdf/2203.09205.pdf)

- [arXiv 2022] GAP: Differentially Private Graph Neural Networks with Aggregation Perturbation [[paper]](https://arxiv.org/pdf/2203.00949.pdf)

- [arXiv 2022] Differentially Private Graph Classification With GNNs [[paper]](https://arxiv.org/pdf/2202.02575.pdf)

- [IEEE S&P 2022] Model Stealing Attacks Against Inductive Graph Neural Networks [[paper]](https://arxiv.org/pdf/2112.08331.pdf) [[code]](https://github.com/xinleihe/GNNStealing)

- [USENIX Security 2022] Inference Attacks Against Graph Neural Networks [[paper]](https://www.usenix.org/system/files/sec22summer_zhang-zhikun.pdf) [[code]](https://github.com/Zhangzhk0819/GNN-Embedding-Leaks)

- [WWW 2022] Learning Privacy-Preserving Graph Convolutional Network with Partially Observed Sensitive Attributes [[paper]](https://dl.acm.org/doi/pdf/10.1145/3485447.3511975?casa_token=Xsle4t9cLdcAAAAA:Gmij-qWaTJ2esGVa-yzKNHqVOMzYyaIgdNcgGmEzHrVyMdwwf9idn3qBjkhCcQeRTvbAkaT6OxiwXsk)

- [arXiv 2022] (black & white-box) A Comprehensive Survey on Trustworthy Graph Neural Networks: Privacy, Robustness, Fairness, and Explainability [[paper]](https://arxiv.org/pdf/2204.08570.pdf)

- [arXiv 2021] Node-Level Membership Inference Attacks Against Graph Neural Networks [[paper]](https://arxiv.org/pdf/2102.05429.pdf)

- [IJCAI 2021] (white-box) GraphMI: Extracting Private Graph Data from Graph Neural Networks [[paper]](https://arxiv.org/pdf/2106.02820v1.pdf) [[code]](https://github.com/zaixizhang/GraphMI)

- [ICML 2021] DeepWalking Backwards: From Node Embeddings Back to Graphs [[paper]](http://proceedings.mlr.press/v139/chanpuriya21a/chanpuriya21a.pdf) [[code]](https://github.com/konsotirop/Invert_Embeddings)

- [ICDE 2021] (black-box) NetFense: Adversarial Defenses against Privacy Attacks on Neural Networks for Graph Data [[paper]](https://arxiv.org/pdf/2106.11865.pdf) [[code]](https://github.com/ICHproject/NetFense)

- [IJCAI 2021] (white-box) A Survey on Gradient Inversion: Attacks, Defenses and Future Directions [[paper]](https://arxiv.org/pdf/2206.07284.pdf)

- [MobiQuitous 2020] Quantifying Privacy Leakage in Graph Embedding [[paper]](https://arxiv.org/pdf/2010.00906.pdf) [[code]](https://github.com/vasishtduddu/GraphLeaks)

- [arXiv 2020] (black & white-box) Reducing Risk of Model Inversion Using Privacy-Guided Training [[paper]](https://arxiv.org/pdf/2006.15877.pdf)

- [USENIX Security 2020] Stealing Links from Graph Neural Networks [[paper]](https://www.usenix.org/system/files/sec21-he-xinlei.pdf) [[code]](https://github.com/xinleihe/link_stealing_attack)

</details>


## Natural language processing domain

<details>
<summary><b>Show the complete NLP list</b></summary>

This historical list includes embedding inversion, prompt inversion, memorization, and adjacent training-data extraction. The [2024–2026 index](#recent-papers-20242026) separates these interfaces and statuses.

- [NeurIPS 2025] (black-box) Better Language Model Inversion by Compactly Representing Next-Token Distributions [[paper]](https://arxiv.org/abs/2506.17090) [[code]](https://github.com/dill-lab/PILS)

- [ACL 2024] (black-box) Text Embedding Inversion Security for Multilingual Language Models [[paper]](https://arxiv.org/abs/2401.12192) [[code]](https://github.com/siebeniris/multivec2text)

- [ICLR 2024] (black-box) Language Model Inversion [[paper]](https://arxiv.org/abs/2311.13647) [[code]](https://github.com/jxmorris12/vec2text)

- [arXiv 2024] (white-box) Do Membership Inference Attacks Work on Large Language Models? [[paper]](https://arxiv.org/pdf/2402.07841.pdf)

- [EMNLP 2024] (black-box) Extracting Prompts by Inverting LLM Outputs [[paper]](https://arxiv.org/pdf/2405.15012) [[code]](https://github.com/collinzrj/output2prompt)

- [ACL 2024] (black-box) Transferable Embedding Inversion Attack: Uncovering Privacy Risks in Text Embeddings without Model Queries [[paper]](https://aclanthology.org/2024.acl-long.230/)

- [COLM 2024] Effective Prompt Extraction from Language Models [[paper]](https://openreview.net/forum?id=0o95CVdNuz#discussion)

- [EMNLP 2023] (black-box) Text Embeddings Reveal (Almost) As Much As Text [[paper]](https://arxiv.org/abs/2311.13647) [[code]](https://github.com/jxmorris12/vec2text)

- [arXiv 2023] (white-box) Deconstructing Classifiers: Towards A Data Reconstruction Attack Against Text Classification Models [[paper]](https://arxiv.org/pdf/2306.13789.pdf)

- [ACL 2023] (black-box) Sentence Embedding Leaks More Information than You Expect: Generative Embedding Inversion Attack to Recover the Whole Sentence [[paper]](https://arxiv.org/pdf/2305.03010.pdf) [[code]](https://github.com/hkust-knowcomp/geia)

- [SaTML 2023] (black-box) Model Inversion Attack with Least Information and an In-depth Analysis of its Disparate Vulnerability [[paper]](https://openreview.net/pdf?id=x42Lo6Mkcrf)

- [NAACL 2022] (white-box) Are Large Pre-Trained Language Models Leaking Your Personal Information? [[paper]](https://aclanthology.org/2022.findings-emnlp.148.pdf) [[code]](https://github.com/jeffhj/LM_PersonalInfoLeak)

- [NeurIPS 2022] (white-box) Recovering Private Text in Federated Learning of Language Models [[paper]](https://arxiv.org/pdf/2205.08514.pdf) [[code]](https://github.com/princeton-sysml/film)

- [ACL 2022] (white-box) Canary Extraction in Natural Language Understanding Models [[paper]](https://arxiv.org/pdf/2203.13920.pdf)

- [arXiv 2022] (white-box) Text Revealer: Private Text Reconstruction via Model Inversion Attacks against Transformers [[paper]](https://arxiv.org/pdf/2209.10505.pdf)

- [arXiv 2022] (black-box) KART: Parameterization of Privacy Leakage Scenarios from Pre-trained Language Models [[paper]](https://arxiv.org/pdf/2101.00036v1.pdf) [[code]](https://github.com/yutanakamura-tky/kart)

- [CEUR Workshop 2021] (black-box) Dataset Reconstruction Attack against Language Models [[paper]](https://ceur-ws.org/Vol-2942/paper1.pdf)

- [EMNLP 2021] (white-box) TAG: Gradient Attack on Transformer-based Language Models [[paper]](https://arxiv.org/pdf/2103.06819.pdf)

- [CCS 2020] (black & white-box) Information Leakage in Embedding Models [[paper]](https://arxiv.org/pdf/2004.00053.pdf)

- [S&P 2020] (black & white-box) Privacy Risks of General-Purpose Language Models [[paper]](https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=9152761)

- [USENIX Security 2020] (black-box) Extracting Training Data from Large Language Models [[paper]](https://arxiv.org/pdf/2012.07805.pdf) [[code]](https://arxiv.org/pdf/2012.07805.pdf)

- [USENIX Security 2019] The Secret Sharer: Evaluating and Testing Unintended Memorization in Neural Networks [[paper]](https://www.usenix.org/system/files/sec19-carlini.pdf)

- [arXiv 2018] Towards Robust and Privacy-preserving Text Representations [[paper]](https://arxiv.org/pdf/1805.06093)

- [arXiv 2018] Privacy-preserving Neural Representations of Text [[paper]](https://arxiv.org/pdf/1808.09408)

- [arXiv 2018] Adversarial Removal of Demographic Attributes from Text Data [[paper]](https://arxiv.org/pdf/1808.06640)

- [NeurIPS 2017] Controllable Invariance through Adversarial Feature Learning [[paper]](https://proceedings.neurips.cc/paper_files/paper/2017/file/8cb22bdd0b7ba1ab13d742e22eed8da2-Paper.pdf)

- [arXiv 2015] Censoring Representations with an Adversary [[paper]](https://arxiv.org/pdf/1511.05897)

</details>

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
- [arXiv 2025] The DCR Delusion: Measuring the Privacy Risk of Synthetic Data. [[paper]](https://arxiv.org/pdf/2505.01524)
- [arXiv 2023] A Linear Reconstruction Approach for Attribute Inference Attacks against Synthetic Data [[paper]](https://arxiv.org/pdf/2301.10053) [[code]](https://github.com/synthetic-society/recon-synth)
- [USENIX 2022] Synthetic Data - Anonymisation of Groundhog Day [[paper]](https://www.usenix.org/system/files/sec22summer_stadler.pdf) [[code]](https://github.com/spring-epfl/synthetic_data_release)

## Others

- [Blog 2020] Uncovering a model's secrets [[blog1]](https://gab41.lab41.org/uncovering-a-models-secrets-model-inversion-part-i-ce460eab93d6) [[blog2]](https://gab41.lab41.org/robust-or-private-model-inversion-part-ii-94d54fd8d4a5)
- [Blog 2020] Attacks against Machine Learning Privacy (Part 1): Model Inversion Attacks with the IBM-ART Framework [[blog]](https://franziska-boenisch.de/posts/2020/12/model-inversion/)
- [Slides 2020] ML and DP [[slides]](https://www.cs.toronto.edu/~toni/Courses/Fairness/Lectures/ML-and-DP-v2.pdf)

### Related representation-space attacks (not model inversion)

These papers affect interfaces also studied by model inversion research, but do not reconstruct private training information and are therefore listed separately.

- [arXiv 2025] (black- and white-box) **Jailbreaking LLMs' Safeguard with Universal Magic Words for Text Embedding Models.** Exploits embedding-distribution bias to find universal suffixes that manipulate cosine similarity and bypass embedding-based safeguards. [[paper]](https://arxiv.org/abs/2501.18280)

## Contributing

Contributions are welcome through pull requests or issues. Please use official publisher, proceedings, OpenReview, ACL Anthology, PMLR, CVF/ECVA, USENIX, DOI, or arXiv links whenever possible.

Suggested entry format:

```text
Year | Paper | Domain | Target/observable | Access | Auxiliary data/prior |
Attack or defense | Venue/status | Paper URL | Code URL (optional)
```

Before submitting an entry:

1. Search this README for duplicate titles and earlier versions.
2. Merge a preprint and its final version into one lineage.
3. Verify the authors, exact title, venue, year, pages, DOI, URL, and current publication status.
4. State the exposed interface and recovered target instead of using only “white-box” or “black-box”.
5. Label gradient inversion, training-data extraction, interpretability-oriented inversion, and unlearning/concept-erasure inversion as **adjacent reconstruction** unless the paper studies the classical MIA threat model.
6. Add at most one original sentence describing the contribution; do not copy the abstract.

## Related repositories

- awesome-ml-privacy-attacks [[repo]](https://github.com/stratosphereips/awesome-ml-privacy-attacks#reconstruction)

## Star History

[![Star History Chart](https://api.star-history.com/svg?repos=AndrewZhou924/Awesome-model-inversion-attack&type=Date)](https://star-history.com/#AndrewZhou924/Awesome-model-inversion-attack&Date)
