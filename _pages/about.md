---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

<style>
  dl {
    margin-bottom: 60px; /* 调整这个值以获得合适的间距 */
    clear: both;
  }

  /* 全局文本颜色 */
  body {
    color: #333; /* 主要文本颜色 */
  }

  /* 链接颜色 */
  a {
    color: #0066cc; /* 链接颜色 */
  }

  /* 作者名字颜色 */
  strong {
    color: #000; /* 作者名字颜色 */
  }

  /* 年份标题颜色 */
  .year-title {
    color: #666;
  }

  /* 会议标签样式 */
  .conference-label {
    position: absolute;
    top: 10px;
    left: -5px;
    background-color: #2c3e50;  /* 深蓝色背景 */
    color: white;  /* 白色文字 */
    padding: 6px 12px;
    border-radius: 6px;
    font-size: 0.95em;
    font-weight: 600;
    letter-spacing: 0.5px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
    z-index: 1;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    font-style: italic;  /* 添加斜体 */
  }

  /* 鼠标悬停效果 */
  .conference-label:hover {
    background-color: #34495e;  /* 悬停时稍微变亮 */
    transition: background-color 0.2s ease;
  }

  dl dt img {
    width: 100%; /* 在移动端默认占满宽度 */
    aspect-ratio: 2/1; /* 设置宽高比为2:1，即高度为宽度的一半 */
    object-fit: cover; /* 确保图片不会被裁剪 */
    display: block;
    margin: 10px 10px 10px 0px; /* 适当的间距 */
    
    /* 添加美化效果 */
    border-radius: 8px; /* 让图片有轻微的圆角 */
    border: 2px solid #ddd; /* 添加淡灰色的边框 */
    box-shadow: 3px 3px 10px rgba(0, 0, 0, 0.2); /* 添加轻微阴影 */
    padding: 5px; /* 给图片一些内边距，让它不贴着边框 */
    background-color: #fff; /* 设置背景色，让图片更加干净 */
  }

  /* 在桌面端（宽度大于768px）时固定宽度 */
  @media screen and (min-width: 768px) {
    dl dt img {
      width: 350px;
    }
  }

  dl dt {
    position: relative;
  }

  hr {
    border: 1px solid #ebebeb; /* 调整分隔线的颜色和样式 */
    /* margin: 10px;  */
    clear: both; 
  }

  dl dd {
  margin-top: 5px; 
  margin-bottom: 5px;
}

  dl dd strong {
  font-weight: bold;
  color: black;
  }

  .co-first {
    color: red;
  }

  .down {
    transform: rotate(180deg);
  }

  /* 教育和工作经历卡片样式 */
  .experience-card, .education-card {
    display: flex;
    align-items: center;
    gap: 25px;
    margin-bottom: 30px;
    padding: 20px;
    background: #f8f9fa;
    border-radius: 12px;
    transition: all 0.3s ease;
    border: 1px solid #e9ecef;
  }

  .experience-card:hover, .education-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 4px 15px rgba(0, 0, 0, 0.1);
    border-color: #dee2e6;
  }

  .experience-info, .education-info {
    flex: 1;
  }

  .experience-logo, .education-logo {
    flex-shrink: 0;
    width: 100px;
    height: 100px;
    display: flex;
    align-items: center;
    justify-content: center;
    background: white;
    border-radius: 10px;
    padding: 10px;
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.05);
  }

  .experience-logo img, .education-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
  }

  .experience-title, .education-title {
    font-size: 1.2em;
    margin-bottom: 8px;
    color: #2c3e50;
  }

  .experience-title a, .education-title a {
    color: #2c3e50;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .experience-title a:hover, .education-title a:hover {
    color: #3498db;
  }

  .experience-role, .education-role {
    color: #666;
    font-style: italic;
    margin-bottom: 5px;
  }

  .experience-topics, .education-topics {
    color: #666;
    font-style: italic;
  }

  .section-title {
    font-size: 1.8em;
    color: #2c3e50;
    margin: 40px 0 20px;
    padding-bottom: 10px;
    border-bottom: 2px solid #ecf0f1;
  }

  /* 奖学金和荣誉部分样式 */
  .honors-list {
    list-style: none;
    padding: 0;
  }

  .honors-list li {
    margin-bottom: 15px;
    padding: 15px 20px;
    background: #f8f9fa;
    border-radius: 8px;
    border-left: 4px solid #3498db;
    transition: transform 0.3s ease, box-shadow 0.3s ease;
  }

  .honors-list li:hover {
    transform: translateX(5px);
    box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
  }

  .honors-list li strong {
    color: #2c3e50;
  }

  .honors-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .honors-list li a:hover {
    color: #2980b9;
  }

  /* 服务部分样式 */
  .service-section {
    margin-bottom: 30px;
  }

  .service-section h3 {
    color: #2c3e50;
    font-size: 1.3em;
    margin: 25px 0 15px;
    padding-bottom: 8px;
    border-bottom: 2px solid #ecf0f1;
  }

  .service-list {
    list-style: none;
    padding: 0;
  }

  .service-list li {
    margin-bottom: 12px;
    padding: 12px 15px;
    background: #f8f9fa;
    border-radius: 6px;
    transition: transform 0.3s ease;
  }

  .service-list li:hover {
    transform: translateX(5px);
  }

  .service-list li a {
    color: #3498db;
    text-decoration: none;
    transition: color 0.3s ease;
  }

  .service-list li a:hover {
    color: #2980b9;
  }
