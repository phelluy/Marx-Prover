# Related work

[Introduction](Introduction.md)

## Training and reward

| Paper | Relevance |
| --- | --- |
| Liu et al., [LLM Collaboration with Multi-Agent Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/40487), AAAI 2026 | MAGRPO: multi-agent, multi-turn updates using a shared team reward. Candidate baseline. |
| Liu et al., [Learning Decentralized LLM Collaboration with Multi-Agent Actor Critic](https://arxiv.org/abs/2601.21972), [ICML 2026](https://www.ccs.neu.edu/home/camato/publications.html) | A centralized critic improves learning on long-horizon, sparse-reward tasks; execution stays decentralized. Relevant to delayed proof rewards. |
| Park et al., [MAPoRL](https://aclanthology.org/2025.acl-long.1459/), ACL 2025 | Joint RL improves LLM collaboration through verifier rewards + discussion incentives. Useful comparison; its discussion protocol is predefined. |
| Foerster et al., [COMA](https://ojs.aaai.org/index.php/AAAI/article/view/11794), AAAI 2018 | Counterfactual credit with a centralized critic. Studied in StarCraft; adaptation to LLM actions remains open. |
| Jiang et al., [Prioritized Level Replay](https://proceedings.mlr.press/v139/jiang21b.html), ICML 2021 | Adaptive replay of training environments. A curriculum reference, not a theorem-proving method. |

## Learning organization

| Work | Organizational choices |
| --- | --- |
| [DyLAN](https://arxiv.org/abs/2310.02170), COLM 2024 | Selects agents and adapts communication during task solving. |
| [GPTSwarm](https://proceedings.mlr.press/v235/zhuge24a.html), ICML 2024 | Optimizes prompts and connectivity in computational graphs. |
| [MasRouter](https://aclanthology.org/2025.acl-long.757/), ACL 2025 | Learns collaboration mode, roles, and model routing. |
| [Graph-GRPO](https://aclanthology.org/2026.findings-acl.1010/), Findings of ACL 2026 | Learns communication edges using relative graph performance. |
| [Guided Topology Diffusion](https://aclanthology.org/2026.acl-long.1764/), ACL 2026 | Generates task-conditioned communication graphs. |


## Evaluation: case study

Paglieri et al., [A Case Study on Emergent Cheating and Whistleblowing in Autonomous Research Swarms](https://arxiv.org/abs/2609.04170), 2026 preprint. An evaluation exploit spreads among 100 theorem-proving agents; others attempt to expose it. Implication: verify shared proofs independently. This studies swarm behavior, not training.
