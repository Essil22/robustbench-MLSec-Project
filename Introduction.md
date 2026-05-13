# Introduction

## 1. Adversarial Robustness in Deep Learning

Deep neural networks are known to be vulnerable to small but carefully crafted perturbations called adversarial attacks. These perturbations can significantly affect model predictions while remaining almost imperceptible to humans.

To evaluate and compare model robustness, standardized benchmarks and strong evaluation methods are required.

---

## 2. RobustBench

RobustBench is a benchmark designed to systematically evaluate and track progress in adversarial robustness research. It provides:

- Standardized adversarially trained models
- Reproducible evaluation settings
- Benchmark results on CIFAR-10 and other datasets

In this project, we use pretrained models from RobustBench to ensure fair and reproducible comparisons.

---

## 3. AutoAttack

AutoAttack is a widely used evaluation framework for adversarial robustness. It combines multiple strong attack strategies (white-box and black-box) to provide a reliable and standardized robustness evaluation.

It is used in this project to compute robust accuracy under different ℓ∞ perturbation strengths.

---

## 4. Relationship Between RobustBench and AutoAttack

RobustBench provides the models and benchmarking framework, while AutoAttack provides the standardized evaluation method.

Together, they allow:

- Fair comparison between different models
- Reliable robustness measurement
- Reduced risk of overestimated robustness results

---

## 5. Evaluation Setting in This Project

In this work:

- CIFAR-10 pretrained models from RobustBench are evaluated
- AutoAttack is used for adversarial evaluation
- ℓ∞ perturbations are applied with different epsilon values:
  1/255 → 16/255
- A subset of test images is used due to computational constraints

---

## 6. Goal of This Study

The main goal of this project is to analyze:

- How robustness changes as perturbation strength increases
- Whether model rankings remain stable across epsilon values
- The reliability of robustness comparisons under different evaluation settings
