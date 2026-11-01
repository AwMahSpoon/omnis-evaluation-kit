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

## Experimental Bitcoin pilot 001

See the [fixed criteria reference](criteria/BTC-PILOT-001.md),
[seal-log entry](SEAL-LOG.md), [frozen packet](packets/BTC-PILOT-001-2026-11-01.zip)
and [timestamp verification](timestamps/BTC-PILOT-001/VERIFY.md).
The packet is assistant-prepared and independently timestamped. This repository
entry does not establish predictive advantage, an immutable release or completed
independent registration. Outcomes remain UNSCORED until resolved under frozen rules.
