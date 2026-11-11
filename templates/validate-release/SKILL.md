---
name: validate-release
description: Validate a release artifact and produce a bounded report.
---

1. Resolve the exact artifact path.
2. Record its digest and validation policy version.
3. Run deterministic checks.
4. Save pass, fail or inconclusive with evidence locations.
5. Never publish or overwrite the artifact.
