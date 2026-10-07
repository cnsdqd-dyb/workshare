---
layout: post
title: "Hi-Lo Prune: Look at What You'll Lose before Pruning"
date: 2026-06-01
author: "Zixun Sun, Yubo Dong, Hehe Fan, Yi Yang"
description: "CVPR 2026 collaborative research on training-free visual token pruning for multimodal language models."
---

**CVPR 2026 · Collaborative research · Multimodal efficiency**

[Read the paper](https://openaccess.thecvf.com/content/CVPR2026/html/Sun_Hi-Lo_Prune_Look_at_What_Youll_Lose_before_Pruning_with_CVPR_2026_paper.html) · [Project repository](https://github.com/sealost/Hi-Lo_Prune)

## The question

Long visual token sequences make multimodal language models expensive to run. Removing tokens early can reduce computation, but it can also discard useful visual evidence before the model has absorbed it.

## The idea

Hi-Lo Prune follows a three-stage process:

1. **Select:** use a coarse-to-fine process to identify retained tokens and pruning candidates.
2. **Fuse:** transfer information from the candidates to retained tokens through attention before removal.
3. **Prune:** remove candidates at a designated Transformer layer to reduce subsequent computation.

The method requires no additional training. The paper evaluates it on Qwen2-VL, Qwen2.5-VL, and Qwen3-VL across multiple vision-language benchmarks.

## Paper and resources

**Full title:** Hi-Lo Prune: Look at What You'll Lose before Pruning with Hierarchical Token Selection  
**Authors:** Zixun Sun, **Yubo Dong (董玉博)**, Hehe Fan, Yi Yang  
**Publication:** IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), 2026, pp. 31941–31951.

The [CVF paper page](https://openaccess.thecvf.com/content/CVPR2026/html/Sun_Hi-Lo_Prune_Look_at_What_Youll_Lose_before_Pruning_with_CVPR_2026_paper.html) provides the paper, supplementary material, and citation. The [authors' repository](https://github.com/sealost/Hi-Lo_Prune) currently contains a placeholder README; implementation availability should be checked there.
