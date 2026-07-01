### Ticket 🎟
[BWA-xxxx](https://trustpilot-production.atlassian.net/browse/BWA-xxxx)

### What ⁉️
_What does this feature add or change in the backend?_
_Summarise the API contract change (new endpoint, changed request/response shape, new query param, etc.)._
_If a LaunchDarkly flag gates the change, note the flag name and default value._

### Why ⁉️
_Why is this feature needed?_
_What downstream system is this serving or integrating with (e.g. Salesforce, SNS, SQS, DynamoDB)?_

### How to review and test 📱
**Helpful resources for generating test users:**
1. [Create and upgrade account – Creating test business units and users](https://trustpilot-production.atlassian.net/wiki/spaces/GPT/pages/2725969952/Developer+Onboarding)
2. [Business Accounts List (TP Admin)](https://p81-admin.tp-staging.com/BusinessAccounts/List)
_Steps to verify the feature in staging or locally:_

**Helpful resources for generating test users:**
1. [Create and upgrade account – Creating test business units and users](https://trustpilot-production.atlassian.net/wiki/spaces/GPT/pages/2725969952/Developer+Onboarding)
2. [Business Accounts List (TP Admin)](https://p81-admin.tp-staging.com/BusinessAccounts/List)

1. Run locally (`assume trustpilot-classic && npm start`).
2. Call the endpoint: `curl -X POST https://<base-url>/<path> -d '<payload>'`
3. Describe the expected response body and HTTP status.



[Standard headers for internal/private endpoints](https://trustpilot-production.atlassian.net/wiki/spaces/GPT/pages/2725969952/Developer+Onboarding#Calling-your-first-endpoint)


### Risk, blast radius & rollback 💥
_What could go wrong? Which downstream systems or data are at risk?_
_Is this change backward-compatible with the current message schema?_
_How do we undo this in production? (e.g. disable LaunchDarkly flag, revert Lambda deployment via alias/version rollback, re-deploy previous CloudFormation stack)_

### Checklist ✅
- [ ] My changes generate no new warnings
- [ ] I have added tests that prove the feature works (unit + integration + e2e where applicable)
- [ ] New and existing unit/integration tests pass locally
- [ ] Local E2E tests have been run and are passing against my branch
- [ ] error path tested
- [ ] Rollback plan is documented above
- [ ] Feature flag / gradual rollout considered if applicable
