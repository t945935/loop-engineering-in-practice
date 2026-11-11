# Loop Engineering in Practice — English Reader Downloads

Companion materials for **Loop Engineering in Practice: Designing Reliable AI Agent Loops with State, Verification, Budgets, and Safe Stops**.

**Author:** Happy eBook Author. **Publisher:** Happy eBook. **Companion package:** English, version 1.0.0.

This repository contains reusable planning templates, fill-in worksheets, and one illustrative State record from the English book. It does **not** contain the book, an EPUB/PDF, or an executable Agent runtime. No French translation is included.

## Download and start

On GitHub, select **Code → Download ZIP** for the current repository contents. Use the **Releases** page for any published versioned packages; do not assume a release exists merely because this document names a package version. You can also open the individual files below and use GitHub's Raw/Download action.

For the local versioned ZIP, extract it and open `README.md` in its top-level folder. No installation, API key, network upload, or paid service is needed to read and complete these materials.

1. Start with the [ten-minute Loop worksheet](worksheets/ten-minute-loop.md).
2. Copy the [core specification](templates/core-loop-spec.yaml) into your own task folder and fill it in.
3. Define acceptance and evidence with the [Verifier checklist](worksheets/verifier-evidence.md).
4. Set limits in the [budget worksheet](worksheets/budget.md) and the [retry/fallback/circuit-breaker worksheet](worksheets/retry-fallback-circuit-breaker.md).
5. Add the [governance extension](templates/governance-extension.yaml) when multiple Agents, real tools, public release, or high-impact decisions are involved.

## Included files and book locations

| Download | Book location | Purpose |
| --- | --- | --- |
| [Core Loop specification](templates/core-loop-spec.yaml) | Appendix A | Define work discovery, outcome, permissions, evidence, State, Budget, and stopping |
| [Governance extension](templates/governance-extension.yaml) | Appendix A | Assign responsibility for orchestration, tools, outcomes, incidents, and lifecycle |
| [Ten-minute worksheet](worksheets/ten-minute-loop.md) | Appendix A | Answer seven minimum control questions |
| [Verifier and evidence checklist](worksheets/verifier-evidence.md) | Appendix B | Bind acceptance and authority to current evidence |
| [Verification report](templates/verification-report.yaml) | Appendix B | Record an actual verdict and its evidence |
| [Budget worksheet](worksheets/budget.md) | Appendix C | Define action allowances, closure reserve, and absolute limits |
| [Next-action decision](templates/next-action-decision.yaml) | Appendix C | Decide whether the next expensive action is justified |
| [Retry/fallback/circuit-breaker worksheet](worksheets/retry-fallback-circuit-breaker.md) | Appendix D | Classify failure and bound continuation |
| [Fallback contract](templates/fallback-contract.yaml) | Appendix D | Record changed guarantees and approval requirements |
| [Project-rule example](templates/project-rules/AGENTS.md) | Appendix E | Illustrate project scope, validation, and human approval boundaries |
| [Release-validation skill example](templates/validate-release/SKILL.md) | Appendix E | Illustrate a bounded validation process |
| [Minimum State example](examples/state/minimum-state.json) | Appendix E | Illustrate external progress and artifact references |

## What these files prove — and what they do not

- The YAML, Markdown, and JSON are companion documents, not an implementation of a reliable Loop. Parsing a file does not execute its policy or prove a real task passed.
- Empty template fields are inputs you must decide. Strings such as `pass | fail | inconclusive` enumerate choices; replace them with one justified result when completing a record.
- The State example's IDs, timestamps, paths, `status`, and `sha256: "..."` are illustrative source values. They are not evidence of a real run or a real artifact digest. Compute and record your own values before operational use.
- `approval_required: false` in the source fallback template is not permission for your task. Decide the actual approval policy before execution.
- An `AGENTS.md` or `SKILL.md` file is not a sandbox, permission lock, or automatically installed integration. Read your tool's own loading rules before copying it into a project. Only the explicitly named sample under `templates/project-rules/` is a project-rule example.
- Keep design, tabletop exercises, runtime evidence, and human approval distinct. Never relabel a template or an expected answer as a successful runtime observation.

The book mentions additional `examples/...` programs. Their original source was not present in the supplied EPUB or located in the inspected local sources, so they are **not included** and have not been recreated under the same names. This package does not claim to deliver or rerun those programs.

## Questions and corrections

Use GitHub **Issues → New issue** for a reader question or correction. Include the book language/version and chapter/subsection; page numbers are optional because reflowable ebooks differ by device. Report expected and observed behavior, and include a minimal example when relevant. We do not promise a fixed response time.

See [contribution and privacy guidance](CONTRIBUTING.md). Do not submit credentials, personal data, a whole private project, or the full book.

## Provenance and rights

[SOURCE_MAP.json](SOURCE_MAP.json) maps every companion file to its source section and records the exact input EPUB's SHA-256. Worksheets add layout and reader-use guidance; eight preformatted source blocks are preserved verbatim apart from final-newline normalization. This digest identifies the inspected input bytes, not all copies of the edition and not proof of correctness.

Read [RIGHTS.md](RIGHTS.md) before redistribution. No blanket MIT or Creative Commons license is asserted. See [CHANGELOG.md](CHANGELOG.md) for package changes.
