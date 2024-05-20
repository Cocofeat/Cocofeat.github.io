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

I'm currently pursuing the Ph.D. degree with the National Key Laboratory of Fundamental Science on Synthetic Vision, the College of Computer Science, Sichuan University, co-advised by [Prof. Xiaojing Shen](https://math.scu.edu.cn/info/1013/5806.htm) and [Prof. Xuedong Yuan](https://cs.scu.edu.cn/info/1359/17827.htm). He was sponsored by the China Scholarship Council (CSC) and participated in a joint doctoral training program at the Agency for Science, Technology and Research (A*STAR) in Singapore from September 2022 to September 2023, under the supervision of [Principal Scientist: Huazhu Fu](https://hzfu.github.io/). 

- 👯 I'm looking to collaborate on __Trustworthy multi-modality learning__ with uncertainty estimation.
- ⚡ I'm seeking __Postdoc/Research fellow__ position in 2024.

****
## His research focuses on: 
* 🔥 **AI+ Healthcare**: Medical image analysis, uncertainty estimation, multi-modal learning，vision-language model.
* **Computer Vision**: Point set registration.
* **Intelligent Vehicle**: Track2track association, multi-sensor fusion (lidar and camera).


# 🔥 News
- [05/2024] One paper about "Confidence-aware multi-modality learning for eye disease screening" was accepted by **MedIA** [[EyeMoSt+ Codes]](https://github.com/Cocofeat/EyeMoSt/tree/main/MedIA%E2%80%9924).
- [05/2024] Two papers about "Domain adaption" and "Semi-supervised segmentation" were early accepted by **MICCAI2024**.
- [10/2023] One paper about "Uncertainty-inspired open set learning for retinal anomaly identification" was accepted by **Nature Communications**.  [[pdf]]([https://www.nature.com/articles/s41467-023-42444-7]) [[code]](https://github.com/Cocofeat/UIOS)
- [07/2023] One paper about "A review of uncertainty estimation and its application in medical imaging" was accepted by **Meta-Radiology**.  [[pdf]](https://www.sciencedirect.com/science/article/pii/S2950162823000036)
- [06/2023] One paper about "Uncertainty-informed Mutual Learning for Joint Medical Image Classification and Segmentation" was accepted by **MICCAI'2023**.  [[pdf]](https://arxiv.org/abs/2303.09790) [[code]](https://github.com/Cocofeat/UML/)
- [06/2023] One paper about "Multi-modality learning with uncertainty estimation" was early accepted by **MICCAI'2023**.  [[pdf]](https://arxiv.org/abs/2303.10049) [[code]](https://github.com/Cocofeat/EyeMoSt/)
- [01/2023] One paper about "Artificial intelligence‐assisted determination of available sites for palatal orthodontic mini‐implants based on palatal thickness through CBCT" was accepted by **Orthodontics & Craniofacial Research**. 
- [08/2022] One paper about "An interactive dual-branch network for hard palate segmentation of the oral cavity from CBCT images" was accepted by **Applied Soft Computing**. 
- [07/2022] Happy to be funded by [[CSC]](https://www.csc.edu.cn/) **CSC: SCU and A\*STAR**. 
- [06/2022] One paper about "TBraTS: Trusted Brain Tumor Segmentation" was accepted by **MICCAI'2022**. 
 [[pdf]](https://arxiv.org/abs/2206.09309) [[code]](https://github.com/Cocofeat/TBraTS/)

# 📝 Publications (\* means co-first author)
## Trustworthy Medical Image Analysis
<div class='paper-box'><div class='paper-box-image'><div><div class="badge">NC 2023</div><img src='images/NC_UIOS.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Uncertainty-inspired open set learning for retinal anomaly identification](\https://www.nature.com/articles/s41467-023-42444-7)

Meng Wang\*, Tian Lin\*, Lianyu Wang\*, Aidi Lin, **Ke Zou**, et al.
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MICCAI 2022, IEEE TCyber submission</div><img src='images/MICCAI_DEviS.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Towards Reliable Medical Image Segmentation by utilizing Evidential Calibrated Uncertainty][[Conference]](https://arxiv.org/abs/2206.09309) [[Code]](https://github.com/Cocofeat/TBraTS)[[Journal]](https://arxiv.org/abs/2301.00349)[[Code]](https://github.com/Cocofeat/DEviS)

**Ke Zou**, Yidi Chen, Ling Huang, Xuedong Yuan, Xiaojing Shen, Meng Wang, Rick Siow Mong Goh, Yong Liu, Huazhu Fu
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MICCAI 2023 Early Accept, MedIA</div><img src='images/MICCAI_EyeMoSt.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Reliable Multimodality Eye Disease Screening via Mixture of Student's t Distributions](https://link.springer.com/chapter/10.1007/978-3-031-43990-2_56)[[EyeMoSt+/EyeMoSt Codes]](https://github.com/Cocofeat/EyeMoSt/tree/main/MedIA%E2%80%9924)

**Ke Zou**\*, Tian Lin\*, Xuedong Yuan, Haoyu Chen, Xiaojing Shen, Meng Wang, Huazhu Fu
</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MICCAI 2023</div><img src='images/MICCAI_UMML.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Uncertainty-informed Mutual Learning for Joint Medical Image Classification and Segmentation](https://link.springer.com/chapter/10.1007/978-3-031-43901-8_4)

Kai Ren\*, **Ke Zou**\*, Xianjie Liu, Yidi Chen, Xuedong Yuan, Xiaojing Shen, Meng Wang, Huazhu Fu
</div>
</div>

## Vision-language/Foundation model
<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">MICCAI 2024 Submission</div><img src='images/MICCAI_MRG.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[MedRG: Medical Report Grounding with Multi-modal Large Language Model](https://arxiv.org/abs/2404.06798)

**Ke Zou**\*, Yang Bai\*, Zhihao Chen, Yang Zhou, Yidi Chen, Kai Ren, Meng Wang, Xuedong Yuan, Xiaojing Shen, Huazhu Fu
</div>
</div>
-->

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MICCAI 2023 workshop</div><img src='images/MICCAI_SAMU.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SAM-U: Multi-box Prompts Triggered Uncertainty Estimation for Reliable SAM in Medical Image](https://link.springer.com/chapter/10.1007/978-3-031-47425-5_33)

Guoyao Deng, **Ke Zou**, Kai Ren, Meng Wang, Xuedong Yuan, Sancong Ying, Huazhu Fu
</div>
</div>

# 🎖 Honors and Awards
- 2021.12 – Outstanding Graduate Thesis of Chongqing
- 2021.09 – Outstanding Postgraduate of Sichuan University
- 2020.06 – Outstanding Graduate Student of Chongqing
- 2017.06 - Outstanding Undergraduate Student of Chongqing
- 2015.11 – National Scholarship (1%)

# 🗣 Activities
## Reviewers
- Conference Reviewer: ***FUSION2022***, ***ICASSP2023, ICASSP2024***, ***MIDL2023, MIDL2024***, ***MICCAI2023, MICCAI2024***, ***ICIP2023, ICIP2024***
- Journal Reviewer: ***IEEE TMI***, ***Signal Processing***, ***IEEE TAI***, ***IEEE JBHI***, ***IEEE Access***

# 💬 Talks and Presentations
- *2024.04*, AIxMed Biweekly Seminar, curated by the MGH/HMS Center for Advanced Medical Computing and Analysis (CAMCA), invited by [Prof. Xiang Li](https://xiangli-shaun.github.io/).
- *2023.12*, Central China Normal University Nanhu Forum academic exchange report, curated by School of Computer Science, Central China Normal University, invited by [Prof. Yutao Ma](https://cs.ccnu.edu.cn/info/1109/2702.htm).
- *2023.11*, The Third Graduate Academic Forum, curated by Chinese Journal of Graphics and Images.
- *2022.08* [MICS2022](https://aim.nuist.edu.cn/events/mics2022.htm) of [TBraTS: Trusted Brain Tumor Segmentation](https://www.bilibili.com/video/BV1nW4y1a7Qp/?spm_id_from=333.337.search-card.all.click&vd_source=6ab19d355475883daafd34a6daae54a5) (**3rd Prize**)
- *2019.07*, FUSION2019, Ottawa, Canada.

# 📖 Educations
- *2020.09 - 2024.06 (now)*, Ph.D, Sichuan University, Chengdu.
- *2017.09 - 2020.06*, M.S, Chongqing University of Posts and Telecomunications.

# 💻 Experiences and Projects

## Experiences

- *2022.10 - 2023.09*, Visiting student, A*STAR, Singapore, advised by [Principal Scientist: Huazhu Fu](https://hzfu.github.io/).

## Projects

- *2019.04 - 2020.04*, Chongqing Postgraduate Research and Innovation Project, Multi-vehicle Lidar Integrated Registration based on Variational Bayesian under Time and Space Factors, **PI, 10,000 RMB**.
- *2021.10 - 2022.09*, Sichuan Provincial Department of Science and Technology, Cultivation Project, Joint Registration, Fusion and Segmentation of Multimodal Medical Image Based on Deep Neural Network, **PI, 30,000 RMB**.
- *2022.10 - 2023.09*, A*STAR SERC Central Research Fund, Robust and Trustworthy AI system for Multi-modality Healthcare, **Key member**.
- *2021.01 - 2024.12*, National Natural Science Foundation of China, Target Tracking of Intelligent Networked Vehicles under Time-varying non-Gaussian Noise and Positioning Failure in Mixed Traffic, **Key member**.
- *2023.01 - 2024.12*, Key research and development project in Sichuan Province, research on the key problems of oral hard palate segmentation and its application in orthodontic treatment, **Key member**.

<a href="http://s01.flagcounter.com/more/V8"><img src="https://s01.flagcounter.com/map/V8/size_s/txt_000000/border_CCCCCC/pageviews_0/viewers_0/flags_0/" alt="Flag Counter" border="0"></a>
