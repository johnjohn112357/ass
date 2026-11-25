# NCFE Assessor Agent — Portable Project

**Edition:** 1.1 Foundation / Calibration Draft  
**Status:** Framework and source-workspace database templates built; not approved for live assessment deployment.

## Files

- [00 Master Prompt](00_MASTER_PROMPT.md) — portable assistant instructions.
- [SKILL.md](SKILL.md) — import-ready Notion Agent Skill; no source workspace IDs.
- [01 Core Skill](01_CORE_SKILL.md) — expanded reusable workflow reference for five modes.
- [02 Notion Installation Guide](02_NOTION_INSTALLATION_GUIDE.md) — independent-workspace setup.
- [03 Acceptance and Calibration Tests](03_ACCEPTANCE_AND_CALIBRATION_TESTS.md) — test cases and release gates.
- [04 Synthetic Qualification Pack](04_SYNTHETIC_QUALIFICATION_PACK.md) — fictional benchmark fixture; not an NCFE source.
- [05 Adopter Source Intake](05_ADOPTER_SOURCE_INTAKE.md) — qualification/policy intake and release gate.
- [06 Notion Database Schema](06_NOTION_DATABASE_SCHEMA.md) — five adopter-owned database templates.
- [07 Mode Output Templates](07_MODE_OUTPUT_TEMPLATES.md) — structured output for all five operating modes.
- [MANIFEST.md](MANIFEST.md) — package inventory and validation status.
- [08 Portable Installation Prompt](08_PORTABLE_INSTALLATION_PROMPT.md) — copy/paste setup wizard for ChatGPT + the adopter's own Notion connection, with Custom GPT and Notion Agent fallback routes.

## Five modes

ASSESS · IQA REVIEW · RESUBMISSION · COMPARE · VIDEO ASSESS

## Separation

This project is independent from:
- NCFE Assessment Master Prompt Version 2 (historical source; reconstructed, not verbatim).
- NCFE Professional Assessment & Quality Assurance System — Modular Edition 1.0.

Do not merge project histories or modes without an explicit decision.

## Installation

Start with [08 Portable Installation Prompt](08_PORTABLE_INSTALLATION_PROMPT.md), then use the Notion Installation Guide. Every adopter must connect their own Notion workspace and create/map databases locally. The prompt guides setup but cannot grant permissions or provision account features by itself. Source workspace IDs, permissions, records and learner evidence are not dependencies.

## Platform availability notes

ChatGPT Notion MCP is a connection for the adopter's own ChatGPT account; do not assume it is automatically available inside every Custom GPT. GPT creation is unavailable on personal ChatGPT Free, Go, Plus and Pro accounts as of the current platform documentation; eligible Business, Enterprise and Edu workspaces may create GPTs subject to workspace settings. A Custom GPT that needs Notion must use an app actually supported in its GPT configuration or a separately configured, secure GPT Action. Notion Custom Agent MCP connections are plan- and admin-dependent.

## Critical limitations

The original Version 2 wording was not recovered verbatim. This project is a controlled reconstruction from preserved history. The synthetic qualification pack is fictional. No real qualification-specific source pack has been loaded. Independent human assessor/IQA benchmark testing and a second-workspace installation test remain outstanding.

The agent is decision support only. It must not invent criteria, policies, evidence or observations; authorised humans retain final assessment and IQA responsibility.
