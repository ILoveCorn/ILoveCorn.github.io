---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<span class="anchor" id="about-me"></span>

I am **Yan Ma (马彦)**, a Ph.D. student in Electronic Engineering at [The Chinese University of Hong Kong](https://www.ee.cuhk.edu.hk/), advised by [Prof. Hongliang Ren](https://www.ee.cuhk.edu.hk/en-gb/people/academic-staff/professors/prof-ren-hongliang). My research focuses on **medical imaging robotics**, with an emphasis on system calibration, surface inspection planning, and robot learning.

I develop robotic systems that connect visual perception with optical coherence tomography (OCT) for large-area skin imaging. My work spans uncertainty-aware hand-eye calibration, geometric and learning-based path planning, and vision-language-action (VLA) models for bimanual manipulation. My publications include *IEEE Transactions on Robotics*, *Nature Communications*, and *IEEE Transactions on Industrial Informatics*.

Before joining CUHK in January 2023, I received my B.Eng. in Mechanical Engineering from [Shanghai Jiao Tong University](https://en.sjtu.edu.cn/) in June 2022, ranking in the top 10% of my major. I expect to complete my Ph.D. in June 2027.

For research discussions and collaboration, please feel free to contact me at [yanloveoat@gmail.com](mailto:yanloveoat@gmail.com).

<h1 id="news">🔥 News</h1>

- **2026.08**: Completed a π₀.₅-driven bimanual manipulation project on the TRON2 robot, covering flower arranging, table tidying, and T-shirt folding.
- **2026**: Our uncertainty-aware OCT hand-eye calibration work is published in *IEEE Transactions on Robotics*. [Paper](https://doi.org/10.1109/TRO.2026.3710397) / [Code](https://github.com/ILoveCorn/2DCalib).
- **2026**: Our work on single twistable tendon-driven continuum robots is published in *Nature Communications*. [Paper](https://doi.org/10.1038/s41467-026-74225-3).

<span class="anchor" id="-publications"></span>
<h1 id="publications">📝 Publications</h1>

<h2>🤖 Medical Imaging and Robotics</h2>

{% include publications.html %}

<span class="anchor" id="-research"></span>
<h1 id="research">🔬 Research Projects</h1>

## Multimodal Skin Inspection Robot

**Project lead · January 2025 – present**

A robotic system integrating vision and OCT to automatically image large, complex skin regions and build 3D skin maps containing surface and tissue information.

- **Uncertainty-aware calibration**: Developed a plane-based OCT calibration model that explicitly represents pose uncertainty using Lie groups and Lie algebras. Joint optimization on a composite manifold uses analytical Jacobians and problem sparsity; the simulation evaluation reports approximately 80% lower orientation error and 10% lower position error than the best baseline. Published in [T-RO](https://doi.org/10.1109/TRO.2026.3710397); [calibration code](https://github.com/ILoveCorn/2DCalib) is available.
- **Surface inspection planning**: Built **ScanSim** with trimesh and Warp to measure coverage and overlap. Developed **ScanPlanner**, a heuristic planner that iteratively propagates seed curves into coverage paths; the related work has been submitted to *IEEE Robotics and Automation Letters*.
- **Learning to plan**: Use ScanPlanner demonstrations for supervised pretraining followed by reinforcement learning to generate inspection paths directly from point clouds.

## VLA-Driven Bimanual Manipulation

**Project lead · July – August 2026**

A π₀.₅-based system on the TRON2 dual-arm robot for flower arranging, table tidying, and T-shirt folding.

- Designed demonstration collection strategies, including randomized initial states and bimanual coordination.
- Compared full fine-tuning with LoRA fine-tuning using **openpi**.
- Reproduced **Real-time Action Chunking** for synchronized inference and execution.

<span class="anchor" id="-education"></span>
<h1 id="education">📖 Education</h1>

- **The Chinese University of Hong Kong**, Hong Kong \\
  Ph.D. in Electronic Engineering · January 2023 – June 2027 (expected) \\
  Advisor: Prof. Hongliang Ren · Research: medical imaging robotics.
- **Shanghai Jiao Tong University**, Shanghai \\
  B.Eng. in Mechanical Engineering · September 2018 – June 2022 \\
  Top 10% of the major · Selected coursework: Robotics and Numerical Analysis.

<span class="anchor" id="-skills"></span>
<h1 id="skills">🛠 Skills</h1>

- **Robotics**: kinematics and dynamics, system calibration, surface path planning.
- **Imitation learning**: ACT, Diffusion Policy, and π-series models; demonstration collection, model training, and deployment on physical robots.
- **Reinforcement learning**: PPO, SAC, Gymnasium, and Stable-Baselines3; experience training small reinforcement-learning models.
- **Computational geometry**: point cloud and triangle mesh processing.
- **Programming and tools**: Python, C/C++, MATLAB, Linux, Git, ROS, PyTorch, OpenCV, PCL, Ceres, and trimesh.
- **Hardware**: mechanical design and fabrication; robot arms, cameras, dexterous hands, and motion capture systems.
- **English**: IELTS 7.5 · CET-6 636.

<p class="template-credit">Built with <a href="https://github.com/RayeRen/acad-homepage.github.io">AcadHomepage</a>.</p>
