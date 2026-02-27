---
layout: post
title: "🚀 Super Research: Answering Highly Complex Questions with Large Language Models"
hide_title: false
feature-img: assets/img/thumbnails/superresearch-thumbnail.png
thumbnail: assets/img/thumbnails/superresearch-thumbnail.png
author: Yubo Dong
tags: [SuperResearch, LLM, Agent, Graph Reasoning, Benchmark]
---

<div align="center" style="font-size: larger;">
    <a href='#'>Yubo Dong</a><sup>1</sup>, 
    <a href='#'>Nianhao You</a><sup>1</sup>, 
    <a href='#'>Yuxuan Hou</a><sup>1</sup>, 
    <a href='#'>Zixun Sun</a><sup>1</sup>, 
    <a href='#'>Yue Zhang</a><sup>1</sup>, 
    <a href='#'>Liang Zhang</a><sup>2</sup>, 
    <a href='#'>Siyuan Zhao</a><sup>2</sup>, 
    <a href='#'>Yi Lin</a><sup>2, ✉</sup>, 
    <a href='#'>Hehe Fan</a><sup>1, ✉</sup>
</div>
<div align="center" style="font-size: larger;">
    <sup>1</sup>Zhejiang University, <sup>2</sup>Ant Group
</div>
<br>

<style>
    .center-flex {
        display: flex; 
        justify-content: center; 
        align-items: center; 
        gap: 15px; 
    }
    .center-flex img {
        height: auto; 
        width: auto; 
    }
    .highlight-btn {
        background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
        color: white !important;
        padding: 10px 20px;
        border-radius: 8px;
        text-decoration: none;
        font-weight: bold;
        display: inline-block;
        transition: transform 0.2s;
        box-shadow: 0 4px 6px rgba(0,0,0,0.1);
    }
    .highlight-btn:hover {
        transform: translateY(-2px);
        box-shadow: 0 6px 12px rgba(0,0,0,0.15);
    }
</style>

<p class="center-flex">
    <a href='https://cnsdqd-dyb.github.io/Super-Research-Benchmark/' class="highlight-btn" target="_blank">
      🌟 Visit the Official Project Website & Leaderboard
    </a>
</p>

<p class="center-flex">
    <a href='https://arxiv.org/'>
      <img src='https://img.shields.io/badge/Paper-PDF-green?style=for-the-badge&logo=arXiv&logoColor=green' alt='Paper PDF'>
    </a>
    <a href='#'>
      <img src='https://img.shields.io/badge/Code-Repository-yellow?style=for-the-badge&logo=GitHub' alt='Code Repository'>
    </a>
</p>

> <span style="color: #3498db; font-weight: bold;">Super Research</span> introduces a new benchmark for evaluating LLMs on highly complex questions requiring long-horizon planning, massive evidence gathering, and synthesis across heterogeneous sources. It evaluates systems on <span style="color: #e74c3c;">Super Deep Investigation</span> and <span style="color: #e74c3c;">Super Wide Retrieval</span>.

---

<h2 style="text-align:center;">Overview</h2>
{% include aligner.html images="feature-img/data_dist_01.png" column=1 %}

While Large Language Models (LLMs) have demonstrated proficiency in Deep Research or Wide Search, their capacity to solve highly complex questions remains largely unexplored. We introduce **Super Research**, a task for complex autonomous research tasks that integrates:
1. Structured decomposition into a research plan
2. **Super wide** retrieval for diverse perspectives
3. **Super deep** investigation to resolve uncertainties through iterative queries.

To evaluate this capability, we curated a benchmark of **300 expert-written questions** across diverse domains, each requiring up to 100+ retrieval steps and 1,000+ web pages to reconcile conflicting evidence.

---

<h2 style="text-align:center;">Methodology & Graph-Anchored Auditing</h2>

Super Research employs a structured graph-based reasoning approach to handle high-stakes analytics. We present a **graph-anchored auditing protocol** that evaluates Super Research along five dimensions: 
* **Coverage** * **Logical Consistency**
* **Report Utility**
* **Objectivity**
* **Citation Health** (Dominance & Monopolization)


{% include aligner.html images="feature-img/superresearch-pipeline.png" column=1 %}
<br>

<div align="center">
    <a href="https://cnsdqd-dyb.github.io/Super-Research-Benchmark/#leaderboard" style="font-size: 1.2rem; font-weight: bold; color: #2c3e50; text-decoration: underline;">
        👉 Click here to view the full interactive Leaderboard & Case Gallery
    </a>
</div>

---

<div style="background-color:#f8f9fa; color:black; padding:20px 0; margin:0; width:100%; border-radius: 8px;">
  <div style="margin:auto; width:90%; padding:10px;">
    <!-- BibTeX entry -->
    <pre style="background: transparent; border: none;">
@article{superresearch2026,
  title={Super Research: Answering Highly Complex Questions with Large Language Models though Super Deep and Super Wide Research},
  author={Yubo Dong, Nianhao You, Yuxuan Hou, Zixun Sun, Yue Zhang, Liang Zhang, Siyuan Zhao, Yi Lin, Hehe Fan},
  journal={ArXiv},
  year={2026}
}
    </pre>
  </div>

</div>






