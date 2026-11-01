# Precision

Each model has one page for what it computes in and what each rounding costs. The method is shared.

This downstream branch retains the v0.1.0 initial expert ranking. CPU and GPU expert paths
round differently, so changing the ranking can change logits even with identical weights.
The upstream measurements describe their recorded profiles rather than this retained ranking;
qualify the engine and ranking together for deployment.

- [Qwen3.8-Flash-Next](qwen38-flash-next.md): stages, prefill, the measured costs, drafting and the lossy flags.
- [DeepSeek-V4.1-Flash](deepseek41.md): stages, the prompt path, verify windows and quality against its BF16 reference.
- [How quality is measured](quality.md): the gate, the BF16 references, greedy identity and reproduction commands.
