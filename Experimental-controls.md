# Experimental controls

[Introduction](Introduction.md)

Measure whether copies of the fine-tuned model benefit from organizing and interacting under a fixed total budget.

## Compare the same checkpoint

Evaluate each base, SFT, and SFT+RL checkpoint in the conditions below. Within each comparison, keep model weights, proof tools, libraries, retrieval access, and total budget constant. Each agent can both prove and coordinate.

| Condition | Behavior |
| --- | --- |
| Solo | One instance with the full budget and scripting tools. |
| Independent parallel | Copies work without messages or shared results. |
| Self-organized swarm | Copies choose how to cooperate and build their tools. |

Compare the swarm's gain over independent parallel runs before and after training. Proving and coordination improve jointly; this measures the benefit of interaction at each checkpoint without assuming they can be fully separated.

## Useful collaboration

Randomly disable messages, shared artifacts, agents to see performance impact.

**WIP:** fixed protocols; stronger solo search baselines; ablation sampling and repeat count; matching training costs against solo fine-tuning.
