# Ragnarok — Community

> **AI-native KubeVirt VM management — natural language provisioning, autonomous healing, cost optimization**

Public issue tracker and community feedback space for **Ragnarok** by [Zyvor AI Labs](https://zyvor.dev).

The source code is maintained in a private repository. This repo is for:
- Bug reports
- Feature requests
- UX feedback
- Documentation gaps
- Questions and discussion

---

## Key features

- Natural language VM provisioning — describe what you want in plain English
- AI healer — detects and autonomously remediates VM incidents
- AI cost optimizer — tracks per-VM cost, detects waste, forecasts spend
- Template wizards — no KubeVirt YAML knowledge required
- Unified React dashboard with full VM lifecycle management
- Rust API + Postgres backend
- KubeVirt operator, Terraform, and Ansible deploy paths

---

## Installation

**Helm (requires KubeVirt cluster):**
```bash
helm repo add hypersdk https://charts.hypersdk.dev
helm upgrade --install ragnarok hypersdk/ragnarok \
  --namespace ragnarok-system --create-namespace
```

**Local dev:**
```bash
git clone https://github.com/hypersdk/ragnarok && cd ragnarok
make dev
```

**Requirements:** Kubernetes 1.28+, KubeVirt installed, PostgreSQL (bundled in Helm chart)

See [QUICKSTART.md](https://github.com/hypersdk/ragnarok/blob/main/docs/QUICKSTART.md) for the full guide.

---

## Report a bug

[Open a Bug Report →](../../issues/new?template=bug_report.yml)

Include: what you did, what happened, what you expected, your environment, and screenshots/logs (redact secrets).

## Request a feature

[Open a Feature Request →](../../issues/new?template=feature_request.yml)

## UX feedback

[Open a UX Feedback →](../../issues/new?template=ux_feedback.yml)

## Ask a question

Use [GitHub Discussions](../../discussions) for open-ended questions, ideas, and roadmap conversations.

---

## Security

**Do not report security vulnerabilities publicly.**

Email **security@zyvor.dev** — see [SECURITY.md](SECURITY.md).

---

## Do not post

- Source code or internal configuration
- API tokens, license keys, or credentials  
- Private logs with sensitive data
- Security vulnerabilities (email security@zyvor.dev)

---

Maintained by [Zyvor AI Labs](https://zyvor.dev)
