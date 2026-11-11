# Token, time, and cost budget worksheet

Source: Appendix C of *Loop Engineering in Practice*, English edition. Tables are retained as fill-in worksheets.

Do not write only “control costs.” Put every dimension, stopping condition, and reserve in one worksheet.

## Action allowance

| Dimension | Used | Soft limit | Action hard limit |
| --- | --- | --- | --- |
| Elapsed time | | | |
| Active runtime | | | |
| Input tokens | | | |
| Output tokens | | | |
| Money | | | |
| Search or tool calls | | | |
| Human review minutes | | | |

## Closure and absolute limits

| Dimension | Closure reserve | Absolute limit | Action after exhaustion |
| --- | --- | --- | --- |
| Elapsed time | | | |
| Active runtime | | | |
| Input tokens | | | |
| Output tokens | | | |
| Money | | | |
| Search or tool calls | | | |
| Human review minutes | | | |

Before each expensive Action, complete the [next-action decision template](../templates/next-action-decision.yaml). Choose one information-gain label and one decision rather than retaining the template's alternatives.

Price, model, and provider-metering fields must include a verification date and policy version. Missing usage is unknown, never an invented zero.

Record alongside your completed sheet:

- Currency and units:
- Model and provider:
- Pricing source and verification date:
- Budget policy version:
- Accountable owner:

The empty fields are deliberately unfilled planning inputs, not recommended defaults.
