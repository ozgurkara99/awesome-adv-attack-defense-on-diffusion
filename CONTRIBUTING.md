# Contributing

Thanks for helping keep this list accurate and up to date! 🎉

## What belongs here

This list covers **adversarial attacks and defenses for diffusion models** across image, video, and 3D:

- **Attacks (protective cloaks / immunization)** — perturbations applied to content so that a diffusion pipeline (personalization, style mimicry, editing, inpainting, face swap, I2V, talking-head, V2V, 3D editing, …) fails on it.
- **Defenses** — purification and counter-attacks against cloaks, concept unlearning, prompt moderation, protective backdoors, and red-teaming of protections.
- **Benchmarks, datasets, and evaluation studies** dedicated to the above.

Out of scope: general adversarial robustness of classifiers, watermarking/detection-only work (unless it directly interacts with diffusion-based editing), and jailbreaks of language models.

**Inclusion criteria:** peer-reviewed publication, or an arXiv preprint with a working implementation / clear technical contribution. When in doubt, open an issue and ask!

## How to add a paper

1. Find the right section: **modality → attacks/defenses → generative task** (see the taxonomy at the top of the README).
2. Add a row to the task's table, keeping rows **chronological** (by first public release):

   ```markdown
   | **MethodName** | Venue 20XX | One-sentence TL;DR of what it does and why it matters. | [📄&nbsp;Paper](https://arxiv.org/abs/XXXX.XXXXX) · [💻&nbsp;Code](https://github.com/...) |
   ```

3. If you can, also add the paper to the modality's collapsible **evaluation matrix** (evaluation sources, target models, and IA/FA/TR/RB coverage — see the legend under each matrix).
4. Link only the **official** code repository. Use `—` in the Links column if nothing is public yet.
5. One paper per pull request is easiest to review, but batch PRs are welcome too.

## Fixing mistakes

Wrong venue, dead link, misattributed code repo, or an unfair TL;DR? Please open an issue or PR — corrections are just as valuable as additions.

## Style notes

- Keep TL;DRs to a single sentence, neutral in tone, and focused on the *mechanism* ("what does it do that its predecessors didn't?").
- Use non-breaking spaces in link labels (`[📄&nbsp;Paper]`) so they don't wrap.
- Venue format: `CVPR 2025`, `ICLR 2026`, `arXiv 2025`, `IEEE TIFS 2025`, `ACM MM 2024`, `USENIX Security 2023`.
