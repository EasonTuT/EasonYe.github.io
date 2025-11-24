---
permalink: /
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---
<style>
    .experience-card {
        display: flex;
        align-items: center;
        background: #f9f9f9;
        border-radius: 12px;
        padding: 16px;
        margin-bottom: 0px;
        box-shadow: 0 4px 8px rgba(0,0,0,0.05);
        transition: transform 0.3s, box-shadow 0.3s;
    }
    .experience-card:hover {
       
        box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    }
    .experience-logo {
        width: 60px;
        height: 60px;
        margin-right: 20px;
        border-radius: 8px;
        object-fit: contain;
    }
    .experience-info {
        font-family: "Segoe UI", sans-serif;
    }
    .experience-info strong {
        font-size: 1.1em;
    }
    .experience-info a {
        text-decoration: none;
        color: #ca6f6f;
    }
    .experience-container {
        display: grid;
        grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
        gap: 20px;
    }
    .experience-card {
        box-sizing: border-box;
    }
    .publication-card {
        display: flex;
        align-items: center;
        padding: 3px;
        border: 1.5px solid #ddd;
        border-radius: 8px;
        background: #fff;
        box-sizing: border-box;
        margin-bottom: 20px; 
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .publication-card:hover {
       
        box-shadow: 0 8px 16px rgba(0,0,0,0.1);
    }

    .publication-card.featured {
        border-color: #f5bba7;       /* 更浅的哈密瓜色边框 */
        background: #fef5f1;         /* 非常浅的哈密瓜色背景 */
        box-shadow: 0 4px 8px rgba(242, 166, 120, 0.2); /* 更柔和的初始阴影 */
        z-index: 10;
    }

    .publication-card.featured:hover {
        box-shadow: 0 8px 16px rgba(242, 166, 120, 0.4); 
    }
    
</style>
<html> 
<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Fredericka+the+Great&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Homemade+Apple&display=swap');
        body {
            background-color:	 #FFFFFF;
            font-family: 'Arial Rounded MT Bold', 'Verdana', sans-serif;
            font-size: 15px;
        }
        .main-heading {
            font-family: 'Permanent Marker', cursive;
            text-align: center;
            color: #ca6f6f;
        }
        div.markdown-body a,a {
            text-decoration: none !important;
            color: #ca6f6f;
            transition: all 0.3s ease; /* 平滑过渡效果 */
        }
        div.markdown-body a:hover, a:hover {
            color: #c71585;            /* 悬浮时变深一点的颜色 */
            text-decoration: underline; /* 加上悬浮时的下划线 */
        }
    </style>
</head>
<body>
<h1 class="main-heading">Hi there <img src="images/Hi.gif" width="40px"> Welcome to my Homepage!</h1>
</body>
</html>

I am an undergraduate (2022-2026) at Shantou University, focusing on World Model and Multi-modal.

I work at [JPG@CSU](https://csu-jpg.github.io) with [Prof. Alex Jinpeng Wang](https://fingerrec.github.io).
Previously I worked at Shantou University with [Prof. Cheng Liu](https://cliu272.github.io).

News
---------------
- *[SMART] is accepted in IEEE TCSVT &#128293;*
- *[scRCL] is accepted in AAAI 2026 &#128293;*
- *[NeuCGC] is accepted in IEEE TKDE &#128293;*
- *[CVNC] is accepted in ICME 2025 &#128293;*

Selected Publications
--------------
<div class="publication-card featured">
    <div style="display: flex; align-items: center;">
        <img src="images/iraa.png" alt="Raa" width="200" height="100" style="margin-right: 20px;">
        <div>
            <strong>SMART: Semantic Matching Contrastive Learning for Partially View-Aligned Clustering</strong><br>
            <i style="font-size: 13px;">
                <a href="" target="_blank">Liang Peng</a>*,
                <a href="" target="_blank"><strong>Yixuan Ye<strong></a>*,
                <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger,
                <a href="" target="_blank">Hangjun Che</a>,
                <a href="" target="_blank">Fei Wang</a>,
                <a href="" target="_blank">Zhiwen Yu</a>,
                <a href="" target="_blank">Si Wu</a>,
                <a href="" target="_blank">Hau-San Wong</a>;
            </i>
            <!-- <br>
            Propose Dense Policy, A bidirectional robotic autoregressive policy, which infers trajectories by gradually expanding actions from sparse keyframes, demonstrated exceeding diffusion policies.
            <br> -->
            <b><i style="color:#83a1c7;">IEEE TCSVT (CCF-B, 中科院一区Top, IF:11.1) &nbsp;</i></b>
            <a href=""><em>[paper]</em></a>
            <a href="https://github.com/THPengL/SMART"><em>[code]</em></a>
        </div>
    </div>
</div>

<div class="publication-card featured">
    <div style="display: flex; align-items: center;">
        <img src="images/iraa.png" alt="Raa" width="200" height="100" style="margin-right: 20px;">
        <div>
            <strong>Refinement Contrastive Learning of Cell-Gene Associations for Unsupervised Cell Type Identification</strong><br>
            <i style="font-size: 13px;">
                <a href="" target="_blank">Liang Peng</a>*,
                <a href="" target="_blank">Haopeng Liu</a>*,
                <a href="" target="_blank"><strong>Yixuan Ye<strong></a>*,
                <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger,
                <a href="" target="_blank">Wenjun Shen</a>,
                <a href="" target="_blank">Si Wu</a>,
                <a href="" target="_blank">Hau-San Wong</a>;
            </i>
            <!-- <br>
            Propose Dense Policy, A bidirectional robotic autoregressive policy, which infers trajectories by gradually expanding actions from sparse keyframes, demonstrated exceeding diffusion policies.
            <br> -->
            <b><i style="color:#83a1c7;">AAAI 2026 (CCF-A) &nbsp;</i></b>
            <a href=""><em>[paper]</em></a>
            <a href="https://github.com/THPengL/scRCL"><em>[code]</em></a>
        </div>
    </div>
</div>

<div class="publication-card featured">
    <div style="display: flex; align-items: center;">
        <img src="images/iraa.png" alt="Raa" width="200" height="100" style="margin-right: 20px;">
        <div>
            <strong>Trustworthy Neighborhoods Mining: Homophily-Aware Neutral Contrastive Learning for Graph Clustering</strong><br>
            <i style="font-size: 13px;">
                <a href="" target="_blank">Liang Peng</a>*,
                <a href="" target="_blank"><strong>Yixuan Ye<strong></a>*,
                <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger,
                <a href="" target="_blank">Hangjun Che</a>,
                <a href="" target="_blank">Fei Wang</a>,
                <a href="" target="_blank">Zhiwen Yu</a>,
                <a href="" target="_blank">Si Wu</a>,
                <a href="" target="_blank">Hau-San Wong</a>;
            </i>
            <!-- <br>
            Propose Dense Policy, A bidirectional robotic autoregressive policy, which infers trajectories by gradually expanding actions from sparse keyframes, demonstrated exceeding diffusion policies.
            <br> -->
            <b><i style="color:#83a1c7;">IEEE TKDE (CCF-A, 中科院一区Top, IF:10.4) &nbsp;</i></b>
            <a href="https://ieeexplore.ieee.org/abstract/document/11206540"><em>[paper]</em></a>
            <a href="https://github.com/THPengL/NeuCGC"><em>[code]</em></a>
        </div>
    </div>
</div>

<div class="publication-card featured">
    <div style="display: flex; align-items: center;">
        <img src="images/iraa.png" alt="Raa" width="200" height="100" style="margin-right: 20px;">
        <div>
            <strong>Trustworthy Neighborhoods Mining: Homophily-Aware Neutral Contrastive Learning for Graph Clustering</strong><br>
            <i style="font-size: 13px;">
                <a href="" target="_blank">Liang Peng</a>*,
                <a href="" target="_blank"><strong>Yixuan Ye<strong></a>*,
                <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger,
                <a href="" target="_blank">Hangjun Che</a>,
                <a href="" target="_blank">Fei Wang</a>,
                <a href="" target="_blank">Zhiwen Yu</a>,
                <a href="" target="_blank">Si Wu</a>,
                <a href="" target="_blank">Hau-San Wong</a>;
            </i>
            <!-- <br>
            Propose Dense Policy, A bidirectional robotic autoregressive policy, which infers trajectories by gradually expanding actions from sparse keyframes, demonstrated exceeding diffusion policies.
            <br> -->
            <b><i style="color:#83a1c7;">IEEE TKDE (CCF-A, 中科院一区Top, IF:10.4) &nbsp;</i></b>
            <a href="https://ieeexplore.ieee.org/abstract/document/11206540"><em>[paper]</em></a>
            <a href="https://github.com/THPengL/NeuCGC"><em>[code]</em></a>
        </div>
    </div>
</div>


Awards
--------
- National Scholarship 2025

Service
--------
- Reviewer for CVPR 2026,ICME 2025-2026, 
- Reviewer for IEEE TKDE

Experience
--------------
<div class="experience-container">
  <div class="experience-card">
      <img src="images/SJTU.png" alt="SJTU logo" class="experience-logo">
      <div class="experience-info">
          <strong>Shanghai Jiao Tong University</strong><br>
          July 2024 - June 2025<br>
          Research Intern at <a href="https://www.mvig.org/index.html"><em>MVIG</em></a> Lab
      </div>
  </div>

<div class="experience-card">
    <img src="images/SJTU.png" alt="SJTU logo" class="experience-logo">
    <div class="experience-info">
        <strong>Shanghai Jiao Tong University</strong><br>
        Sep 2022 - July 2026<br>
        B.E at <a href="https://www.mvig.org/index.html"><em>MVIG</em></a> Lab
    </div>
</div>

  <div class="experience-card">
      <img src="images/XDU.png" alt="Xi'dian logo" class="experience-logo">
      <div class="experience-info">
          <strong>Shantou University</strong><br>
          Sep 2022 - July 2026<br>
          Rank 4/174, <b>National Scholarship</b><br>
          B.E at <a href="https://sai.xidian.edu.cn"><em>SAI</em></a> & RA at <a href="https://web.xidian.edu.cn/mggong/"><em>OMEGA</em></a> Lab
      </div>
  </div>
</div>