</style>

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

I am currently a Ph.D. student at the [Department of Computer Science and Engineering](https://www.cs.sjtu.edu.cn/) of [Shanghai Jiao Tong University (SJTU)](https://en.sjtu.edu.cn/), advised by Prof. [Dacheng Tao](https://scholar.google.com/citations?user=RwlJNLcAAAAJ&hl=zh-CN&oi=ao) and Prof. [Ya Zhang](https://scholar.google.com/citations?user=pbjw9sMAAAAJ&hl=zh-CN&oi=ao). I received my bachelor's degree from Shanghai Jiao Tong University in June 2022, during which I worked as a research assistant at [ThinkLab](https://thinklab.sjtu.edu.cn/) under the guidance of Prof. [Junchi Yan](https://scholar.google.com/citations?user=ga230VoAAAAJ&hl=zh-CN&oi=ao).

**I am open to potential collaborations. If you are interested, please feel free to contact me via email.**

# 🔎 Research 
My current research interests focus on two key areas:

- **Computer Vision:** autonomous driving, embodied AI
- **Machine Learning:** reinforcement learning, continuous learning
- **LLM:** agentical RL


# 🔥 News

<div style="max-height: 350px; overflow-y: auto; padding: 20px; background: #f8f9fa; border-left: 4px solid #2c3e50; margin: 0px 0;">
<style>
  /* 为 Webkit 浏览器（Chrome, Safari, Edge）设置滚动条样式 */
  div::-webkit-scrollbar {
    width: 8px;
  }

  div::-webkit-scrollbar-track {
    background: #e9ecef;
    border-radius: 4px;
  }

  div::-webkit-scrollbar-thumb {
    background: #2c3e50;
    border-radius: 4px;
  }

  div::-webkit-scrollbar-thumb:hover {
    background: #1a252f;
  }

  /* 为 Firefox 设置滚动条样式 */
  div {
    scrollbar-width: thin;
    scrollbar-color: #2c3e50 #e9ecef;
  }
</style>
<ul style="list-style-type: none; padding-left: 0; margin: 0;">
  <li><em>[Jan. 2026]</em> Three papers are accepted to ICLR 2026.</li>
  <li><em>[Jan. 2026]</em> One paper is accepted to TKDE.</li>
  <li><em>[Sep. 2025]</em> Two papers are accepted to NeurIPS 2025.</li>
  <li><em>[Sep. 2025]</em> I received an outstanding doctoral student scholarship.</li>
  <li><em>[Aug. 2025]</em> One paper is accepted to SCIS (CCF-A Journal).</li>
  <li><em>[Apr. 2025]</em> One paper is accepted to J-STSP (IEEE Journal of Selected Topics in Signal Processing).</li>
  <li><em>[Feb. 2025]</em> One paper is accepted to SCIS (CCF-A Journal).</li>
  <li><em>[Feb. 2025]</em> One paper is accepted to ICLR 2025 (Oral).</li>
  <li><em>[Jan. 2025]</em> I was selected as Young Talent Support Project Doctoral Special Program (青年人才托举工程博士生专项计划).</li>
  <li><em>[Dec. 2024]</em> One paper is accepted to AAMAS 2025.</li>
  <li><em>[Dec. 2024]</em> I went to NTU for one year of research.</li>
  <li><em>[Nov. 2024]</em> I received the national scholarships of 2024.</li>
  <li><em>[Sep. 2024]</em> One paper is accepted to NeurIPS 2024.</li>
  <li><em>[May. 2024]</em> One paper is accepted to TPAMI.</li>
  <li><em>[May. 2024]</em> Three papers are accepted to ICML 2024.</li>
  <li><em>[Jan. 2024]</em> Our paper about multi-agent communication is accepted to ICLR 2024.</li>
  <li><em>[Jun. 2022]</em> Our paper about autonomouse driving is accepted to ECCV 2022.</li>
</ul>
</div>

# 📝 Publications ([Full List](https://scholar.google.com/citations?user=dOsBnNkAAAAJ&hl=zh-CN&oi=ao))

<div style="text-align: left; margin: 20px 0; font-size: 1.5em; color: #666;">
2026
</div>
<ul>
    <li>
      The State of Reinforcement Finetuning for Transformer-based Generative Agents
      <br><b>Shengchao Hu</b>, Guozheng Ma, Shi Fu, Peng Wang, Li Shen, Ya Zhang, Dacheng Tao<br>
      <i>International Conference on Learning Representations (<b>ICLR</b>), <b><font color="#9400D3">non-CCF</font></b>, 2026</i><br>
      [<a href="https://openreview.net/forum?id=Cbg9MR6dR7">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Rethinking Data Curation in LLM Training: Online Reweighting Offers Better Generalization than Offline Methods
      <br>Wanru Zhao, Yihong Chen, Wentao Ma, Yuzhi Tang, <b>Shengchao Hu</b>, Shell Xu Hu, Alex Iacob, Abhinav Mehrotra, Nicholas D Lane<br>
      <i>International Conference on Learning Representations (<b>ICLR</b>), <b><font color="#9400D3">non-CCF</font></b>, 2026</i><br>
      [<a href="https://openreview.net/forum?id=UFwnsmFZ6R">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Understanding the Dynamics of Forgetting and Generalization in Continual Learning via the Neural Tangent Kernel
      <br>Guodong Zheng, <b>Shengchao Hu</b>, Peng Wang, Quan Zheng, Li Shen<br>
      <i>International Conference on Learning Representations (<b>ICLR</b>), <b><font color="#9400D3">non-CCF</font></b>, 2026</i><br>
      [<a href="https://openreview.net/forum?id=NE2yIxdo1w">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Communication Learning in Multi-Agent Systems from Graph Modeling Perspective
      <br><b>Shengchao Hu</b>, Li Shen, Ya Zhang, Dacheng Tao<br>
      <i>IEEE Transactions on Knowledge and Data Engineering (<b>TKDE</b>), <b><font color="red">CCF-A</font></b>, 2026</i><br>
      [<a href="https://arxiv.org/abs/2411.00382">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
</ul>
<div style="text-align: left; margin: 20px 0; font-size: 1.5em; color: #666;">
2025
</div>
<ul>
    <li>
      Analytic Energy-Guided Policy Optimization for Offline Reinforcement Learning
      <br>Jifeng Hu, Sili Huang, Zhejian Yang, <b>Shengchao Hu</b>, Li Shen, Hechang Chen, Lichao Sun, Yi Chang, Dacheng Tao<br>
      <i>Neural Information Processing Systems (<b>NeurIPS</b>), <b><font color="red">CCF-A</font></b>, 2025</i><br>
      [<a href="https://arxiv.org/abs/2505.01822">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Tackling Continual Offline RL through Selective Weights Activation on Aligned Spaces
      <br>Jifeng Hu, Sili Huang, Li Shen, Zhejian Yang, <b>Shengchao Hu</b>, Shisong Tang, Hechang Chen, Lichao Sun, Yi Chang, Dacheng Tao<br>
      <i>Neural Information Processing Systems (<b>NeurIPS</b>), <b><font color="red">CCF-A</font></b>, 2025</i><br>
      [<a href="https://arxiv.org/abs/2410.15698">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Prompt-tuning Decision Transformer with Preference Ranking
      <br><b>Shengchao Hu</b>, Li Shen, Ya Zhang, Dacheng Tao<br>
      <i>Science China Information Sciences (<b>SCIS</b>), <b><font color="red">CCF-A</font></b>, 2025</i><br>
      [<a href="https://arxiv.org/abs/2305.09648">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Reconstruct the Pruned Model without Any Retraining
      <br>Pingjie Wang, Ziqing Fan, <b>Shengchao Hu</b>, Zhe Chen, Yanfeng Wang, Yu Wang,<br>
      <i>IEEE Journal of Selected Topics in Signal Processing (<b>J-STSP</b>), <b><font color="#4169e1">SCI 2</font></b>, 2025</i><br>
      [<a href="https://arxiv.org/abs/2407.13331">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
   </li>
    <li>
      Graph decision transformer for offline reinforcement learning
      <br><b>Shengchao Hu</b>, Li Shen, Ya Zhang, Dacheng Tao,<br>
      <i>Science China Information Sciences (<b>SCIS</b>), <b><font color="red">CCF-A</font></b>, 2025</i><br>
      [<a href="https://link.springer.com/article/10.1007/s11432-024-4353-9">Paper</a>][<a href="https://github.com/charleshsc/Graph-DT">Code</a>]
   </li>
    <li>
      Combatting Dimensional Collapse in LLM Pre-Training Data via Diversified File Selection
      <br>Ziqing Fan, Siyuan Du, <b>Shengchao Hu</b>, Pingjie Wang, Li Shen, Ya Zhang, Dacheng Tao, Yanfeng Wang,<br>
      <i>International Conference on Learning Representations (<b>ICLR</b>), <b><font color="#9400D3">non-CCF, Oral</font></b>, 2025</i><br>
      [<a href="https://arxiv.org/abs/2504.20644">Paper</a>][<a href="https://github.com/MediaBrain-SJTU/DiSF">Code</a>]
   </li>
   <li>
      Prompt Tuning with Diffusion for Few-Shot Pre-trained Policy Generalization
      <br><b>Shengchao Hu</b>, Wanru Zhao, Weixiong Lin, Li Shen, Ya Zhang, Dacheng Tao,<br>
      <i>International Conference on Autonomous Agents and Multiagent Systems (<b>AAMAS</b>), <b><font color="#4169e1">CCF-B</font></b>, 2025</i><br>
      [<a href="https://arxiv.org/pdf/2411.01168">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
   </li>
</ul>
<div style="text-align: left; margin: 20px 0; font-size: 1.5em; color: #666;">
2024
</div>
<ul>
    <li>
      On Transforming Reinforcement Learning by Transformer: The Development Trajectory
      <br><b>Shengchao Hu</b>, Li Shen, Ya Zhang, Yixin Chen, Dacheng Tao,<br>
      <i>IEEE Transactions on Pattern Analysis and Machine Intelligence (<b>TPAMI</b>), <b><font color="red">CCF-A</font></b>, 2024</i><br>
      [<a href="https://ieeexplore.ieee.org/abstract/document/10546317">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Is Mamba Compatible with Trajectory Optimization in Offline Reinforcement Learning?
      <br>Yang Dai, Oubo Ma, Longfei Zhang, Xingxing Liang, <b>Shengchao Hu</b>, Mengzhu Wang, Shouling Ji, Jincai Huang, Li Shen,<br>
      <i>Neural Information Processing Systems (<b>NeurIPS</b>), <b><font color="red">CCF-A</font></b>, 2024</i><br>
      [<a href="https://arxiv.org/abs/2405.12094">Paper</a>][<a href="https://charleshsc.github.io/">Code</a>]
    </li>
    <li>
      Locally Estimated Global Perturbations is Better than Local Perturbations for Federated Sharpness-aware Minimization
      <br>Ziqing Fan, <b>Shengchao Hu</b>, Jiangchao Yao, Gang Niu, Ya Zhang, Masashi Sugiyama, Yanfeng Wang,<br>
      <i>International Conference on Machine Learning (<b>ICML</b>), <b><font color="red">CCF-A, Spotlight</font></b>, 2024</i><br>
      [<a href="https://arxiv.org/abs/2405.18890">Paper</a>][<a href="https://github.com/MediaBrain-SJTU/FedLESAM">Code</a>]
    </li>
    <li>
      HarmoDT: Harmony Multi-Task Decision Transformer for Offline Reinforcement Learning
      <br><b>Shengchao Hu</b>, Ziqing Fan, Li Shen, Ya Zhang, Yanfeng Wang, Dacheng Tao,<br>
      <i>International Conference on Machine Learning (<b>ICML</b>), <b><font color="red">CCF-A</font></b>, 2024</i><br>
      [<a href="https://arxiv.org/abs/2405.18080">Paper</a>][<a href="https://github.com/charleshsc/HarmoDT">Code</a>]
    </li>
    <li>
      Q-value Regularized Transformer for Offline Reinforcement Learning
      <br><b>Shengchao Hu</b>, Ziqing Fan, Chaoqin Huang, Li Shen, Ya Zhang, Yanfeng Wang, Dacheng Tao,<br>
      <i>International Conference on Machine Learning (<b>ICML</b>), <b><font color="red">CCF-A</font></b>, 2024</i><br>
      [<a href="https://arxiv.org/abs/2405.17098">Paper</a>][<a href="https://github.com/charleshsc/QT">Code</a>]
    </li>
    <li>
      Learning Multi-Agent Communication from Graph Modeling Perspective
      <br><b>Shengchao Hu</b>, Li Shen, Ya Zhang, Dacheng Tao,<br>
      <i>International Conference on Learning Representations (<b>ICLR</b>), <b><font color="#9400D3">non-CCF</font></b>, 2024</i><br>
      [<a href="https://arxiv.org/abs/2405.08550">Paper</a>][<a href="https://github.com/charleshsc/CommFormer">Code</a>]
    </li>
</ul>
<div style="text-align: left; margin: 20px 0; font-size: 1.5em; color: #666;">
2022
</div>
<ul>
   <li>
      St-p3: End-to-end vision-based autonomous driving via spatial-temporal feature learning
      <br><b>Shengchao Hu</b>, Li Chen, Penghao Wu, Hongyang Li, Junchi Yan, Dacheng Tao,<br>
      <i>European Conference on Computer Vision (<b>ECCV</b>), <b><font color="#4169e1">CCF-B</font></b>, 2022</i><br>
      [<a href="https://arxiv.org/abs/2207.07601">Paper</a>][<a href="https://github.com/OpenDriveLab/ST-P3">Code</a>]
   </li>
</ul>

# 🎖 Honors and Awards
- *2025.09* 85届计算机系教育发展基金暨杨元庆教育基金优秀博士生奖学金
- *2025.01* Young Talent Support Project Doctoral Special Program (青年人才托举工程博士生专项计划)
- *2024.09* National Scholarships 
- *2020-2021* Shanghai Jiao Tong University Category C Scholarship
- *2018-2022* Zhiyuan Honor Scholarship of Shanghai Jiao Tong University
- *2020.12* Interdisciplinary Contest In Modeling, Honorable Mention
- *2020.12* National Undergraduate Mathematical Modeling Contest in Shanghai Division, Second Prize
- *2019.11* Non-Mathematics Category of Shanghai College Student Mathematics Competition (Higher Education Society Cup), First Prize

# 📖 Educations

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>2022.09 - Now</strong><br/>
      PhD, Computer Science, Shanghai Jiao Tong University
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/SJTU.png" alt="SJTU Logo" />
  </div>
</div>

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>2024.11 - 2025.11</strong><br/>
      PhD Visiting Student, Computer Science, Nanyang Technological University (NTU)
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/NTU.png" alt="NTU Logo" />
  </div>
</div>

<div class="education-card">
  <div class="education-info">
    <div class="education-title">
      <strong>2018.09 - 2022.06</strong><br/>
      Bachelor, Computer Science, Shanghai Jiao Tong University
    </div>
  </div>
  <div class="education-logo">
    <img src="../images/SJTU.png" alt="SJTU Logo" />
  </div>
</div>


# 🎡 Service

<div class="service-section">
  <h3>Conference Committee Member</h3>
  <ul class="service-list">
    <li><a href="https://icml.cc/"><autocolor>International Conference on Machine Learning (ICML)</autocolor></a></li>
    <li><a href="https://iclr.cc/"><autocolor>International Conference on Learning Representations (ICLR)</autocolor></a></li>
    <li><a href="https://neurips.cc/"><autocolor>Neural Information Processing Systems (NeurIPS)</autocolor></a></li>
    <li><a href="http://cvpr2024.thecvf.com/"><autocolor>IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR)</autocolor></a></li>
    <li><a href="https://iccv.thecvf.com/"><autocolor>International Conference on Computer Vision (ICCV)</autocolor></a></li>
    <li><a href="https://aaai.org/conference/aaai/aaai-25/"><autocolor>The Association for the Advancement of Artificial Intelligence (AAAI)</autocolor></a></li>
  </ul>
</div>

<div class="service-section">
  <h3>Journal Reviewer</h3>
  <ul class="service-list">
    <li><a href="https://cis.ieee.org/publications/t-neural-networks-and-learning-systems"><autocolor>IEEE Transactions on Neural Networks and Learning Systems (TNNLS)</autocolor></a></li>
  <li><a href="https://www.ieee-ras.org/publications/ra-l"><autocolor>IEEE Robotics and Automation Letters (RA-L)</autocolor></a></li>
  </ul>
</div>

# 💻 Internships

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://dr.ntu.edu.sg/entities/person/Tao-Dacheng">GenAI Lab</a>, Nanyang Technological University
    </div>
    <div class="experience-role">Research Assistant, 2024-2025</div>
    <div class="experience-topics">Mentor: Dacheng Tao</div>
  </div>
  <div class="experience-logo">
    <img src="../images/NTU.png" alt="NTU Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://annzhanglion.github.io/">Smart Medical Research</a>, Shanghai AI Lab
    </div>
    <div class="experience-role">Research Assistant, 2023-2024</div>
    <div class="experience-topics">Mentor: Ya Zhang</div>
  </div>
  <div class="experience-logo">
    <img src="../images/ailab.png" alt="ailab Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://opendrivelab.com/">OpenDriveLab</a>, SenseTime
    </div>
    <div class="experience-role">Research Intern, 2021-2022</div>
    <div class="experience-topics">Topics: Autonomous Driving</div>
    <div class="experience-topics">Mentor: Hongyang Li</div>
  </div>
  <div class="experience-logo">
    <img src="../images/sensetime.png" alt="sensetime Logo" />
  </div>
</div>

<div class="experience-card">
  <div class="experience-info">
    <div class="experience-title">
      <a href="https://thinklab.sjtu.edu.cn/">ThinkLab</a>, Shanghai Jiao Tong University
    </div>
    <div class="experience-role">Research Assistant, 2019-2022</div>
    <div class="experience-topics">Mentor: Junchi Yan</div>
  </div>
  <div class="experience-logo">
    <img src="../images/SJTU.png" alt="SJTU Logo" />
  </div>
</div>

<div id="footer">
	<div id="footer-text"></div>
</div>
