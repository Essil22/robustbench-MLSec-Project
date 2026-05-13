# Final Results Table

This table summarizes clean accuracy and robust accuracy under different ℓ∞ perturbation strengths (AutoAttack evaluation).

---

## Main Results

| Model | Clean | 1/255 | 4/255 | 8/255 | 12/255 | 16/255 |
|---|---|---|---|---|---|---|
| Rebuffi2021Fixing_70_16_cutmix_extra | 96% | 96% | 84% | 58% | 46% | ~33% |
| Carmon2019Unlabeled | 92% | 90% | 72% | 52% | 40% | 20% |
| Wu2020Adversarial | 88% | 84% | 70% | 50% | 36% | 18% |
| Rice2020Overfitting | 86% | 84% | 76% | 52% | 32% | 14% |
| Engstrom2019Robustness | 90% | 86% | 76% | 48% | 24% | 12% |

---

## Key Observation

- Robust accuracy decreases as epsilon increases for all models.
- Rankings are not fully stable across different perturbation strengths.
- Rebuffi2021Fixing_70_16_cutmix_extra consistently performs best across all settings.
