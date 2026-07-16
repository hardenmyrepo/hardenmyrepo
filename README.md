# Harden My Repo

Evidence-first tools for repositories that use AI coding agents.

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

## Deeper local evidence

[Harden My Repo](https://hardenmyrepo.com/?utm_source=github&utm_medium=profile&utm_campaign=profile-readme) also provides an adaptable setup kit and a bounded local analyzer that produces HTML, Markdown, and JSON reports plus inert remediation drafts.

These are configuration-readiness tools, not security audits or certifications. Findings are review prompts and should be evaluated against each repository's architecture and risk tolerance.
