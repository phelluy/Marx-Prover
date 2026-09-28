# Marx-Prover

Marx-Prover studies how small or heavily quantized language models can collaborate on formal proofs. Can these teams close the gap with larger models under a fixed compute budget?

The project is inspired by [OpenAI's ~10 000-agent Navier–Stokes experiment](https://openai.com/index/navier-stokes-solution/). We want to explore cooperation at a smaller scale.

The central idea is to train agents to build their own working setup for each problem: choose tools, divide tasks, and coordinate their work. Simple problems may need little preparation; harder ones may benefit from more organization.

- [Environment](Agent-environment.md)
- [Evaluation](Evaluation.md)
- [Training](Training.md)
- [Related work](Related-work.md)
- [Research workflow](Research-workflow.md)
