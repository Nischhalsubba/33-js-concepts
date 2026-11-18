# Writing reliable JavaScript concept lessons

The value of a learning example comes from a **reproducible explanation**: a reader should be able to predict its output, run it, understand why it behaves that way, and identify where the claim stops applying.

## Suggested lesson structure

Each changed or new lesson should contain:

1. **Question:** a specific JavaScript behavior, not a broad keyword.
2. **Mental model:** the minimal rules a learner needs, with jargon explained.
3. **Executable example:** the smallest self-contained snippet that demonstrates the concept.
4. **Expected output:** explicit values or observable browser effects, with any asynchronous order stated carefully.
5. **Explanation:** why the behavior follows from the rules, including relevant types, scopes and coercions.
6. **Counterexample:** one nearby case that changes the result and reveals a boundary condition.
7. **Try it:** an exercise that asks the reader to predict the result *before* running it.
8. **References:** authoritative specifications or accurate runtime documentation as appropriate.

Avoid example titles that promise universal behavior when browser and Node runtimes differ.

## Correctness and portability checklist

- Identify the environment: Node, browser, ES module, classic script or strict mode where it matters.
- Declare the supported runtime/version if behavior depends on it.
- Use distinct variables and clearly named functions; no hidden globals or unexplained side effects.
- Verify the shown output by actually running the example; mark illustrative output as illustrative.
- Distinguish integer precision, floating-point limitations, \`NaN\`, signed zero and \`undefined\` where applicable.
- For promises/timers, do not assert deterministic interleavings that the runtime does not guarantee.
- For equality and coercion, explain relevant operand types before drawing conclusions.
- Do not reproduce a long proprietary tutorial; write original explanations and attribute sources.
- Keep educational additions isolated so a learner can run a single snippet without unrelated dependencies.

## Repository-specific verification

The teaching material is under \`study/\`, and the maintained package exposes a narrow syntax test. From the repository root:

~~~bash
cd study
npm test
~~~

That command runs \`node --check index.js\`. It does **not** validate every concept lesson or the truth of example output. Test any new standalone snippet directly in its documented environment, and record the runtime, command and output in the PR.

## PR review template

- Concept and intended learner level
- Before/after problem solved
- Linked paths and original sources where useful
- Runtime(s) actually tested
- Command and observed output
- Counterexample and common misconception addressed
- Remaining limitations

## Review and rollback

Prefer one conceptual correction per PR, with a clear diff and an example a reviewer can rerun. If a lesson makes a false claim, correct or revert that focused example without obscuring its prior context.
