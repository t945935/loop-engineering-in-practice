# Verifier and evidence checklist

Source: Appendix B of *Loop Engineering in Practice*, English edition. Checklist wording is retained; Markdown checkboxes are added for use.

## Acceptance contract

- [ ] The Goal, prohibited outcomes, and non-goals are explicit.
- [ ] Every acceptance condition maps to evidence.
- [ ] The contract was frozen and versioned before Action began.
- [ ] Tests, rules, and baselines are explicitly classified as protected or unprotected assets.
- [ ] Subjective decisions are assigned to a person instead of disguised as machine scores.

## Evidence binding

- [ ] Evidence includes the task ID, run ID, artifact digest, and contract version.
- [ ] The Checker verifies the current artifact, not an artifact from an earlier run.
- [ ] The report is reproducible or at least traces its inputs, environment, and rules.
- [ ] A hash identifies bytes and is not misrepresented as proof of correctness.
- [ ] External side effects are verified through a receipt and read-back, not only a tool's success response.

## Authority over completion

- [ ] The Maker may submit a claim but cannot write the verdict or approval.
- [ ] The Checker cannot silently modify protected rules.
- [ ] The Approver understands unchecked risks and evidence limitations.
- [ ] A change to the artifact automatically invalidates the old verdict.
- [ ] Irreversible action requires an explicit decision by a named accountable person.

## Verification record

Use the [verification report template](../templates/verification-report.yaml). Fill identifiers and evidence locations, then replace the template's list of verdict choices with exactly one actual verdict. An unchecked checklist or unfilled report is not a passing result.
