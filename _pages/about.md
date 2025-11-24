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

    /* Publication card updated for fixed image layout */
.publication-card {
    display: flex;
    align-items: flex-start;  /* 保持顶部对齐 */
    padding: 16px;
    border: 1.5px solid #ddd;
    border-radius: 8px;
    background: #fff;
    box-sizing: border-box;
    margin-bottom: 20px; 
    transition: transform 0.3s ease, box-shadow 0.3s ease;
    min-height: 130px; /* 移除之前固定的140px，改为更灵活的最小高度 */
}

.publication-card:hover {
    box-shadow: 0 8px 16px rgba(0,0,0,0.1);
}

.publication-card.featured {
    border-color: #f5bba7;
    box-shadow: 0 4px 8px rgba(242, 166, 120, 0.2);
    z-index: 10;
}

.publication-card.featured:hover {
    box-shadow: 0 8px 16px rgba(242, 166, 120, 0.4); 
}

.paper-links a {
    color: #ca6f6f !important;
    text-decoration: none;
}

.paper-links a:hover {
    color: #c71585 !important;
    text-decoration: underline;
}

.author-links a {
    color: #494E52 !important;
    text-decoration: none;
}

.author-links a:hover {
    color: #000000 !important;
    text-decoration: underline;
}

/* Abstract section styles */
.abstract-container {
    background-color: #f5f5f5;
    border-radius: 8px;
    padding: 12px;
    margin-top: 8px;
    display: none;
    position: relative; /* 添加相对定位 */
    z-index: 1; /* 确保在正确层级 */
}

.abstract-content {
    font-size: 13px;
    line-height: 1.5;
}

.abstract-toggle {
    cursor: pointer;
    font-weight: normal;
    display: inline-block;
    font-size: 13px;
}

.abstract-toggle:hover {
    text-decoration: underline;
}

/* Bibtex section styles */
.bibtex-container {
    background-color: #f5f5f5;
    border-radius: 8px;
    padding: 12px;
    margin-top: 8px;
    display: none;
    position: relative; /* 添加相对定位 */
    z-index: 1; /* 确保在正确层级 */
}

.bibtex-content pre {
    font-size: 13px;
    line-height: 1.5;
    font-family: 'Arial Rounded MT Bold', 'Verdana', sans-serif;
    white-space: pre-wrap;
    word-wrap: break-word;
    margin: 0;
    padding: 0;
    overflow-wrap: break-word;
}

/* Image wrapper for lightbox - modified for fixed dimensions */
.image-wrapper {
    width: 200px;        
    height: auto;        /* 改为自动高度 */
    min-height: 120px;   /* 设置最小高度以保持基本比例 */
    margin-right: 20px;
    cursor: pointer;
    border-radius: 6px;
    overflow: hidden;
    flex-shrink: 0;      
    align-self: flex-start; /* 保持与文本顶部对齐 */
    display: flex;
    align-items: center;     /* 垂直居中 */
    justify-content: center; /* 水平居中 */
}

.paper-image {
    width: 100%;
    height: auto;        /* 高度自适应 */
    max-height: 100%;    /* 最大高度不超过容器 */
    object-fit: contain; /* 保持图片完整显示，不裁剪 */
    object-position: center; /* 图片居中显示 */
    transition: transform 0.2s;
    border-radius: 4px;
}

.paper-image:hover {
    transform: scale(1.05);
}

/* Lightbox overlay */
#lightbox-overlay {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: rgba(250, 250, 250, 0.88); /* 浅灰白 + 高透明度 */
    backdrop-filter: blur(4px); /* 可选：毛玻璃效果，更现代 */
    display: none;
    justify-content: center;
    align-items: center;
    z-index: 10000;
}

#lightbox-image {
    max-width: 90%;
    max-height: 90%;
    border: 2px solid #e0e0e0;
    box-shadow: 0 4px 20px rgba(0, 0, 0, 0.12);
    border-radius: 8px; /* 可选圆角 */
}
</style>

