> 🚀 **Trial v0.30.0 is live!** The latest release is available for trial today — [get started in 5 minutes →](#try-v030-in-5-minutes)

# Ragnarok — Community

> **AI-native KubeVirt VM management — natural language provisioning, autonomous healing, cost optimization.**

![Version](https://img.shields.io/badge/version-v0.30.0-blue) ![Discussions](https://img.shields.io/github/discussions/hypersdk/ragnarok-community) ![Issues](https://img.shields.io/github/issues/hypersdk/ragnarok-community) ![License](https://img.shields.io/badge/license-Proprietary-red)

Public issue tracker and community feedback space for **Ragnarok** by [Zyvor AI Labs](https://zyvor.dev).
The source code is maintained in a private repository. This repo is for bug reports, feature requests, UX feedback, and community discussion.

---

## What's new in v0.30

- NL provisioning GA — describe a VM in plain English, Ragnarok creates the KubeVirt manifest and deploys it
- Cost forecasting — per-VM 30-day cost projection based on historical resource usage
- AI healer auto-approve — configure thresholds for fully autonomous remediation without human gates
- Helm v0.30 — bundled PostgreSQL, cert-manager, and ingress — single chart, one command deploy
- Playwright E2E test suite — full coverage of VM lifecycle, AI flows, and cost dashboard

---

## Why Ragnarok

| Problem | Ragnarok answer |
|---------|----------------|
| KubeVirt YAML is verbose and error-prone | Template wizards and NL provisioning — describe what you want, Ragnarok creates it |
| No VMware vCenter equivalent for Kubernetes VMs | Unified dashboard with full VM lifecycle, metrics, and cost in one place |
| GPU and VM fleet costs are invisible until the bill arrives | Per-VM cost tracking, waste detection, and 30-day forecasting |
| Incident response is reactive and slow | AI healer detects and autonomously remediates — configurable from advisory to auto-approve |
| KubeVirt ops require Kubernetes expertise | Chat-style ops — ask questions, get answers, take actions without kubectl |

---

## Architecture

```
┌──────────────────────────────────────────────────────────────┐
│  Frontend     React dashboard · AI copilot · VM wizards      │
├──────────────────────────────────────────────────────────────┤
│  Backend      Rust API · Postgres · KubeVirt operator        │
├──────────────────────────────────────────────────────────────┤
│  AI           NL provisioning · Healer · Cost optimizer      │
└──────────────────────────────────────────────────────────────┘
```

---

## Try v0.30 in 5 minutes

```bash
# Helm (requires KubeVirt cluster)
helm repo add hypersdk https://charts.hypersdk.dev
helm upgrade --install ragnarok hypersdk/ragnarok --version 0.30.0 \
  --namespace ragnarok-system --create-namespace

# Local dev
git clone https://github.com/hypersdk/ragnarok && cd ragnarok
git checkout v0.30.0 && make dev
```

**Requirements:** Kubernetes 1.28+, KubeVirt installed, PostgreSQL (bundled in Helm chart)

---

## Report a bug

[Open a Bug Report →](../../issues/new?template=bug_report.yml)

Include: what you did, what happened, what you expected, your environment, screenshots or logs (redact secrets).

## Request a feature

[Open a Feature Request →](../../issues/new?template=feature_request.yml)

## UX feedback

[Open a UX Report →](../../issues/new?template=ux_feedback.yml)

## Ask a question

Use [GitHub Discussions](../../discussions) for open-ended questions, ideas, and roadmap conversations.

---

## Security

**Do not report security vulnerabilities publicly.**
Email **security@zyvor.dev** — see [SECURITY.md](SECURITY.md).

---

## Do not post

- Source code, internal configs, or architecture details
- API tokens, license keys, or credentials
- Private logs with sensitive data
- Security vulnerabilities — email security@zyvor.dev instead

---

## Join the community

⭐ [Star this repo](https://github.com/hypersdk/ragnarok-community) · 💬 [Open a Discussion](https://github.com/hypersdk/ragnarok-community/discussions) · 🐛 [Report a Bug](../../issues/new?template=bug_report.yml) · 📧 [hello@zyvor.dev](mailto:hello@zyvor.dev)

Maintained by [Zyvor AI Labs](https://zyvor.dev)
