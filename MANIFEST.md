# Manifest — Edition 1.1 Foundation / Calibration Draft

- 00_MASTER_PROMPT.md
- SKILL.md
- 01_CORE_SKILL.md
- 02_NOTION_INSTALLATION_GUIDE.md
- 03_ACCEPTANCE_AND_CALIBRATION_TESTS.md
- 04_SYNTHETIC_QUALIFICATION_PACK.md
- 05_ADOPTER_SOURCE_INTAKE.md
- 06_NOTION_DATABASE_SCHEMA.md
- 07_MODE_OUTPUT_TEMPLATES.md
- README.md

Deployment design:
- Default path: ChatGPT conversation connected to the adopter's own Notion workspace through Notion MCP.
- Optional path: Custom GPT only where account/workspace creation rights and a supported Notion app or separately configured secure Action are available.
- Optional path: Notion Skill / Custom Agent where the adopter's Notion plan and admin settings support it.
- Prompt does not grant permissions, provision account features, or create a GPT automatically.

Validation:
- Import-ready Skill frontmatter: cleaned; source Notion page ID removed.
- Source-workspace Notion database templates: created (five).
- Synthetic benchmark fixture: created; fictional only.
- Mode-specific output templates: created (five).
- Starter calibration cases: 18 created; all Not run pending execution.
- Independent human assessor/IQA benchmark: not completed.
- Second-workspace installation: not tested.
- Live assessment release: NOT APPROVED.
