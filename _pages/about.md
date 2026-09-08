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
- Motus2 is the **first fully multimodal General World Model** for high-DoF dexterous manipulation, integrating vision, language, action, and touch. It is the first to realize **closed-loop self-evolution** with one shared model serving as a policy, simulator, and evaluator. Expert demonstrations supervise action learning, while failed and suboptimal interactions support dynamics and value learning. Data scaling spans approximately 130,000 raw hours of monocular and stereo egocentric recordings, followed by robot-domain adaptation at the hundred-hour scale. The model further explores **long-context modeling** and adds **tactile feedback** for contact-aware control. Together, egocentric data scaling and closed-loop general world model scaling provide a general path toward self-evolving dexterous manipulation.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR2026</div><img src='images/motus.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Motus: A Unified Latent Action World Model](https://arxiv.org/abs/2512.13030)

**Hongzhe Bi**, Hengkai Tan, Shenghao Xie, Zeyuan Wang, Shuhe Huang, Haitian Liu,
Ruowen Zhao, Yao Feng, Chendong Xiang, Yinze Rong, Hongyan Zhao, Hanyu Liu,
Zhizhong Su, Lei Ma, Hang Su, Jun Zhu

[**Project**](https://motus-robotics.github.io/motus) <strong><span class='show_paper_citations' data=''></span></strong>
- Motus is among the earliest world-action models to **unify understanding, imagination, and action** through joint video-action modeling. It integrates pretrained vision-language and video-generation models with an action expert, allowing one shared model to switch flexibly across **five prediction and control modes**. Motion-based latent actions enable **large-scale action pretraining** from human videos and heterogeneous robot experience. Simulation and real-world experiments demonstrate that unifying these capabilities and pretrained priors improves downstream robot manipulation over strong contemporary baselines.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">AAAI2026</div><img src='images/hrdt_aaai2025.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[H-RDT: Human Manipulation Enhanced Bimanual Robotic Manipulation](https://arxiv.org/abs/2507.23523)

**Hongzhe Bi**, Lingxuan Wu, Tianwei Lin, Hengkai Tan, Zhizhong Su, Hang Su, Jun Zhu

[**Project**](https://embodiedfoundation.github.io/hrdt) <strong><span class='show_paper_citations' data=''></span></strong>
- H-RDT is among the first studies to establish **large-scale egocentric human data** as a foundation for bimanual robot manipulation, addressing the scarcity of robot demonstrations. It pretrains on human videos with paired 3D hand poses, then transfers these manipulation priors to diverse robots through **cross-embodiment fine-tuning**. Simulation and real-world evaluations demonstrate improvements over contemporary baselines, including Pi0 and RDT, together with **few-shot learning** and robustness across tasks. The work has also informed the development of embodied manipulation foundation models at Horizon Robotics.
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
- UniMem unifies long-context language modeling from the perspective of **memory augmentation**, turning isolated methods into a common framework for systematic analysis and design. It reformulates **16 methods** across memory management, writing, reading, and injection, and analyzes representative approaches to reveal their design principles and complementary strengths. This analysis guides **UniMix**, which integrates those strengths to improve long-context processing and reduce perplexity relative to baselines. The work provides a systematic basis for understanding existing approaches and designing more effective memory mechanisms for long-context language models.
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