<html> 
<head>
    <style>
        @import url('https://fonts.googleapis.com/css2?family=Permanent+Marker&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Fredericka+the+Great&display=swap');
        @import url('https://fonts.googleapis.com/css2?family=Homemade+Apple&display=swap');
        body {
            background-color: #FFFFFF;
            font-family: 'Arial Rounded MT Bold', 'Verdana', sans-serif;
            font-size: 15px;
        }
        .main-heading {
            font-family: 'Permanent Marker', cursive;
            text-align: center;
            color: #ca6f6f;
        }
        div.markdown-body a, a {
            text-decoration: none !important;
            color: #ca6f6f;
            transition: all 0.3s ease;
        }
        div.markdown-body a:hover, a:hover {
            color: #c71585;
            text-decoration: underline;
        }
    </style>
</head>
<body>
<h1 id="introduction" class="main-heading">Hi there <img src="images/Hi.gif" width="40px"> Welcome to my Homepage!</h1>

<p>I am an undergraduate (2022-2026) at Shantou University, focusing on World Model and Multi-modal.</p>

<p>I work at <a href="https://csu-jpg.github.io">JPG@CSU</a> with <a href="https://fingerrec.github.io">Prof. Alex Jinpeng Wang</a>.<br>
Previously I worked at Shantou University with <a href="https://cliu272.github.io">Prof. Cheng Liu</a>.</p>

<h2 id="news">News</h2>
<ul>
    <li><strong>[SMART]</strong> is accepted in IEEE TCSVT &#128293;</li>
    <li><strong>[scRCL]</strong> is accepted in AAAI 2026 &#128293;</li>
    <li><strong>[NeuCGC]</strong> is accepted in IEEE TKDE &#128293;</li>
    <li><strong>[CVNC]</strong> is accepted in ICME 2025 &#128293;</li>
</ul>

<h2 id="publications">Selected Publication</h2>

<div class="publication-card">
    <div class="image-wrapper" onclick="openLightbox('images/TCSVT25.png')">
        <img src="images/TCSVT25.png" alt="SMART" class="paper-image">
    </div>
    <div class="publication-details">
        <span style="color:#ca6f6f; font-weight:500; text-shadow: 0 0 0.8px rgba(202, 111, 111, 0.75);">
        SMART: Semantic Matching Contrastive Learning for Partially View-Aligned Clustering
        </span><br>
        <div class="author-links" style="font-size: 13px">
            <a href="" target="_blank">Liang Peng</a>*, 
            <a href="" target="_blank"><strong>Yixuan Ye</strong></a>*, 
            <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger;,
            <a href="" target="_blank">Hangjun Che</a>,
            <a href="" target="_blank">Fei Wang</a>,
            <a href="" target="_blank">Zhiwen Yu</a>,<br>
            <a href="" target="_blank">Hau-San Wong</a>
        </div>
        <div style="font-size: 13px;">IEEE Transactions on Circuits and Systems for Video Technology (<strong>IEEE TCSVT</strong>)</div>
        <div class="paper-links" style="font-size:13px;">
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'abstract-4')">[Abstract]</a>
            <a href="#">[Paper]</a>
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'Bibtex-4')">[BibTex]</a>
            <a href="https://github.com/THPengL/SMART">[Code]</a>
        </div>
        <div id="abstract-4" class="abstract-container">
            <div class="abstract-content">
                Multi-view clustering has been empirically shown to improve learning performance by leveraging the inherent complementary information across multiple views of data. However, in real-world scenarios, collecting strictly aligned views is challenging, and learning from both aligned and unaligned data becomes a more practical solution. Partially View-aligned Clustering (PVC) aims to learn correspondences between misaligned view samples to better exploit the potential consistency and complementarity across views, including both aligned and unaligned data.
However, most existing PVC methods fail to leverage unaligned data to capture the shared semantics among samples from the same cluster. Moreover, the inherent heterogeneity of multi-view data induces distributional shifts in representations, leading to inaccuracies in establishing meaningful correspondences between cross-view latent features and, consequently, impairing learning effectiveness.
To address these challenges, we propose a <strong>S</strong>emantic <strong>MA</strong>tching cont<strong>R</strong>as<strong>T</strong>ive learning model (SMART) for PVC. The main idea of our approach is to alleviate the influence of cross-view distributional shifts, thereby facilitating semantic matching contrastive learning to fully exploit semantic relationships in both aligned and unaligned data. Specifically, we mitigate view distribution shifts by aligning cross-view covariance matrices, which enables the inference of a semantic graph for all data. Guided by the learned semantic graph, we further exploit semantic consistency across views through semantic matching contrastive learning. 
After the optimization of the above mechanisms, our model smoothly performs semantic matching for different view embeddings instead of the cumbersome view realignment, which enables the learned representations to enjoy richer category-level semantics and stronger robustness.
Extensive experiments on eight benchmark datasets demonstrate that our method consistently outperforms existing approaches on the PVC problem.
            </div>
        </div>
        <div id="Bibtex-4" class="abstract-container">
            <div class="abstract-content">
                None.
            </div>
        </div>
    </div>
