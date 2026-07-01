### Ticket 🎟
[BWA-xxxx](https://trustpilot-production.atlassian.net/browse/BWA-xxxx)

### What ⁉️
_What does this feature add or change in the UI?_
_Include screenshots or GIFs for any layout, style, or interaction change — even small ones.
_Which user-facing flow is affected (e.g. `/form`, `/create-account`, signup popup)?_

### Why ⁉️
_Why is this feature needed?_

### How to review and test 📱
_Steps to exercise the feature locally or in staging:_

**Helpful resources for generating test users:**
1. [Create and upgrade account – Creating test business units and users](https://trustpilot-production.atlassian.net/wiki/spaces/GPT/pages/2725969952/Developer+Onboarding)
2. [Business Accounts List (TP Admin)](https://p81-admin.tp-staging.com/BusinessAccounts/List)
3. [VoiceOver Guide](https://trustpilot-production.atlassian.net/wiki/spaces/EN/pages/1267400728/Intro+to+VoiceOver+for+Developers)

**If the change is component-only (no full user flow required):**
1. Run Storybook (`npm run storybook`) and navigate to the relevant story.
2. _(Link the Storybook story or describe which story covers this component.)_
3. _(Describe the props / controls to set and the expected visual outcome.)_

**If the change requires a full user flow:**
1. Run `npm start` and navigate to the relevant route.
2. _(List the exact URL with any query params needed, e.g. `?domain=example.com&domainLocked=true`)_
3. _(Describe the interaction to trigger the feature — button click, form submit, flag state, etc.)_
4. _(State the expected visual or behavioural outcome.)_
5. If a LaunchDarkly flag controls the feature, describe how to toggle it in the local dev config or staging environment.
6. Open the browser DevTools and check responsiveness at all reasonable width and heights of screen (from small phone to horizontal tablet to 4k monitor)
7. Verify accessibility:
   - Tab through all interactive elements and confirm logical focus order with no focus traps.
   - Activate the feature using keyboard only (Enter / Space / arrow keys).
   - Enable VoiceOver (macOS: `⌘ F5`) and confirm all controls have meaningful labels, state changes are announced, and no content is inaccessible. See [Intro to VoiceOver for Developers](https://trustpilot-production.atlassian.net/wiki/spaces/EN/pages/1267400728/Intro+to+VoiceOver+for+Developers).
   - Run the [axe DevTools](https://www.deque.com/axe/devtools/) browser extension (or Lighthouse Accessibility audit) and resolve any violations before merging.

### Risk, blast radius & rollback 💥
_What could go wrong? Which users, markets, or flows are affected?_
_Does this change affect shared components used across multiple pages or flows?_
_Are there any A/B tests or experiments currently running on the same surface?_
_How do we turn this off or undo it in production? (e.g. disable LaunchDarkly flag, revert commit, config change)_

### Checklist ✅
- [ ] My changes generate no new warnings
- [ ] I have added tests (unit, integration and/or E2E where relevant) that prove the feature works
- [ ] Local E2E tests have been run and are passing against my branch
- [ ] New and existing tests pass locally
- [ ] Screenshots / GIFs included for all visual changes
- [ ] Tested with keyboard navigation and VoiceOver (screen reader)
- [ ] en-US translation keys added for all strings (including those for screen readers)
- [ ] Segment tracking events verified (added / updated where needed)
- [ ] LaunchDarkly flag usage documented (if applicable)
- [ ] Rollback plan is documented above
- [ ] Feature flag / gradual rollout considered if applicable
