# Contributing to BCDees

Thank you for contributing. These guidelines apply across all BCDees repositories.

## Branching Strategy

We use **trunk-based development** with short-lived feature branches.

```
main          — production-ready code; protected, requires PR + review
staging       — pre-production integration branch
dev           — active development integration
feature/*     — short-lived feature branches (branch from dev)
fix/*         — bug fix branches
hotfix/*      — urgent production fixes (branch from main)
```

Branch naming examples:
- `feature/kyc-tier-2-submission`
- `fix/escrow-release-race-condition`
- `hotfix/wallet-balance-display`

## Commit Messages

Follow [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short description>

[optional body]

[optional footer: JIRA/issue ref]
```

**Types:** `feat` · `fix` · `chore` · `docs` · `refactor` · `test` · `perf` · `ci`

**Scopes (examples):** `auth` · `kyc` · `wallet` · `p2p` · `escrow` · `admin` · `api` · `mobile` · `infra`

Examples:
```
feat(escrow): lock NGN on order creation before FX confirmation
fix(kyc): handle null BVN on tier-2 submission
docs(api): add wallet endpoint response schemas
```

## Pull Requests

- PRs must target `dev` (or `staging` for release candidates). Never directly to `main`.
- Fill out the PR template completely.
- All CI checks must pass before merge.
- Minimum **1 approval** required; **2 approvals** for anything touching wallet, escrow, or auth.
- Keep PRs small and focused — one concern per PR.

## Code Review Expectations

**For reviewers:**
- Review within 24 hours (business days).
- Be specific and constructive.
- Approve only what you'd be comfortable owning.

**For authors:**
- Respond to all comments before merging.
- Don't force-push after review starts.

## Issue Reporting

Use the appropriate issue template:
- 🐛 **Bug Report** — something is broken
- ✨ **Feature Request** — new capability
- 🔒 **Security Issue** — email security@bcdees.com directly; do not open a public issue

## Security & Sensitive Data

- **Never commit** API keys, secrets, wallet credentials, or PII.
- Use `.env.example` files for environment variable documentation.
- Any accidental secret commit → immediately rotate the credential and notify the team.

## Questions?

Open a Discussion in the relevant repo or reach out in the team Slack.
