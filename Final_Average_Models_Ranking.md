# Final Model Ranking (Average Robust Accuracy)

Models are ranked based on the average robust accuracy across all epsilon values (1/255 → 16/255).

---

## Average Ranking

| Rank | Model | Average Robust Accuracy |
|---|---|---|
| 1 | Rebuffi2021Fixing_70_16_cutmix_extra | ~65.4% |
| 2 | Carmon2019Unlabeled | ~54.8% |
| 3 | Wu2020Adversarial | ~51.6% |
| 4 | Rice2020Overfitting | ~51.6% |
| 5 | Engstrom2019Robustness | ~49.2% |

---

## Key Insight

Rebuffi2021Fixing_70_16_cutmix_extra is consistently the strongest model across all perturbation levels, while Engstrom2019Robustness shows the weakest overall robustness on average.
