---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html

---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I'm Hongzhe Bi, a second-year Matser student advised by [Professor Jun Zhu](https://ml.cs.tsinghua.edu.cn/~jun/index.shtml) in the TSAIL, Department of Computer Science and Technology, Tsinghua University, and co-advised by [Zhizhong Su](https://scholar.google.com/citations?user=HQfc8TEAAAAJ&hl=en) at Horizon Robotics.I graduated from Class of Artificial Intelligence, Beijing University of Posts and Telecommunications with a bachelor's degree. \
My Research Interests include **General Embodied Intelligence**, **Cross-Embodied Robot Foundation Model** and **Bimanual Dextrous Manipulation**.


# Publications 

## General Embodied Intelligence
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">arXiv 2026</div><img src='images/motus2.png' alt="Motus2 overview" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Motus2: A Self-Evolving General World Model for Dexterous Manipulation](https://arxiv.org/abs/2608.30237)

**Hongzhe Bi**, Zihao Zhou, Yihang Tang, Jingrui Pang, Shuhe Huang, Haitian Liu,
Runqing Wang, Shuai Huang, Yichen Wang, Yiming Cheng, Ruowen Zhao, Zhenghua Li,
Hengkai Tan, Xiaolong Liu, Jinhui Wan, Jiabao Liu, Min Zhao, Fan Bao, Jun Zhu

