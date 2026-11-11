# Ten-minute Loop specification worksheet

Source: Appendix A, “Ten-minute minimum version” of *Loop Engineering in Practice*, English edition.

Use this worksheet to make a decision about a real task. Empty answers do not authorize automation. Record the accountable person and stop when a safety boundary is unresolved.

1. **How does work appear, and what counts as the same task?**
   - Your answer:
2. **What observable outcome must actually change?**
   - Your answer:
3. **What may the Agent do, and what must it never do?**
   - Your answer:
4. **What external evidence can prove completion?**
   - Your answer:
5. **Where is progress stored, and how are stale writes rejected?**
   - Your answer:
6. **What are the maximum time, token, monetary, and tool-call costs?**
   - Your answer:
7. **Which conditions require the Loop to stop, and who receives the handoff?**
   - Your answer:

Then complete the [core Loop specification](../templates/core-loop-spec.yaml). Add the [governance extension](../templates/governance-extension.yaml) for multiple Agents, real tools, public release, or high-impact decisions.

The source's rule remains in force: if a field is unresolved, convert it into a prohibition on automation or a human handoff. Do not leave it for the Agent to guess during execution.