</div>

<div class="publication-card">
    <div class="image-wrapper" onclick="openLightbox('images/AAAI26.png')">
        <img src="images/AAAI26.png" alt="scRCL" class="paper-image">
    </div>
    <div class="publication-details">
        <span style="color:#ca6f6f; font-weight:500; text-shadow: 0 0 0.8px rgba(202, 111, 111, 0.75);">
        Refinement Contrastive Learning of Cell-Gene Associations for Unsupervised Cell Type Identification
        </span><br>
        <div class="author-links" style="font-size: 13px">
            <a href="" target="_blank">Liang Peng</a>*, 
            <a href="" target="_blank">Haopeng Liu</a>*,
            <a href="" target="_blank"><strong>Yixuan Ye</strong></a>*, 
            <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger;,
            <a href="" target="_blank">Wenjun Shen</a>,
            <a href="" target="_blank">Si Wu</a>,
            <a href="" target="_blank">Hau-San Wong</a>
        </div>
        <div style="font-size: 13px;">The 40th Annual AAAI Conference on Artificial Intelligence (<strong>AAAI 2026</strong>)</div>
        <div class="paper-links" style="font-size:13px;">
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'abstract-3')">[Abstract]</a>
            <a href="#">[Paper]</a>
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'Bibtex-3')">[BibTex]</a>
            <a href="https://github.com/THPengL/scRCL">[Code]</a>
        </div>
        <div id="abstract-3" class="abstract-container">
            <div class="abstract-content">
                Unsupervised cell type identification is crucial for uncovering and characterizing heterogeneous populations in single cell omics studies. Although a range of clustering methods have been developed, most focus exclusively on intrinsic cellular structure and ignore the pivotal role of cell-gene associations, which limits their ability to distinguish closely related cell types. To this end, we propose a Refinement Contrastive Learning framework (<strong>scRCL</strong>) that explicitly incorporates cell-gene interactions to derive more informative representations. 
Specifically, we introduce two contrastive distribution alignment components that reveal reliable intrinsic cellular structures by effectively exploiting cell-cell structural relationships.
Additionally, we develop a refinement module that integrates gene-correlation structure learning to enhance cell embeddings by capturing underlying cell-gene associations. This module strengthens connections between cells and their associated genes, refining the representation learning to exploiting biologically meaningful relationships.
Extensive experiments on several single‑cell RNA‑seq and spatial transcriptomics benchmark datasets demonstrate that our method consistently outperforms state-of-the-art baselines in cell-type identification accuracy. Moreover, downstream biological analyses confirm that the recovered cell populations exhibit coherent gene‑expression signatures, further validating the biological relevance of our approach.
            </div>
        </div>
        <div id="Bibtex-3" class="abstract-container">
            <div class="abstract-content">
                None.
            </div>
        </div>
    </div>
</div>

