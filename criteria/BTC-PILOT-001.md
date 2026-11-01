# BTC-PILOT-001 — experimental prospective criteria

Status: LOCAL PROPOSAL; GitHub release and independent registration are pending.
Outcome status: UNSCORED. No independent evaluation or predictive edge is claimed.

## Frozen source of authority

The unchanged packet is [BTC-PILOT-001-2026-11-01.zip](../packets/BTC-PILOT-001-2026-11-01.zip).
Its exact SHA-256 is `ca65ba4ec2f30f3305dec477f2c5f462cb775e6dd5d4c0ae8b41f5824fd17e9e`.
The original METHOD.md version 1.0, complete forecast cards, source metadata,
baseline definitions and protocol inside that packet control resolution.
This later reference file does not replace or modify any frozen rule.

The [signed timestamp receipt](../timestamps/BTC-PILOT-001/RECEIPT.json)
records FreeTSA service time `2026-11-01T12:24:34Z` for the packet hash.
This reference file and its later GitHub commit are not themselves covered
by that earlier timestamp. A new seal is required if packet bytes change.

## Three fixed claims

Reference: Coinbase Exchange BTC-USD October 31, 2026 UTC candle close,
77,423.98 USD. Only each target day final UTC close counts; intraday touches
do not. Use Decimal comparison against the exact unrounded thresholds.

| Forecast | Target UTC day | Exact comparison in USD | Frozen p | Frozen baseline q |
| --- | --- | --- | --- | --- |
| WYS-F0001 | 2026-11-30 | > 77423.9800 | 0.535950 | 0.535633 |
| WYS-F0002 | 2026-12-31 | >= 85166.3780 | 0.349255 | 0.365573 |
| WYS-F0003 | 2027-01-30 | <= 61939.1840 | 0.176181 | 0.160516 |

## Resolution and evidence limits

Use the exact official source, fallback, seven-day reporting grace and
revision rules in each frozen card. All three outcomes remain future.
Missing source evidence is not automatically NO. Preserve every miss,
unresolvable case and correction. These are assistant-computed experimental
probabilities, not elicited personal probability judgments from Agent-8.

The questions share Bitcoin and overlapping horizons. Three entries
are not three independent trials. Scores may be reported descriptively;
there is no preregistered statistical threshold establishing an advantage.

The current method requires an immutable GitHub release plus independent
time-stamped registration, such as OSF. The additional FreeTSA signature
does not by itself complete either publication step. Keep fully issued
status pending until real receipts exist.

See [mechanical scoring](../scoring/BTC-PILOT-001.md) and
[verification commands](../timestamps/BTC-PILOT-001/VERIFY.md).
