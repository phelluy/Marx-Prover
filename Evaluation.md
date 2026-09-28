# Evaluation

[Introduction](Introduction.md)

**Benchmark:** PutnamBench. [NEAR reports full coverage](https://github.com/nearai/putnambench-deepseek) after retries + two statement corrections. Despite large-model saturation, measure how collaboration closes the small-model gap. Direct comparisons use Lean; Rocq needs equivalent formalizations.

**Models:** small LLMs vs heavily quantized medium LLMs, e.g. [ternary Qwen3.8-27B / Bonsai 2](https://huggingface.co/prism-ml/Ternary-Bonsai-2-27B-gguf), plus an unquantized baseline. Each swarm consists of copies of one checkpoint.

Compare base, SFT, and SFT+RL checkpoints using the [organization baselines and controls](Experimental-controls.md). Match inference budgets; report training and teacher-data costs separately.

**Metrics:**

- Checked proofs vs budget; elapsed time and gap to a large-model baseline.
- Cumulative IN/OUT tokens, including setup + messages; GPU-time and VRAM across models/precisions.
- Setup cost vs problem difficulty: does organization pay for itself?
- Coordination effort (agent labels + logs), repeated work (post-run analysis), reused results, communication connectivity.
- Change in success when contributions are removed, using controlled reruns.

## Generalization

**WIP:** How to test whether the swarm's self-organization transfers across proof problems and budgets?

**WIP:** Difficulty definition; transfer budgets; model sizes and quantization levels. Track known pretraining exposure separately from SFT/RL exclusions.

Verify proofs independently against frozen statements/assumptions; [exploits can spread](Related-work.md).
