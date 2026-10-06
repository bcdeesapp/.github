## What this changes

<!-- Two or three sentences a teammate can read without opening the diff. What was wrong or missing, and what is true now. -->

## Linear

<!-- Name the ticket with "Part of", never "Closes" or "Fixes". A merge moves the ticket to On Staging, and Done is set by hand after the check on staging. -->

Part of BCD-

<!-- If this pull request is only one piece of a larger ticket, say which piece, and say what is still left. -->

## How to check it

<!-- Steps a reviewer can follow on staging, or the test that proves it. For a bug, say how you reproduced it first. -->

1.
2.

## Tests

- [ ] New or changed behaviour has a test
- [ ] Existing checks pass locally and in CI
- [ ] For a defect fix: the test fails without this change and passes with it

## Touches money, limits or webhooks?

<!-- Anything under wallet, ledger, fees, escrow, limits or webhook folders. If yes, a second reviewer is required. -->

- [ ] No
- [ ] Yes, and I have listed below what happens if this fails halfway, and what happens if the same request or webhook arrives twice

## Database or config changes

- [ ] None
- [ ] Migration included, rehearsed on a copy of staging data, and the rollback is written below
- [ ] New or changed environment variable, added to the environment matrix and to staging and production

## Rollout and rollback

<!-- How this goes out, whether it needs a flag, and how we undo it. "Revert the pull request" is a fine answer when it is true. -->

## Screenshots or recordings

<!-- For anything a person can see: mobile, back office or website. Before and after. -->

## Before you ask for review

- [ ] The branch name and the ticket match, and the ticket is In Progress
- [ ] I read my own diff once and removed stray logs, commented code and unrelated edits
- [ ] The pull request is small enough to review in one sitting, or I have said in the description how to read it in order
- [ ] No secrets, keys or personal data in the code, the logs or the screenshots
