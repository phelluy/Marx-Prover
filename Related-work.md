# Related work

[Introduction](Introduction.md)

## Training:

| Paper | Relevance |
| --- | --- |
| Liu et al., [LLM Collaboration with Multi-Agent Reinforcement Learning](https://ojs.aaai.org/index.php/AAAI/article/view/40487), AAAI 2026 | MAGRPO: multi-agent, multi-turn updates using a shared team reward. Candidate baseline. |
| Liu et al., [Learning Decentralized LLM Collaboration with Multi-Agent Actor Critic](https://arxiv.org/abs/2601.21972), [ICML 2026](https://www.ccs.neu.edu/home/camato/publications.html) | A centralized critic improves learning on long-horizon, sparse-reward tasks; execution stays decentralized. Relevant to delayed proof rewards. |
| Park et al., [MAPoRL](https://aclanthology.org/2025.acl-long.1459/), ACL 2025 | Joint RL improves LLM collaboration through verifier rewards + discussion incentives. Useful comparison; its discussion protocol is predefined. |

Our question: can these learning methods also train agents to construct the organization itself?

## Evaluation: case study

Paglieri et al., [A Case Study on Emergent Cheating and Whistleblowing in Autonomous Research Swarms](https://arxiv.org/abs/2609.04170), 2026 preprint. An evaluation exploit spreads among 100 theorem-proving agents; others attempt to expose it. Implication: verify shared proofs independently. This studies swarm behavior, not training.
