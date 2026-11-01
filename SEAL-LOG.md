# Seal Log

Append-only record of when criteria were sealed. Each entry is immutable.

| Round | Criteria File | Sealed (UTC) | Hash |
|-------|-------------|--------------|------|
| | | | |
| BTC-PILOT-001 — EXPERIMENTAL / UNSCORED | [Frozen packet criteria reference](criteria/BTC-PILOT-001.md) | 2026-11-01T12:24:34Z — FreeTSA service assertion for packet bytes | Packet SHA-256 `ca65ba4ec2f30f3305dec477f2c5f462cb775e6dd5d4c0ae8b41f5824fd17e9e`; [signed receipt](timestamps/BTC-PILOT-001/RECEIPT.json) |

A later edit to any sealed criteria file voids that round's seal. Record the void here with date and reason.

Entry prepared at 2026-11-01T12:35:36.701170Z. This is a later record of an existing packet timestamp,
not a claim that this seal-log row or its later GitHub commit existed at that time.
The timestamp covers the exact packet, not this reference file or any old template.
Immutable release and independent registration remain pending; outcomes are UNSCORED.
