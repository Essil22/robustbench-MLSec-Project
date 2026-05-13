# robustbench-MLSec-Project
We chose PROJECT-1 from proposed list where we :
Selected 5 CIFAR-10 ℓ∞ models from RobustBench
Used a small subset of 50 CIFAR-10 test images.
Re-evaluate these models using AutoAttack under several epsilon values: from about 1/255 to 16/255 including the standard benchmark 8/255.
For each model and epsilon:
compute the baseline accuracy
compute the AutoAttack robust accuracy.
Compare:
how robustness changes as epsilon increases
how the ranking of models changes across epsilon values.
Analyze whether the rankings are:
stable
or if some models move significantly up/down.
Discuss what these ranking changes reveal about the reliability of RobustBench leaderboards and whether robustness rankings depend strongly on the chosen epsilon.

MODEL ZOO :

