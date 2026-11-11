# Retry, fallback, and circuit breaker worksheet

Source: Appendix D of *Loop Engineering in Practice*, English edition. Failure-classification and circuit-breaker tables are retained; retry decisions use fill-in checkboxes.

## Failure classification

| Question | Entry |
| --- | --- |
| Error fingerprint | |
| Failure class | transient / permanent / policy / unknown |
| Side-effect certainty | not_started / none / applied / unknown |
| New information or changed condition | |
| Attempts and deadline remaining | |
| Idempotency or reconciliation method | |

Select one class and one side-effect certainty value for the observed attempt. Do not treat the alternative values as an observed result.

## Retry decision

- [ ] Create a new attempt for the same task instead of inventing new work.
- [ ] The next attempt has explainable new information or a changed condition.
- [ ] The operation deadline, attempt cap, and Budget all permit another attempt.
- [ ] An uncertain side effect is queried or handed to a person instead of being blindly resubmitted.
- [ ] Backoff is capped and includes jitter.

## Fallback contract

Complete the [fallback contract template](../templates/fallback-contract.yaml). Its `approval_required: false` is the source template value, not approval for a real operation: explicitly decide this field for the task before use.

## Circuit breaker

| Field | Setting |
| --- | --- |
| Dependency or operation scope | |
| Qualifying failure | |
| Window and threshold | |
| Open behavior | |
| Cooldown | |
| Half-open probe limit | |
| Closing condition | |
| Human-handoff condition | |

Do not invent successful retries, known side effects, or a closed circuit breaker without the corresponding observations.