[**Project**](https://motus-robotics.github.io/motus2)
- Motus2 is a **self-evolving General World Model** for dexterous manipulation. A shared video-action backbone exposes a policy, an action-conditioned simulator, and a value evaluator. Candidate actions are simulated and scored for Best-of-N planning and **model-based policy optimization** with DiffusionNFT. Successful demonstrations supervise action learning, while failed and suboptimal interactions train dynamics and value estimation. A staged data curriculum progresses from monocular to stereo egocentric human data, followed by robot-domain adaptation. The framework also studies long-history context mechanisms and tactile action refinement, addressing partial observability and contact-sensitive control.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR2026</div><img src='images/motus.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Motus: A Unified Latent Action World Model](https://arxiv.org/abs/2512.13030)

**Hongzhe Bi**, Hengkai Tan, Shenghao Xie, Zeyuan Wang, Shuhe Huang, Haitian Liu,
Ruowen Zhao, Yao Feng, Chendong Xiang, Yinze Rong, Hongyan Zhao, Hanyu Liu,
Zhizhong Su, Lei Ma, Hang Su, Jun Zhu

[**Project**](https://motus-robotics.github.io/motus) <strong><span class='show_paper_citations' data=''></span></strong>
- Motus is a **unified latent action world model** that connects pretrained vision-language and video-generation models with an action expert through a Mixture-of-Transformers architecture. A UniDiffuser-style scheduler supports five modes: policy prediction, world modeling, inverse dynamics, video generation, and joint video-action prediction. **Optical-flow latent actions** capture transferable motion information, enabling action pretraining on human videos and heterogeneous robot trajectories through a three-stage training pipeline and six-level data pyramid. Motus achieves 87.02% average success across 50 RoboTwin 2.0 tasks under scene randomization, compared with 72.84% for X-VLA, with additional evaluations on two real-world bimanual robot platforms.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">AAAI2026</div><img src='images/hrdt_aaai2025.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[H-RDT: Human Manipulation Enhanced Bimanual Robotic Manipulation](https://arxiv.org/abs/2507.23523)

**Hongzhe Bi**, Lingxuan Wu, Tianwei Lin, Hengkai Tan, Zhizhong Su, Hang Su, Jun Zhu

[**Project**](https://embodiedfoundation.github.io/hrdt) <strong><span class='show_paper_citations' data=''></span></strong>
- H-RDT transfers manipulation knowledge from large-scale **egocentric human demonstrations** to bimanual robots. It pretrains a 2B-parameter flow-matching transformer on EgoDex using 3D wrist poses and fingertip positions, then fine-tunes on robot demonstrations with **embodiment-specific state/action adapters** and action decoders while reusing pretrained perception and transformer weights. Evaluations on RoboTwin 2.0 and three real-world robot platforms show improved average performance over training without human pretraining, including few-shot manipulation with limited robot demonstrations. These results highlight human motion data as a scalable source of behavioral priors for cross-embodiment policy learning.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Arxiv</div><img src='images/holobrain0.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[HoloBrain-0 Technical Report](https://arxiv.org/abs/2602.12062)

Xuewu Lin, Tianwei Lin, Yun Du, Hongyu Xie, Yiwei Jin, Jiawei Li, Shijie Wu, Qingze Wang, Mengdi Li, Mengao Zhao, Ziang Li, Chaodong Huang, **Hongzhe Bi**, Lichao Huang, Zhizhong Su

[**Project**](https://horizonrobotics.github.io/robot_lab/holobrain/) <strong><span class='show_paper_citations' data=''></span></strong>
- HoloBrain-0 is a comprehensive VLA framework that bridges foundation models with reliable real-world deployment. By explicitly incorporating embodiment priors (kinematics & camera parameters), we achieve SOTA manipulation performance on both simulation and real-world benchmarks. We open-source the full ecosystem, including the RoboOrchard infrastructure, to democratize scalable robot learning.
</div>
</div>

## Other Directions
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">COLM 2024</div><img src='images/unimem_colm.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[UniMem: Towards a Unified View of Long-Context Large Language Models](https://arxiv.org/abs/2402.03009)

Junjie Fang, Likai Tang, **Hongzhe Bi**, Yujia Qin, Si Sun, Zhenyu Li, Haolun Li, Yongjian Li, Xin Cong, Yankai Lin, Yukun Yan, Xiaodong Shi, Sen Song, Zhiyuan Liu, Maosong Sun

[**Project**](https://github.com/thunlp/UniMem) <strong><span class='show_paper_citations' data='LOJF4AAAAJ:u-x6o8ySG0sC'></span></strong>
- UniMem unifies context caching, context compression, and sparse attention through **four dimensions of memory augmentation**: management, writing, reading, and injection. It reformulates 16 long-context methods within a common framework, enabling systematic comparison and analysis of their design choices. Building on this framework, **UniMix** combines similarity-based retrieval, position-based attention, and compressed memory tokens. Experiments with TinyLLaMA and LLaMA2-7B show that UniMix matches or improves on the evaluated baselines in text and code perplexity, while achieving the highest average LongBench score in the TinyLLaMA comparison. Ablations reveal that where memory is injected can matter more than how many layers are augmented.
</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">WWW 2023</div><img src='images/eeft_www.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Beyond Fine-Tuning: Eficient and Efective Fed-Tuning for Mobile/Web Users](https://yaoguopku.github.io/papers/Liu-WWW-23.pdf)

Bingyan Liu, Yifeng Cai, **Hongzhe Bi**, Ziqi Zhang, Ding Li, Yao Guo, Xiangqun Chen

[**Project**](https://dl.acm.org/doi/abs/10.1145/3543507.3583212) <strong><span class='show_paper_citations' data='LOJF4AAAAJ:u5HHmVD_uO8C'></span></strong>
- This paper extend the local-user fine-tuning to multi-user fed-tuning with the help of Federated Learning (FL).
</div>
</div>

# Honors and Awards
- *2025.06* First place in Real-world Track and Second place in Simulation Track of [RoboTwin Dual-Arm Collaboration Challenge](https://robotwin-benchmark.github.io/cvpr-2025-challenge/#challenge-details)@CVPR2025

# Teaching
- 2026 Spring, TA in **Statistical Learning Theory and Applications**, instructed by [Prof. Jun Zhu](https://ml.cs.tsinghua.edu.cn/~jun/index.shtml)

# Educations
- *2024.09 - now*, Master, TSAIL, Department of Computer Science and Technology, Tsinghua University
- *2020.09 - 2024.06*, Undergraduate, School of Artificial Intelligence, Beijing University of Posts and Telecommunications(BUPT)
- *2014.09 - 2020.06*, High School, Beijing 101 Middle School

# Internships
- *2024.10 - 2026.03*, Horizon Robotics Lab
- *2024.04 - 2024.08*, D-Robotics
- *2023.10 - 2024.01*, ModelBest
