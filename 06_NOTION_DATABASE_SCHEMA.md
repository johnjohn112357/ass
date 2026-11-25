# Notion Database Template Specification

The source Notion project contains five adopter-facing databases. Recreate them in the adopter's own workspace or map them to existing databases. Database/page IDs from the source project are examples only and MUST NOT be reused.

| Database | Purpose | Core properties |
|---|---|---|
| Qualification & Source Register | Versioned source documents and authority status | Source title (title), Source type (select), Awarding organisation, Qualification number, Version, Publication date, Applicable cohort, Authority status (select), Source URL, File, Verified by human (checkbox), Verification notes |
| Units & Assessment Criteria Register | Exact source-linked criteria | Criterion reference (title), Qualification, Unit or component, Learning outcome, Exact criterion wording, Source version, Source location, Evidence conditions, Decision vocabulary, Human verified, Status |
| Learner Evidence Register | Evidence provenance and access classification | Evidence item (title), Learner pseudonym, Qualification and unit, Evidence type (select), File or URL, File attachment, Version, Submitted date, Source location, Authenticity status (select), Access classification (select), Notes |
| Assessment & IQA Records | Provisional decisions and human sign-off audit | Record ID (title), Learner pseudonym, Qualification and unit, Mode (select), Assessment stage (select), Date, Source versions, Evidence versions, Provisional outcome (select), Human verified, Human sign-off status (select), AI limitations and caveats, Record URL |
| Calibration Test Register | Controlled tests and release gates | Test case (title), Test category (select), Input fixture, Expected behaviour, Observed result, Pass status (select), Severity if failed (select), Benchmark reviewer, Run date, Evidence or notes |

## Configuration rules

- Fetch the actual data source schema before writing. Use exact property names, option values and relations.
- If importing into a different Notion workspace, create new databases there. Do not rely on source workspace IDs or cross-workspace relations.
- Use pseudonymous learner identifiers; classify learner evidence as restricted by default.
- Keep source versions and evidence versions as explicit text/version metadata and preserve underlying files or stable links according to local policy.
- A criterion row is not usable for live assessment until exact wording and source location have been human-verified.
- A source marked Controlling requires a human applicability check for the learner's cohort.
- Keep AI output provisional. Human sign-off is a distinct field and cannot be set merely because the agent generated an assessment.
