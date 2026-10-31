# OMNIS Evaluation Kit

Sealed external evaluation framework for AI governance and foresight claims.

## Purpose

This repository holds frozen evaluation criteria, raw outcome data, and independent scoring instructions. The design goal: an outside party can score claims without access to the system's internal analysis, conclusions, or reasoning traces.

## Structure

- `criteria/` — Frozen scoring rules and pass/fail thresholds. Locked before any outcome is observed.
- `raw-data/` — Unprocessed inputs and results. No analysis, no commentary.
- `scoring/` — Mechanical scoring instructions for an independent evaluator (human or AI).
- `evaluator/` — Instructions for the external scorer: what they may see, what they must not see, how to report.
- `results/` — Append-only scored outcomes. Nothing here rewrites criteria or data.

## Rules

1. Criteria are sealed with a timestamp before outcomes are known.
2. Raw data is recorded as-is. No retroactive cleaning.
3. The evaluator receives criteria and raw data only — never the system's own analysis.
4. Scores are appended, never edited. A failed test stays visible.
5. Any change to sealed criteria voids the seal for that evaluation round.

## Status

Initial structure. Criteria and data to be added per evaluation round.