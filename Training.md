# Training

[Introduction](Introduction.md)

Train agents to build a harness for each problem, choosing roles, tools, task decomposition, and communication.

## Data and SFT

Run a larger teacher, e.g. [DeepSeek V4.1 Flash](https://api-docs.deepseek.com/news/news260910/), as collaborating agents in the minimal environment.

Record how the agents organize, write scripts, exchange messages, and complete proofs. Keep verified examples across difficulty levels, including solutions needing almost no setup. Train each student from its agent's observations.

**SFT supplies a few collaborative examples to warm up RL.**

## RL

Give agents a problem and a budget. They organize, attempt a proof, and adjust their approach. Use the team's proof success to train organization decisions; setup, messages, and proving share the budget.

Easy problems should need almost no initialization. Harder problems may justify more setup when it improves success. This tradeoff should emerge from training.

[MAGRPO and centralized-critic methods](Related-work.md) provide candidate learning algorithms.
