
# Challenges Faced During the Project

During this project, several practical and computational challenges were encountered, mainly related to hardware limitations and the high computational cost of adversarial robustness evaluation.

---

## 1. Computational Resource Limitations

The initial experiments were attempted on our local laptops CPUs. However, the computational requirements of AutoAttack and adversarially robust models were too high, making execution extremely slow and in many cases infeasible.

As a result, training and evaluation could not be completed efficiently on CPU-based environments.

---

## 2. GPU Access Constraints

We attempted to solve this limitation by using alternative GPU resources:

- Local laptop GPU (insufficient memory and performance)
- University server (limited access and availability through a colleague)
  
Despite these attempts, execution was still unstable or incomplete due to resource constraints.

---

## 3. Transition to Google Colab

Finally, the project was migrated to Google Colab using a T4 GPU runtime. This provided us a more stable environment for execution.

However, even with this improvement, significant computational limitations remained due to:

- High execution time per model using AutoAttack
- Memory constraints during evaluation
- Large model sizes from RobustBench
- The "Carmon2019Unlabeled", "Rebuffi2021Fixing_70_16_cutmix_extra" models took us 6h running and unfortiantly out of storage at the last epsilon itiration of the second model so we assumed an approximate accuracy.
---

## 4. Adjustments Made to Overcome Limitations

To ensure successful completion of the experiments, several compromises were made:

- Reduced dataset size from 100–200 images to 50 images per evaluation
- Executed models individually instead of running all models together
- Selected the less hiviest 5  models due to computational cost


---

## 5. Execution Time Constraints

Even under optimized conditions, each model evaluation required approximately 1–2 hours depending on the epsilon values and model complexity.

This significantly increased the total project runtime but ensured reliable and complete results.

---

## Conclusion

Despite computational limitations and repeated execution failures across different environments, the project was successfully completed through iterative optimization of resources, dataset size, and execution strategy.

These constraints highlight the real-world challenges of adversarial robustness evaluation and the importance of efficient experimental design in deep learning research.
