---
title: "(Neurips 2023) Provably Safe Reinforcement Learning with Step-wise Violation Constraints"
collection: publications
permalink: /publication/2010-10-01-paper-title-number-2
excerpt: '*Nuoya Xiong*, Yihan Du, Longbo Huang'
date: 2023-09-28
venue: 'Thirty-seventh Conference on Neural Information Processing Systems'
paperurl: ' '
citation: ' '
---
We investigate a novel safe reinforcement learning problem with step-wise violation constraints. Our problem differs from existing works in that we focus on stricter step-wise violation constraints and do not assume the existence of safe actions, making our formulation more suitable for safety-critical applications that need to ensure safety in all decision steps but may not always possess safe actions, e.g., robot control and autonomous driving.
We propose an efficient algorithm SUCBVI, which guarantees $\widetilde{\mathcal{O}}(\sqrt{ST})$ or gap-dependent $\widetilde{\mathcal{O}}(S/\mathcal{C}_{\mathrm{gap}} + S^2AH^2)$ step-wise violation and $\widetilde{\mathcal{O}}(\sqrt{H^3SAT})$ regret. Lower bounds are provided to validate the optimality in both violation and  regret performance with respect to the number of states $S$ and the total number of steps $T$. 
Moreover, we further study an innovative safe reward-free exploration problem with step-wise violation constraints. For this problem, we design algorithm SRF-UCRL to find a near-optimal safe policy, which achieves nearly state-of-the-art  sample complexity $\widetilde{\mathcal{O}}((\frac{S^2AH^2}{\varepsilon}+\frac{H^4SA}{\varepsilon^2})(\log(\frac{1}{\delta})+S))$, and guarantees $\widetilde{\mathcal{O}}(\sqrt{ST})$ violation during exploration.  Experimental results demonstrate the  superiority of our algorithms in safety performance and corroborate our theoretical results. 

[Download paper here](https://arxiv.org/abs/2302.06064)