<div class="publication-card">
    <div class="image-wrapper" onclick="openLightbox('images/TKDE25.png')">
        <img src="images/TKDE25.png" alt="NeuCGC" class="paper-image">
    </div>
    <div class="publication-details">
        <span style="color:#ca6f6f; font-weight:500; text-shadow: 0 0 0.8px rgba(202, 111, 111, 0.75);">
        Trustworthy Neighborhoods Mining: Homophily-Aware Neutral Contrastive Learning for Graph Clustering
        </span><br>
        <div class="author-links" style="font-size: 13px">
            <a href="" target="_blank">Liang Peng</a>, 
            <a href="" target="_blank"><strong>Yixuan Ye</strong></a>, 
            <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger;,
            <a href="" target="_blank">Hangjun Che</a>,
            <a href="" target="_blank">Man-Fai Leung</a>,
            <a href="" target="_blank">Si Wu</a>,
            <a href="" target="_blank">Hau-San Wong</a>
        </div>
        <div style="font-size: 13px;">IEEE Transactions on Knowledge and Data Engineering (<strong>IEEE TKDE</strong>)</div>
        <div class="paper-links" style="font-size:13px;">
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'abstract-2')">[Abstract]</a>
            <a href="https://ieeexplore.ieee.org/abstract/document/11206540">[Paper]</a>
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'Bibtex-2')">[BibTex]</a>
            <a href="https://github.com/THPengL/NeuCGC">[Code]</a>
        </div>
        <div id="abstract-2" class="abstract-container">
            <div class="abstract-content">
                Recently, neighbor-based contrastive learning has been introduced to effectively exploit neighborhood information for clustering. However, these methods rely on the homophily assumption—that connected nodes share similar class labels and should therefore be close in feature space—which fails to account for the varying homophily levels in real-world graphs.
As a result, applying contrastive learning to low-homophily graphs may lead to indistinguishable node representations due to unreliable neighborhood information, making it challenging to identify trustworthy neighborhoods with varying homophily levels in graph clustering.
To tackle this, we introduce a novel neighborhood Neutral Contrastive Graph Clustering method NeuCGC that extends traditional contrastive learning by incorporating neutral pairs—node pairs treated as weighted positive pairs, rather than strictly positive or negative. These neutral pairs are dynamically adjusted based on the graph’s homophily level, enabling a more flexible and robust learning process. 
Leveraging neutral pairs in contrastive learning, our method incorporates two key components: 1) an adaptive contrastive neighborhood distribution alignment that adjusts based on the homophily level of the given attribute graph, ensuring effective alignment of neighborhood distributions, and 2) a contrastive neighborhood node feature consistency learning mechanism that leverages reliable neighborhood information from high-confidence graphs to learn robust node representations, mitigating the adverse effects of varying homophily levels and effectively exploiting highly trustworthy neighborhood information.
Experimental results demonstrate the effectiveness and robustness of our approach, outperforming other state-of-the-art graph clustering methods.
            </div>
        </div>
        <div id="Bibtex-2" class="bibtex-container">
            <div class="bibtex-content">
                <pre>@ARTICLE{11206540,
                author={Peng, Liang and Ye, Yixuan and Liu, Cheng and Che, Hangjun and Leung, Man-Fai and Wu, Si and Wong, Hau-San},
                journal={IEEE Transactions on Knowledge and Data Engineering}, 
                title={Trustworthy Neighborhoods Mining: Homophily-Aware Neutral Contrastive Learning for Graph Clustering}, 
                year={2025},
                pages={1-15},
                keywords={Contrastive learning;Reliability;Computer science;Representation learning;Estimation;Silicon;Semantics;Robustness;Nickel;Learning systems;Contrastive Graph Clustering;Graph Homophily},
                doi={10.1109/TKDE.2025.3622998}}</pre>
            </div>
        </div>
    </div>
</div>

