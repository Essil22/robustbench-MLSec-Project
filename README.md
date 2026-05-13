# robustbench-MLSec-Project
# CIFAR-10 Adversarial Robustness Evaluation using AutoAttack

## Project Overview

This project evaluates the robustness of five adversarially trained CIFAR-10 models from RobustBench under multiple ℓ∞ perturbation strengths using AutoAttack.

The objective is to analyze how adversarial robustness changes as epsilon increases and to study whether model rankings remain stable across different attack strengths.

---

## Evaluated Models

The following RobustBench models were evaluated:

- Carmon2019Unlabeled
- Rebuffi2021Fixing_70_16_cutmix_extra
- Rice2020Overfitting
- Engstrom2019Robustness
- Wu2020Adversarial

---

## Evaluation Settings

- Dataset: CIFAR-10
- Threat Model: ℓ∞
- Attack Method: AutoAttack
- Evaluation Device: CUDA GPU
- Number of Test Samples: 50
- Epsilon Values:
  - 1/255
  - 4/255
  - 8/255
  - 12/255
  - 16/255

---

## Methodology

For each model:

1. The clean accuracy was computed on a subset of CIFAR-10 test images.
2. AutoAttack was applied using several epsilon values.
3. The robust accuracy was measured after adversarial perturbation.
4. Robustness curves and ranking stability graphs were generated to compare model behavior across perturbation strengths.

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

## Key Findings

- Robust accuracy decreases progressively as epsilon increases for all evaluated models.
- Rebuffi2021Fixing_70_16_cutmix_extra achieved the best overall robustness and stability.
- Several models changed ranking positions depending on epsilon.
- Robustness rankings are not universally stable and depend strongly on perturbation strength.
- Evaluating robustness using a single epsilon value may not fully reflect model behavior under adversarial attacks.

---

## Repository Structure

```text
.
├── notebooks/
├── figures/
├── results/
├── robust_accuracy.csv
├── rankings.csv
├── requirements.txt
└── README.md
