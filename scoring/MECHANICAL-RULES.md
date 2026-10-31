# Mechanical Scoring Rules

For the independent evaluator. Apply in order. Do not skip steps.

1. Read `criteria/` for the round under test. Note the seal timestamp.
2. Read `raw-data/` for the same round. Confirm the data timestamp is after the criteria seal.
3. Check each pass condition against the raw data only.
4. Check each fail condition. Any single fail = FAIL for the round.
5. Record the result in `results/` as an append-only entry.
6. Do not read, reference, or request the system's internal analysis, reasoning traces, or prior self-assessments.
7. If a required input is missing, the round is UNSCORED, not passed.

## Output Format

```
Round: [number]
Date scored: [YYYY-MM-DD]
Result: PASS / FAIL / UNSCORED
Conditions met: [list]
Conditions failed: [list]
Missing inputs: [list]
Scorer: [name or model]
```