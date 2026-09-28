# Learning signal

[Introduction](Introduction.md)

## Budget and reward

Proposed starting point: maximize verified proof success under a hard episode budget. A complete proof earns 1; failure or budget exhaustion earns 0. The external verifier checks the original statement and allowed assumptions.

Setup, messages, proof search, and tool execution consume the budget. Give agents access to the remaining budget so the swarm can adapt. A hard cap makes organization compete with proving for resources.

**WIP:** budget units and limits. Token caps are useful within one model; comparisons across sizes and quantizations need compute accounting. A soft cost penalty is a separate experiment.

## Credit assignment

All agents' experience updates the same model. Credit assignment determines how their actions contribute to that shared update. Compare:

| Method | Learning signal |
| --- | --- |
| Shared reward / MAGRPO | Relative returns from sampled team trajectories. |
| Centralized critic | Value estimates using the joint history during training. |
| COMA-style credit | Estimate an action's contribution by varying it while holding other agents' actions fixed. |

These [candidate methods](Related-work.md) need adaptation to shared weights. A centralized critic would estimate training signals only; execution remains a swarm of copies. Counterfactual estimates need validation. Graph-GRPO offers a reference for edge-level credit.

**WIP:** credit unit (message, script, organizational decision, or agent); treatment of delayed contributions; cost of counterfactual estimates.
