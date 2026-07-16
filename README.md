# Harden My Repo

Evidence-backed repository reliability findings and fixes.

## Repository Reliability Sprint

The **[$750 Repository Reliability Sprint](https://hardenmyrepo.com/repository-reliability-sprint?utm_source=github&utm_medium=profile&utm_campaign=reliability_sprint)** reviews one repository's CI/CD, release path, dependency controls, secret handling, ownership boundaries, and recovery evidence. It includes a prioritized report, a review-ready patch for up to three agreed fixes, and a verification ledger.

Start with a **[free five-point teardown](https://hardenmyrepo.com/repository-reliability-sprint?utm_source=github&utm_medium=profile&utm_campaign=reliability_sprint#teardown)** of a public repository you maintain. No sales call or production access is required.

## Start free

- **[Harden My Repo Doctor](https://github.com/hardenmyrepo/doctor)** — a dependency-free Node.js CLI and GitHub Action that checks inspectable repository-readiness evidence without executing project code or using the network.
- **[Browser Repository Audit](https://hardenmyrepo.github.io/browser-audit/)** — a static, open-source readiness snapshot. Repository data stays in the browser; there is no login, analytics, cookie, or upload.
- **[Claude Code Hooks](https://github.com/hardenmyrepo/claude-code-hooks)** — three tested, inspectable hooks for dangerous commands, protected paths, and format-on-edit, installable as a Claude Code plugin.

## Use the Doctor Action

Run the CLI directly from GitHub with Node.js 20 or newer:

```bash
npm exec --yes --package=github:hardenmyrepo/doctor -- harden-my-repo .
```

Or add the maintained major version to GitHub Actions:

```yaml
- uses: hardenmyrepo/doctor@v1
  with:
    path: .
    fail-below: "60"
```

## Install the Claude Code hooks

Review the three shell scripts, then run these commands inside Claude Code:

```text
/plugin marketplace add hardenmyrepo/claude-code-hooks
/plugin install harden-my-repo-hooks@harden-my-repo
```

## Self-serve local evidence

[Harden My Repo](https://hardenmyrepo.com/?utm_source=github&utm_medium=profile&utm_campaign=self_serve) also provides an adaptable setup kit and a bounded local analyzer that produces HTML, Markdown, and JSON reports plus inert remediation drafts.

The sprint and self-serve tools are repository reliability/configuration reviews, not penetration tests, security certifications, or guarantees. Findings are evaluated against the repository's architecture and risk tolerance before any remediation is proposed.
