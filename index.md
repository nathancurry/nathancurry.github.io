---
layout: page
title: Nathan Curry
tagline: Applied AI · Forward Deployed Engineering
description: Nathan Curry builds agentic LLM systems and runs them on self-hosted infrastructure. Software Maintenance Engineer at Red Hat.
---

I build agentic LLM systems and run them in production on self-hosted infrastructure. Before that, and alongside it, I spent eight years at Red Hat, SAP NS2 and Redis debugging customers' distributed systems under 15-minute SLAs, leading incident bridges, and writing the Python and Ansible tooling that took the manual work out.

I'm a Software Maintenance Engineer in OpenShift Enhanced Support at Red Hat (July 2024 to present), where I also built an AI troubleshooting assistant that works alongside support engineers on live cases.

[GitHub](https://github.com/junglestyle) · [LinkedIn](https://linkedin.com/in/nathandcurry) · [nathancurry@gmail.com](mailto:nathancurry@gmail.com)

### What I'm building

**[Hearsay](https://github.com/junglestyle/hearsay) → [Idea Machine](https://github.com/junglestyle/ideamachine) → [Lattice](https://github.com/junglestyle/lattice)**: from recorded conversations to an idea map. Python, Swift, pgvector.

- Hearsay transcribes conversations recorded with consent. iOS and macOS capture apps (BLE pendant, two-channel mic and system audio) feed a self-hosted pipeline: Parakeet transcription, pyannote speaker diarization, and a web portal for naming speakers. Audio never leaves my own hardware.
- Idea Machine triages the transcripts. I evaluated a local LLM, a small classifier and a logistic-regression baseline on hand-labeled episodes, measuring accuracy and reliability per question and router precision.
- Claude extracts ideas from what's left, and every keep or discard is logged with a reason and fed back into the extraction prompt. Lattice turns the result into a browsable idea map.

**[Hypertrace](https://github.com/nathancurry/hypertrace)**: an auditable LLM research harness. The model proposes searches and interpretations; source text, exact excerpts, dates and review notes are stored with provenance so every claim traces back. Batched adversarial review, per-provider cost accounting, failover on rate limits, 119 tests.

**[Teem](https://github.com/junglestyle/teem)** (archived): turned a Telegram voice note into a pull request. Claude Code implemented in egress-restricted rootless Podman containers, checks ran, and Codex reviewed the result adversarially. Work started only on an Approve button, and no model could grant permissions or declare its own work done. I built it to understand the problem, and archived it once it was stable, with a [write-up of the lessons](https://github.com/junglestyle/teem#lessons-im-carrying-forward).

### At Red Hat

- Built an AI troubleshooting assistant for Enhanced Support engineers that launches Claude or Gemini as a partner on a live case, with durable per-case knowledge and deterministic guardrails on its tools. It carries 22 domain skills that mirror Red Hat's support-group boundaries, plus a review skill that separates observed, attributed and inferred claims before anything reaches a customer.
- Built Thunder with AI coding agents: a Go terminal UI that gives support engineers fast access to the case they're working, now used by other engineers.
- Lead customer incident bridges for production OpenShift outages at premium accounts, and turn what customers hit into engineering work: bugs, backports and Requests for Enhancement.

### Before that

- **SAP NS2** (2022–2024): technical lead for Linux security and DISA STIG compliance across AWS GovCloud FedRAMP environments. Built an Ansible remediation framework and a Python STIG-checklist tool that each cut the manual work by more than half.
- **Redis** (2021–2022): escalation engineer for Redis Enterprise on Linux and Kubernetes.
- **Red Hat, OpenStack Enhanced Support** (2018–2021): incident response for telco NFV deployments (SR-IOV, NUMA, OVS-DPDK, SDN).

### Skills

- **AI:** Claude and OpenAI-compatible APIs, Claude Code and Codex agents, prompt design, LLM evals and baselines, adversarial review, pgvector, Parakeet, pyannote
- **Languages:** Python, Bash, SQL, Swift, Go (basics)
- **Platforms:** Kubernetes, OpenShift, Podman, Docker, AWS and GovCloud, GCP, OpenStack, RHEL
- **Automation and ops:** Ansible, Terraform, GitLab CI, OpenShift GitOps and Pipelines, Prometheus, Grafana
- **Security:** OpenSCAP, DISA STIG, FedRAMP, CVE triage

Red Hat Certified Architect (Infrastructure), Red Hat Certified OpenShift Administrator, CompTIA Security+, HashiCorp Terraform Associate. Bachelor of Music, University of Miami. Fluent Spanish.
