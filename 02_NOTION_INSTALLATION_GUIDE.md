## Purpose

This guide enables another educator to install the NCFE Assessor Agent in their own Notion workspace and connect it to Notion AI or an external assistant through supported Notion MCP access.

**Each adopter must use their own workspace.** This source project is a template only. No source workspace page ID, database ID, permission, credential or learner record should be reused.

## What the adopter needs

- A Notion workspace with permission to create pages/databases and manage Skills.
- Notion AI/Agent access if using the Skill inside Notion; availability depends on plan and workspace settings.
- For external assistants, a supported Notion MCP integration authenticated to their own workspace.
- Master Prompt, import-ready Skill and supporting templates.
- Applicable qualification specification, unit criteria, assessment brief and centre policies.
- An anonymised evidence set for calibration.

## Installation paths

### A. Notion Agent / Notion Skills

1. Import `SKILL.md` (or the packaged Skill archive) into the adopter's own Notion workspace using Notion's Skills import workflow.
2. Confirm the imported page is designated as a Skill and its name/description are correct.
3. Enable the Skill for Notion Agent.
4. Enable automatic use only if desired.
5. Enable connected-agent/MCP use if supported and required.
6. Test with anonymised sample evidence; verify that missing criteria are requested rather than invented.

### B. External AI assistant with Notion MCP

1. Connect the assistant to the adopter's own Notion workspace using its supported Notion MCP/connector flow.
2. Authenticate as the adopter; never use another person's token or workspace.
3. Import the Skill and enable it for connected agents.
4. Add `00_MASTER_PROMPT.md` to the assistant's supported project/instruction configuration. A Skill alone is not a replacement for the full master prompt where platform instructions are available.
5. Grant access only to qualification and evidence records required for the task.
6. Verify read and write access separately. Read-only is preferable during initial calibration.
7. Confirm records are written only to the adopter's workspace.

### C. No Notion connection

Use the Markdown Master Prompt and Skill in a supported AI project/chat. Database automation will not work; the assistant must return copy-ready records in chat and must not claim that anything was saved to Notion.

## Recommended database templates

The five database schemas are specified in `06_NOTION_DATABASE_SCHEMA.md`:

1. Qualification & Source Register
2. Units & Assessment Criteria Register
3. Learner Evidence Register
4. Assessment & IQA Records
5. Calibration Test Register

Create them in the adopter's own workspace or map existing databases. Fetch each actual schema before creating records; do not assume example columns exist.

## Qualification source onboarding

Use the ordered workflow in `05_ADOPTER_SOURCE_INTAKE.md`. Confirm the exact specification applicable to the learner's cohort and assessment date, complete unit criteria, assessment brief and local policies. Record versions and source locations. If applicability cannot be established, stop qualification-specific decisions.

## First-run calibration

Use the synthetic fixture in `04_SYNTHETIC_QUALIFICATION_PACK.md`, then adopter-approved anonymised cases. The synthetic fixture is fictional and is not a qualification source. Test normal evidence, missing criteria, conflicting versions, practical evidence, resubmission, IQA over-assessment, video limitations, authenticity concerns, privacy and write permissions.

Compare outputs with an authorised human assessor/IQA benchmark. Record input, full output, expected behaviour, observed result, reviewer, Skill/prompt version and corrective action. A self-review by the model is not an independent benchmark.

## Privacy and access controls

- Keep learner evidence and assessment records private by default.
- Use pseudonymous identifiers where feasible.
- Avoid uploading unnecessary personal data.
- Do not enable public links for learner evidence.
- Do not change permissions or invite collaborators without explicit approval.
- Follow centre retention, access, data-protection and incident procedures.

## Completion checklist

- [ ] Own Notion workspace connected.
- [ ] Skill imported and enabled.
- [ ] Connected-agent access enabled where required.
- [ ] Master Prompt installed.
- [ ] Five databases created or mapped.
- [ ] Qualification source and cohort verified.
- [ ] Centre policies imported.
- [ ] Evidence access restricted.
- [ ] Critical calibration tests passed.
- [ ] Human assessor/IQA benchmark review completed.
- [ ] Human sign-off process documented.
- [ ] No dependency on source creator workspace remains.

**Release status:** Foundation draft. The project databases and fixtures have been created in the source workspace, but second-workspace installation and independent human benchmark validation have not been completed.
