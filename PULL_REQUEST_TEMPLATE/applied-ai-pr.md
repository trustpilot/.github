# 📝 PR Documentation
*Description*
`<In 1-2 sentences, describe what this change does and why it is needed.>`

## ✅ Release Checklist
THE RELEASE CHECKLIST MUST BE COMPLETED BEFORE THIS PR IS APPROVED.
=========================
*This release is an:*
- [ ] ⚙️ Infrastructure change (e.g. CI/CD, monitoring, tooling, etc.)
- [ ] 🧠 Model change (e.g new model, new features, etc.)

## General checklist
- [ ] 🔙 I can rollback this change if something goes wrong
- [ ] 👓 I will monitor the live service after deploying this change or have arranged for someone to do so
- [ ] 📄 I have updated documentation or this is not applicable

*Select ONE 🐈‍⬛ of the following 3 options:*
- [ ] 🐈‍⬛ Shadow deployment **is available** and I have tested that my code changes work in the shadow environment. Link: `<insert link to shadow deployment dashboard or logs>`
- [ ] 🐈‍⬛ Shadow deployment **is not available**, and I have tested that my code changes work in a local or staging environment. Link: `<insert link to locally triggered test run or description of local testing>`
- [ ] 🐈‍⬛ This is a CI/CD change, and is not subject to shadow deployment or local testing, but I have tested the changes before merging to main.

*Select ONE ⌛ of the following 2 options:*
- [ ] ⌛ I confirm that I am deploying this change in the morning / early afternoon and not on a Friday or during code freeze
- [ ] ⌛ I have obtained approval from my function lead to deploy this change outside of the regular hours

## Model changes only
- [ ] 📈 I have confirmed the performance of the model is as expected. `<insert link to training run or evaluation results>`
- [ ] ⁉️ My changes do not introduce a discrepancy between training and inference (e.g. features used, data transformations, etc.)
- [ ] 🐈‍⬛ 🐈‍⬛ I ran inference using shadow deployment or local testing and confirmed the model is working as expected. Link: `<insert link to shadow deployment, or link to locally triggered test run>`
- [ ] 🕵️ F&I have validated and signed off on the model performance and monitoring plan
- [ ] 👍 I have received approval from my function lead to deploy this model
- [ ] 📊 New circuit breaker thresholds have been communicated to Engineering, or I have confirmed that no changes are necessary