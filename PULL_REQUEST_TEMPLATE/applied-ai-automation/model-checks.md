
# 🧑‍💻 Model checks

---

#### ❗️THIS SECTION MUST BE COMPLETED BEFORE PR APPROVAL❗️

> *Shows/hides AUTOMATICALLY depending if model files have changed*

---

*Confirm ALL checks:*

- [ ] 📈 I have confirmed the performance of the model is as expected (see "Shadow deployments log" section for shadow training pipeline run)
- [ ] ⁉️ My changes do not introduce a discrepancy between training and inference (e.g. features used, data transformations, etc.)
  - check training/inference consistency with Copilot review by using `/compare-training-inference` as a PR comment
- [ ] 🐈‍⬛ I ran inference using shadow deployment or local testing and confirmed the model is working as expected (see "Shadow deployments log" section for shadow inference pipeline run)
- [ ] 🕵️ F&I have validated and signed off on the model performance and monitoring plan
- [ ] 👍 I have received approval from my function lead to deploy this model
- [ ] 📊 New circuit breaker thresholds have been communicated to Engineering, or I have confirmed that no changes are necessary
