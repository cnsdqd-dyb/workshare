---
layout: post
title: "🌍 VillagerAgent: A Graph-Based Multi-Agent Framework for Coordinating Complex Task Dependencies in Minecraft 🏰"
hide_title: false
feature-img: assets/img/VillagerAgent/VillagerBench.png
thumbnail: assets/img/VillagerAgent/VillagerBench.png
author: Yubo Dong
tags: [VillagerAgent, Multi-Agent, ]
---
<div align="center">Yubo Dong, Xukun Zhu, Zhengzhe Pan, Linchao Zhu, Yi Yang<br>ReLER Lab, Zhejiang University</div>
<br>

<style>
    .center-flex {
        display: flex; /* 设置为Flexbox容器 */
        justify-content: center; /* 水平居中 */
        align-items: center; /* 垂直居中 */
        gap: 0px; /* 设置元素之间的间距 */
        
    }
    .center-flex img {
        height: auto; /* 保持图片的宽高比 */
        width: auto; /* 调整图片宽度，从而调整按钮大小 */
    }
</style>

<p class="center-flex">
    <a href='https://arxiv.org/abs/2406.05720'>
      <img src='https://img.shields.io/badge/Paper-PDF-green?style=for-the-badge&logo=arXiv&logoColor=green' alt='Paper PDF'>
    </a>
    <a href='https://github.com/cnsdqd-dyb/VillagerAgent-Minecraft-multiagent-framework'>
      <img src='https://img.shields.io/badge/Code-Repository-yellow?style=for-the-badge&logo=GitHub' alt='Code Repository'>
    </a>
</p>

> <span style="color: green;">VillagerBench</span> is a multi-agent cooperation evaluate platform in Minecraft, support more than <span style="color: orange;">40 APIs</span> for minecraft agents to interact with the world and cooperate with each other, we have designed three scenarios: <span style="color: purple;">construction building</span> tasks, <span style="color: purple;">farm to table cooking</span> tasks and <span style="color: purple;">escape the room</span> challenge.
{% include aligner.html images="VillagerAgent/01.gif" column=1 %}

---


<h2 style="text-align:center;">Abstract</h2>
In this paper, we aim to evaluate multi-agent systems against complex dependencies, including spatial, causal, and temporal constraints. First, we construct a new benchmark, named **VillagerBench**, within the Minecraft environment. VillagerBench comprises diverse tasks crafted to test various aspects of multi-agent collaboration, from workload distribution to dynamic adaptation and synchronized task execution. Second, we introduce a Directed Acyclic Graph Multi-Agent Framework (**VillagerAgent**) to resolve complex inter-agent dependencies and enhance collaborative efficiency. This solution incorporates a task decomposer that creates a directed acyclic graph (DAG) for structured task management, an agent controller for task distribution, and a state manager for tracking environmental and agent data.

Our empirical evaluation on VillagerBench demonstrates that VillagerAgent outperforms the existing AgentVerse model, reducing hallucinations and improving task decomposition efficacy. The results underscore VillagerAgent's potential in advancing multi-agent collaboration, offering a scalable and generalizable solution in dynamic environments.


---

<h2 style="text-align:center;">BenchMark</h2>
{% include aligner.html images="VillagerAgent/benchmark.png,VillagerAgent/radar.png" %}
- **Introduce a new multi-agent benchmark focusing on complex dependencies in Minecraft.**
  As we discussed  above (see our responses to Q1), our work distinguishes itself by focusing on complex multi-agent interactions within the Minecraft environment. This is a  underexplored area compared to the prevalent single-agent or task-specific benchmarks. VillagerBench offers a fresh perspective for evaluating multi-agent teamwork in environments that are both complex and dynamic.



---

<h2 style="text-align:center;">VillagerAgent Framework</h2>
{% include aligner.html images="VillagerAgent/framework.png" column=1 %}
- **Introduce a new DAG-based multi-agent framework to tackle complex dependencies in multi-agent collaborations.** 
  Our VillagerAgent framework consists of a Task Decomposer that breaks down tasks into graph nodes, an Agent Controller responsible for assigning agents to nodes, and a State Manager in charge of managing experience and state information. Our approach enables the decomposition of tasks into sub-task nodes, differing from previous methods that fix agents in specific locations or execute steps simultaneously according to rules. Our DAG structure accurately describes the sequential and parallel order and dependencies of different sub-tasks, allowing agents to precisely execute synchronous and sequential sub-tasks, thereby enhancing the degree of multi-agent cooperation.

---
<h2 style="text-align:center;">Other Demo</h2>
{% include aligner.html images="VillagerAgent/villagerbench-2.gif,VillagerAgent/villagerbench-3.gif,VillagerAgent/villagerbench-4.gif" column=3 %}
{% include aligner.html images="VillagerAgent/villagerbench-5.gif,VillagerAgent/villagerbench-6.gif,VillagerAgent/villagerbench-7.gif" column=3 %}
{% include aligner.html images="VillagerAgent/villagerbench-8.gif,VillagerAgent/villagerbench-9.gif,VillagerAgent/villagerbench-10.gif" column=3 %}

---

<h2 style="text-align:center;">Demo in Overcooked Benchmark</h2>

{% include aligner.html images="VillagerAgent/layouts.gif" %}



{% include aligner.html images="VillagerAgent/o0.gif,VillagerAgent/o1.gif,VillagerAgent/o2.gif" column=3 %}

<div style="display: flex; width: 100%;">
  <div style="text-align: left; flex-grow: 1; padding-right: 10px;">Cramped Room</div>
  <div style="text-align: center; flex-grow: 1;">Asymmetric Advantages</div>
  <div style="text-align: right; flex-grow: 1; padding-left: 10px;">Coordination Ring</div>
</div>

---

<div style="background-color:#f0f0f0; color:black; padding:20px 0; margin:0; width:100%;">
  <div style="margin:auto; width:90%; padding:10px;">
    <!-- BibTeX entry -->
    <pre>
@misc{dong2024villageragent,
  title={VillagerAgent: A Graph-Based Multi-Agent Framework for Coordinating Complex Task Dependencies in Minecraft},
  author={Yubo Dong and Xukun Zhu and Zhengzhe Pan and Linchao Zhu and Yi Yang},
  year={2024},
  eprint={2406.05720},
  archivePrefix={arXiv},
  url={https://arxiv.org/abs/2406.05720}
}
    </pre>
  </div>
</div>