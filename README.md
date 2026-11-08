# SafeAgentOps research results

Supporting data for **Guard Coverage and Finite Verification in Kubernetes Service Repair**, by Manpreet Singh Sachdeva and Ratan Deep Singh. Prepared for IEEE Transactions on Network and Service Management submission. No acceptance or publication is claimed.

This is a public results-only derivative of the private SafeAgentOps research repository. It includes aggregate and per-unit result tables; it does not include experiment runners, raw journals, cloud credentials, infrastructure identifiers, the manuscript, or private Git history. No DOI has been assigned.

## Cohorts

- `original-campaign/`: 400 attempted sessions in ten blocks, 398 campaign-complete and two incomplete. Forty policy/condition cells retain true/false/unknown endpoints. The 20 later-writer FM/VC sessions form ten original pairs and are a subset of these 400 attempts, not additional experiments.
- `normal-case-cost/`: separate 25-session matched normal-case cost cohort; five blocks and five policies. Differences are within-block policy-minus-native-SSA; they are whole-workflow measures, not pure guard latency.
- `final-cohort/`: separate prospectively frozen 50-unit GKE cohort: fallback 18, enforcement 12, verification 20 across 11 fresh lifecycles. All 50 independently re-audited; all blocks passed cleanup and independent final resource-absence checks. All 50 units had zero compensation attempts.

Do not pool the denominators. Slots are dependent within-session observations, not independent incidents. Fixed cyclic ordering is not randomization. Results concern a bounded synthetic selector-fault family on a single-node fixture and do not establish production prevalence, durable safety or general agent superiority.

## Files and use

CSV files can be opened in a spreadsheet or standard CSV reader. JSON files provide grouped descriptive summaries. `DATA_DICTIONARY.md` describes fields and scope. `PROVENANCE.json` records source-relative names and byte hashes; the original source evidence remains private. These tables support inspection and recomputation of reported summaries but are not a complete raw-evidence reproduction or executable experiment package. Pilot, engineering and exploratory timing cohorts are outside this deposit.

All data files are byte-identical copies of the listed source result tables. No unfavorable rows or incomplete-attempt counts were removed. Source experiment inputs, allocations, receipts and runtime freezes remain unchanged. The public repository's Git history begins with this derivative; private history is not copied.

Copyright 2026 Manpreet Singh Sachdeva and Ratan Deep Singh. Public access is provided; no additional software or data reuse license is granted by this deposit.
