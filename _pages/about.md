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

I'm Hongzhe Bi, a second-year Master student advised by [Professor Jun Zhu](https://ml.cs.tsinghua.edu.cn/~jun/index.shtml) in the [TSAIL](https://ml.cs.tsinghua.edu.cn/people.html), Department of Computer Science and Technology, Tsinghua University, and co-advised by [Zhizhong Su](https://scholar.google.com/citations?user=HQfc8TEAAAAJ&hl=en) at [Horizon Robotics](https://horizonrobotics.github.io/robot_lab/main/index.html).I graduated from Class of Artificial Intelligence, Beijing University of Posts and Telecommunications with a bachelor's degree. \
My Research Interests include **General Embodied Intelligence**, **Cross-Embodied Robot Foundation Model** and **Bimanual Dextrous Manipulation**.


# Publications 

## General Embodied Intelligence
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">CVPR2026</div><img src='images/motus.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Motus: A Unified Latent Action World Model](https://arxiv.org/abs/2512.13030)

**Hongzhe Bi**, Hengkai Tan, Shenghao Xie, Zeyuan Wang, Shuhe Huang, Haitian Liu,
Ruowen Zhao, Yao Feng, Chendong Xiang, Yinze Rong, Hongyan Zhao, Hanyu Liu,
Zhizhong Su, Lei Ma, Hang Su, Jun Zhu

[**Project**](https://motus-robotics.github.io/motus) <strong><span class='show_paper_citations' data=''></span></strong>
- Motus is a **unified latent action world model** that leverages existing pretrained models and rich, sharable motion information. Motus introduces a **Mixture-of-Transformers (MoT)** architecture to integrate three experts (understanding, action, and video generation) and adopts a **UniDiffuser-style scheduler** to enable flexible switching between different modeling modes (World Models, Vision-Language-Action Models, Inverse Dynamics Models, Video Generation Models, and Video-Action Joint Prediction Models). Motus further leverages **optical flow** to learn **latent actions** and adopts a **three-phase training pipeline** and **six-layer data pyramid**, thereby extracting pixel-level "delta action" and enabling large-scale action pretraining.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">AAAI2026</div><img src='images/hrdt_aaai2025.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[H-RDT: Human Manipulation Enhanced Bimanual Robotic Manipulation](https://arxiv.org/abs/2507.23523)

**Hongzhe Bi**, Lingxuan Wu, Tianwei Lin, Hengkai Tan, Zhizhong Su, Hang Su, Jun Zhu

[**Project**](https://embodiedfoundation.github.io/hrdt) <strong><span class='show_paper_citations' data=''></span></strong>
- H-RDT (Human to Robotics Diffusion Transformer) is a novel approach that leverages human manipulation data to enhance robot manipulation capabilities.
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
- A Unified framework that reformulates existing long-context methods from the view of Memory augmentation of LLMs. 
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
- *2024.10 - 2026.03*, [Horizon Robotics Lab](https://horizonrobotics.github.io/robot_lab/main/index.html)
- *2024.04 - 2024.08*, [D-Robotics](https://d-robotics.cc/)
- *2023.10 - 2024.01*, [ModelBest](https://modelbest.cn/)
