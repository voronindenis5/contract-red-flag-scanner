---
name: contract-red-flag-scanner
description: First-pass triage for contracts you're about to sign — 20+ high-risk clause detectors.
version: 1.0.0
author: Denis Voronin
license: MIT
tags: [contracts, legal, lease-review, consumer-protection]
---

# Contract Red Flag Scanner

**Before you sign a lease, job offer, or subscription — know what's hiding in the fine print.**

Scans plain contract text for 20+ high-risk clause patterns: auto-renewal traps,
rent acceleration, arbitration/class-action waivers, one-sided fees, non-competes,
unilateral amendments. Infers contract type, risk-ranks findings (HIGH/MEDIUM/LOW)
with the exact matched language in plain English, checks for MISSING protections,
and generates the question list to ask before signing.

## Quick Start
```bash
python3 scripts/contract_scanner.py scan contract.txt
python3 scripts/contract_scanner.py list-detectors
```

## Output
Risk-ranked findings with quoted contract language + plain-language explanation +
negotiation question per finding + missing-clause checklist + scrutiny score 0-100.

100% offline, pure stdlib. Not legal advice — triage that tells you whether you
need a lawyer and exactly what to ask.
