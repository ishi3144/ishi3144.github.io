---
layout: page
title: Differential Privacy in Best-of-n Alignment
description: Calibrated-noise mechanisms for differentially private inference-time alignment of LLMs.
img:
importance: 1
category: research
related_publications: true
---

With [Prof. Sayak Ray Chowdhury](https://sayakraychowdhury.github.io/), IIT Kanpur — Jan 2026 to present.

Best-of-N sampling is a widely used inference-time alignment strategy for large language models, but it suffers from reward hacking and provides no privacy protection for the human preference data used to train the reward model. We designed two calibrated-noise mechanisms that add differential privacy to Best-of-N selection:

- **PrivBoN.** Gumbel noise at an appropriate scale simultaneously provides ε-differential privacy and implements KL-regularized alignment.
- **PrivITP** (Private Inference-Time Pessimism). Combines χ²-regularized rejection sampling with a two-phase Gaussian mechanism, achieving (ε, δ)-DP with a privacy cost independent of the number of responses *n*.

Both methods are scaling-monotonic. We validated the privacy–utility tradeoff on the Anthropic HH dataset, matching theoretical bounds. Preprint available at [arXiv:2608.26324](https://arxiv.org/abs/2608.26324).