<div class="publication-card">
    <div class="image-wrapper" onclick="openLightbox('images/ICME2025.jpg')">
        <img src="images/ICME2025.png" alt="CVNC" class="paper-image" style="object-position: center 10%;">
    </div>
    <div class="publication-details">
        <span style="color:#ca6f6f; font-weight:500; text-shadow: 0 0 0.8px rgba(202, 111, 111, 0.75);">
        Cross-View Neighborhood Contrastive Multi-View Clustering with View Mixup Feature Learning
        </span><br>
        <div class="author-links" style="font-size: 13px">
            <a href="" target="_blank"><strong>Yixuan Ye</strong></a>, 
            <a href="" target="_blank">Yang Zhang</a>,
            <a href="" target="_blank">Liang Peng</a>,
            <a href="https://cliu272.github.io" target="_blank">Cheng Liu</a>&dagger;,
            <a href="" target="_blank">Rui Li</a>,
            <a href="" target="_blank">Si Wu</a>,
            <a href="" target="_blank">Hau-San Wong</a>
        </div>
        <div style="font-size: 13px;">The 26th IEEE International Conference on Multimedia and Expo (<strong>ICME 2025</strong>)</div>
        <div class="paper-links" style="font-size:13px;">
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'abstract-1')">[Abstract]</a>
            <a href="https://ieeexplore.ieee.org/document/11209498">[Paper]</a>
            <a href="#" class="abstract-toggle" onclick="toggleAbstract(event, 'Bibtex-1')">[BibTex]</a>
            <a href="https://github.com/EasonTuT/ICME2025-CVNC">[Code]</a>
        </div>
        <div id="abstract-1" class="abstract-container">
            <div class="abstract-content">
                Multi-view clustering (MVC) has shown that leveraging both consistency and complementary information across views enhances clustering performance. However, most existing methods focus on aligning features into the same dimension, often neglecting cross-view heterogeneity and introducing discrepancies. To address this, we propose a novel multi-view clustering framework that combines cross-view neighborhood contrastive learning with a cross-attention view-mixup feature learning mechanism. Specifically, the cross-attention view-mixup module learns view-invariant feature representations by capturing complementary and consistent information, while the neighborhood contrastive learning module uncovers semantic structures across views based on the learned mixup features. By implicitly performing feature mixup across views and effectively integrating cross-view neighborhood contrastive learning, our method alleviates cross-view discrepancies and enables more effective integration of complementary and consistent information, ultimately enhancing clustering performance. Experiments conducted on several real datasets demonstrate the effectiveness of our proposed method in comparision with several representative MVC approaches.
            </div>
        </div>
        <div id="Bibtex-1" class="bibtex-container">
          <div class="bibtex-content">
              <pre>@INPROCEEDINGS{11209498,
                author={Ye, Yixuan and Zhang, Yang and Peng, Liang and Li, Rui and Liu, Cheng and Wu, Si and Wong, Hau-San},
                booktitle={2025 IEEE International Conference on Multimedia and Expo (ICME)}, 
                title={Cross-View Neighborhood Contrastive Multi-View Clustering with View Mixup Feature Learning}, 
                year={2025},
                pages={1-6},
                keywords={Representation learning;Semantics;Contrastive learning;Benchmark testing;Multi-view clustering;Cross-view contrastive learning;Cross-attention},
                doi={10.1109/ICME59968.2025.11209498}}</pre>
          </div>
        </div>
    </div>
</div>

<h2 id="awards">Awards</h2>
<ul>
    <li>National Scholarship 2025</li>
</ul>

<h2 id="service">Service</h2>
<ul>
    <li>Reviewer for ICME 2025-2026</li>
    <li>Reviewer for IEEE TKDE</li>
</ul>

<h2 id="experience">Experience</h2>
<div class="experience-container">
  <div class="experience-card">
      <img src="images/CSU.png" alt="CSU logo" class="experience-logo">
      <div class="experience-info">
          <strong>Central South University</strong><br>
          July 2026 - June 2029<br>
          M.S at <a href="https://csu-jpg.github.io"><em>JPG</em></a>
      </div>
  </div>

  <div class="experience-card">
      <img src="images/STU.png" alt="STU logo" class="experience-logo">
      <div class="experience-info">
          <strong>Shantou University</strong><br>
          Sep 2022 - July 2026<br>
          B.E Rank 1/79
      </div>
  </div>
</div>

<!-- Lightbox Overlay -->
<div id="lightbox-overlay" onclick="closeLightbox()">
    <img id="lightbox-image" src="" alt="Enlarged view">
</div>

<script>
function toggleAbstract(event, abstractId) {
    event.preventDefault();
    const container = document.getElementById(abstractId);
    if (container.style.display === 'block') {
        container.style.display = 'none';
    } else {
        container.style.display = 'block';
    }
}

function openLightbox(src) {
    const overlay = document.getElementById('lightbox-overlay');
    const img = document.getElementById('lightbox-image');
    img.src = src;
    overlay.style.display = 'flex';
    document.body.style.overflow = 'hidden';
}

function closeLightbox() {
    document.getElementById('lightbox-overlay').style.display = 'none';
    document.body.style.overflow = '';
}

document.addEventListener('keydown', (e) => {
    if (e.key === 'Escape') closeLightbox();
});
</script>

</body>
</html>
