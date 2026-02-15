# Arch Platform Technologies

## Overview
**Client**: Arch Platform Technologies (Arch PT)
**Ali's Role**: Ruby on Rails Engineer (Freelance)
**Platform**: Mane — a cloud orchestration platform providing Virtual Desktop Infrastructure (VDI) on AWS
**Started**: Mid-2025 (onboarding calls July 2025)
**Code Location**: `/Users/najafali/Code/freelance/archpt/`

## What Mane Does
Manages the full lifecycle of cloud workstations on AWS — provisioning infrastructure, managing user access, monitoring usage. Enables organizations to provide secure, scalable remote desktop environments.

Key capabilities:
- Facility creation (automated AWS infra: VPC, subnets, security groups)
- Workstation lifecycle (create, boot, shutdown, reboot EC2 instances)
- Image pipelines (Chef-based AMI building)
- User/access management (SSO via WorkOS, RBAC, directory integration)
- SSM parameter management (Ali's recent feature)

## People
- **Simon Lau** — Primary developer, Ali's main technical contact. Friendly, responsive in bursts.
- **Edward Churchward (Ed)** — Business side, cares about visible progress and attendance.
- **Jon Mah** — Team member
- **Olly Glenn** — Team member

## Tech Stack
- **Backend (mane/)**: Rails 6.1, Ruby 2.7.8, PostgreSQL, Redis, Sidekiq, Graphiti (JSON:API), Pundit, Statesman
- **Frontend (mane-frontend/)**: React 18, Material-UI v5, Redux-bundler
- **Auth**: Ory Hydra (OAuth2/OIDC), BFF token handler (Node.js), WorkOS (SSO)
- **Infra**: Deep AWS integration (EC2, VPC, SSM, Lambda, CloudFormation)
- **Dev env**: Caddy reverse proxy, Zellij layout, local domains (api.local.com:8443, app.local.com)

## Repository Structure
All in `/Users/najafali/Code/freelance/archpt/`:
- `mane/` — Rails API backend (main app, has its own CLAUDE.md)
- `mane-frontend/` — React SPA
- `bff-token-handler/` — Node.js token handler
- `hydra/` — Ory Hydra OAuth2 server
- `caddy/` — Reverse proxy config
- `mane-dev-setup/` — Centralized dev config (symlinked)
- `arch-workshop/` — Documentation, Claude Code workflow, session logs

## Customers
- Fox
- Imagica

## Working Patterns
- Branch naming: `na-feature-<name>` or `na-chore-<name>`
- Ali's last feature: SSM Parameter Management
- Daily standups (Ali targets 3x/week: Tue, Wed, Fri)
- Ed values visible activity — PRs, docs, demos matter for optics
- Simon is the only one who can fix deep platform issues (bus factor risk)

## Relationship History
- July 2025: Onboarding calls with Simon, steep learning curve on vast technical domain
- Aug 2025: Got to point of contributing mergeable PRs, built rapport with Simon
- Sep 2025: Attendance dropped, Ed concerned. Ali created "recapture strategy" (demos, PR descriptions, Notion docs)
- Oct 2025: Programming sessions, continued SSM parameter work

## Obsidian Vault References
Key notes in ali-vault:
- `Arch Platform Technologies.md` — Main hub note
- `Arch Work Reflections.md` — Ali's candid reflections on the engagement
- `Arch Glossary.md` — Domain terminology
- `2025-09-29 - Arch recapture strategy.md` — Recovery plan after attendance dip
- `2025-10-20 Arch Programming Session.md`
- `Chat with Ed at Arch Tech.md` — Initial conversation notes
- `Arch S1E1 - The Tale of El Brancho.md` / `S1E2` — Work session stories

## Detailed Claude Code Context
The comprehensive CLAUDE.md at `/Users/najafali/Code/freelance/archpt/CLAUDE.md` has full architecture diagrams, domain model, and development workflows. Read that file when doing actual Arch development work.

---
*Last updated: 2026-01-31*
