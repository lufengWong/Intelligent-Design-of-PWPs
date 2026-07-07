# Ablation and comparison experiments

Supplementary results for the ablation and comparison experiments of the paper.
All quantitative results are averaged over **ten independent runs** with different
random seeds; figures are provided as vector PDF (journal-ready) and 600 dpi PNG.
The ten cases (Cases 1–10) span design scopes of 25–250 PWP segments (paper Table 2).

## Baseline comparison
- `figures/Fig_comparison_waste.{pdf,png}` — material waste of the proposed Inner
  EA versus the FFD and BFD heuristics across the ten cases.
- `figures/Fig_comparison_time.{pdf,png}` — computation time (log scale).
- `tables/comparison_FFD_BFD_results.xlsx` — per-run data and summary.

## Ablation experiments
- **Combination box** — `figures/Fig_ablation_box.*`,
  `tables/ablation_combination_box.xlsx`.
- **Baseline-wise gene pool** (first-stage Outer EA) —
  `figures/fig15_baseline_wise_pool.*` (number of PWP segments, w/o vs proposed),
  `tables/ablation_baseline_wise_gene_pool.xlsx`.
- **Public gene pool** (second-stage EA) —
  `figures/fig_public_pool_ablation.*` (spare standard panels, w/o vs proposed),
  `tables/ablation_public_gene_pool_{raw,summary,wilcoxon}.csv`.
- **Heuristic-seeded initialization** — `figures/Fig_ablation_seeding.*`,
  `tables/ablation_heuristic_seeding.xlsx`.

## Sensitivity analysis
- `figures/Fig_sensitivity_stage1.{pdf,png}` — first-stage EA hyperparameters
  (population size, generations, crossover/mutation probabilities, etc.).
- `figures/Fig_sensitivity_stage2.{pdf,png}` — second-stage EA hyperparameters.
- `tables/sensitivity_analysis.xlsx` — one-factor-at-a-time results.

## Notes
- "w/o …" denotes the ablated variant; "proposed" the full method.
- The public gene pool table reports the raw 200 runs (10 cases × 2 variants × 10
  seeds), the per-instance mean ± std summary, and the paired Wilcoxon signed-rank
  tests.
- Statistical significance throughout uses the paired Wilcoxon signed-rank test,
  p < 0.05.
