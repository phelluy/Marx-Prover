# Evaluation

[Introduction](Introduction.md)

**Benchmark:** PutnamBench. [NEAR reports full coverage](https://github.com/nearai/putnambench-deepseek) after retries + two statement corrections. Despite large-model saturation, measure how collaboration closes the small-model gap. Direct comparisons use Lean; Rocq needs equivalent formalizations. Exclude evaluation problems from SFT/RL.

**Models:** small LLMs vs heavily quantized medium LLMs, e.g. [ternary Qwen3.8-27B / Bonsai 2](https://huggingface.co/prism-ml/Ternary-Bonsai-2-27B-gguf), plus an unquantized baseline.

**Comparisons:** solo / independent parallel / fixed organization / learned organization; base / SFT / SFT+RL.

**Metrics:**

- Checked proofs vs budget; elapsed time and gap to a large-model baseline.
- Cumulative IN/OUT tokens, including setup + messages; GPU-time and VRAM across models/precisions.
- Setup cost vs problem difficulty: does organization pay for itself?
- Coordination effort (agent labels + logs), repeated work (post-run analysis), reused results, communication connectivity.

Verify proofs independently against frozen statements/assumptions; [exploits can spread](Related-work.md).
