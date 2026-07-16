# Harden My Repo

Evidence-first tools for repositories that use AI coding agents.

## Start free

- **[Harden My Repo Doctor](https://github.com/hardenmyrepo/doctor)** — a dependency-free Node.js CLI and GitHub Action that checks inspectable repository-readiness evidence without executing project code or using the network.
- **[Browser Repository Audit](https://hardenmyrepo.github.io/browser-audit/)** — a static, open-source readiness snapshot. Repository data stays in the browser; there is no login, analytics, cookie, or upload.
- **[Claude Code Hooks](https://github.com/hardenmyrepo/claude-code-hooks)** — three tested, inspectable project hooks for dangerous commands, protected paths, and format-on-edit.

## Use the Doctor Action

```yaml
- uses: hardenmyrepo/doctor@v1
  with:
    path: .
    fail-below: "60"
```

## Deeper local evidence

[Harden My Repo](https://hardenmyrepo.com/?utm_source=github&utm_medium=profile&utm_campaign=profile-readme) also provides an adaptable setup kit and a bounded local analyzer that produces HTML, Markdown, and JSON reports plus inert remediation drafts.

These are configuration-readiness tools, not security audits or certifications. Findings are review prompts and should be evaluated against each repository's architecture and risk tolerance.
