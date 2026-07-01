### Ticket 🎟
[BWA-xxxx](https://trustpilot-production.atlassian.net/browse/BWA-xxxx)

### What ⁉️
_What does this feature add or change in the microservice?_
_Summarise the any contract change (new type, changed request/response shape etc.)._
_If a LaunchDarkly flag gates the change, note the flag name and default value._

### Why ⁉️
_Why is this change needed?_
_(e.g. support new feature, security hardening, cost reduction, deprecation of old resource)_

### How to test locally 🖥
_Steps to invoke and verify the microservice change on a developer machine:_

```bash
# Install dependencies
npm install

# Run tests
npm run test

# Describe test payload
# Put test payload local test file
npm run local
```

_Describe what a successful local response looks like._


### Risk, blast radius & rollback 💥
_What systems, environments, or teams could be affected? Is there a risk of data loss, increased latency, or cost spike?_
_Is a maintenance window or coordinated deploy needed?_
_How do we revert if this causes an incident? (e.g. roll back the CloudFormation stack, re-deploy previous Lambda version via alias, revert SSM parameter)_
_Are there any non-reversible steps (e.g. table deletion, data migration)?_

### Checklist ✅
- [ ] My changes generate no new warnings
- [ ] Lambda tested locally with a representative event payload
- [ ] I have added/amended tests to verify this change works
- [ ] All new and existing unit, integration and/or e2e tests have been run and are passing against my branch
- [ ] New SSM parameters / secrets provisioned in all target environments
- [ ] Manual steps outside this PR documented in the ticket
- [ ] Rollback plan is documented above
