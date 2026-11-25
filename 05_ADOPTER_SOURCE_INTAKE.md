# Adopter Source Intake and Release Gate

## Workspace isolation

Create and use databases only in the adopting organisation's own Notion workspace. Do not copy source creator learner records, credentials, permissions or workspace IDs. Keep learner evidence restricted by default and follow local retention, access and deletion rules.

## Required local databases

1. Qualification & Source Register
2. Units & Assessment Criteria Register
3. Learner Evidence Register
4. Assessment & IQA Records
5. Calibration Test Register

The adopter may rename or map these to existing databases, but must inspect the actual schema before writing. Do not assume imported properties or relations exist.

## Intake order

1. Record exact qualification title and number.
2. Obtain the specification/handbook applicable to the learner's registration and assessment date; confirm version and effective date.
3. Confirm learner cohort/registration and applicability.
4. Obtain the unit/component document and complete learning outcomes and assessment criteria.
5. Obtain the actual assignment/assessment brief and amendments.
6. Obtain relevant centre policies: assessment, authenticity, reasonable adjustments/access arrangements, appeals, malpractice, safeguarding where relevant, and IQA.
7. Record title, issuer, version, publication/effective date, cohort, exact page/section and URL/file.
8. Mark a source Controlling only after a human has verified applicability. Until then mark Unverified.
9. Enter criterion wording verbatim, with source location and conditions. A second person should verify transcription before decisions use it.
10. Add evidence as versioned records with pseudonymous learner IDs and provenance.

## Conflict handling

If two sources conflict, do not choose the newer source by default. Determine applicability to the learner's cohort and document the conflict. If the controlling source cannot be established, stop the affected criterion decision and request authorised clarification.

## Evidence intake

Record file/link, version, submission date, evidence type, source location (page/paragraph/timestamp), authenticity-check status and access classification. Store minimum personal data. Do not treat a learner's written description as proof of practical performance unless the criterion permits that evidence form.

## First-run validation

Run the synthetic fixture in `04_SYNTHETIC_QUALIFICATION_PACK.md`. It is a reasoning test only and must never be uploaded as an NCFE specification or used for learner assessment. Then run adopter-approved anonymised cases and compare with an authorised human assessor/IQA benchmark. Record disagreements and causes.

## Release gate

Do not use for live learner decisions until all conditions are met:

- Qualification and cohort applicability checked.
- Source documents and criteria human-verified.
- Centre policies loaded and access controlled.
- All critical calibration tests pass.
- Major disagreements resolved and documented.
- Assessor and IQA roles approve the workflow.
- Human sign-off and retention process is clear.

## Failure response

If a source, file, video, database or permission cannot be accessed, say so. Do not imply it was inspected. Use Unable to determine where the missing item affects the decision.
