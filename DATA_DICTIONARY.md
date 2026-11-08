# Data dictionary

Policy names: SSA/native_ssa = native server-side apply; RSSA/known_read_set_ssa adds a known-object read set; KG/current_guard checks the approved backend contract; FM/full_membership_guard checks complete candidate membership; VC/full_membership_verify_compensate adds finite verification and conditional compensation. Final arms additionally distinguish VC-original/VC-fallback and FM-unprotected/FM-enforced.

## Original campaign
`attempted` and `complete` are campaign counts. `exposure_true` means at least one observed wrong business response; `exposure_unknown` retains unresolved exposure. `recovery_true` is the fixed final recovery endpoint; `recovery_unknown` retains unresolved recovery. False counts are attempted minus true minus unknown. Historical `campaign_recovery_unknown_original` preserves the original campaign classification before the logical endpoint refinement; it is not interchangeable with refined recovery. Status-count columns and the separate execution-status CSV describe execution dispositions, not independent recovery. All forty cells have ten attempts.

Later-writer `block` indexes matched cluster blocks. `correct_business`, `wrong_business`, `unavailable`, `unknown` partition 120 action slots per session. Unit IDs are research allocation labels, not infrastructure identifiers. Paired differences are VC minus FM within block.

## Normal-case costs
`block` identifies the matched block; `policy` identifies the arm. `metric` names the distinct wall-time, observer-window CPU, client-process CPU or reaped-child CPU measure. Values, baselines and paired differences are in seconds. Verification counts/RPC counts use their named count units. `paired_difference` is policy minus native-SSA baseline. Ratios are dimensionless; `ratio_reason` explains unavailable ratios and `pair_valid` records validity. Summary ranges and medians preserve five planned block pairs. The measures have distinct boundaries and must not be summed into pure guard CPU.

## Final 50-unit cohort
`unit_id`, `study`, `block`, `position`, `arm` and `condition` retain the original allocation. `correct_business`, `wrong_business`, `unavailable`, `unknown` partition 120 neutral action slots per unit; control receipts are not represented as separate CSV rows. `any_wrong_response` is the exposure endpoint; `final_ten_slots_correct` is a sampled response suffix, not a durable correctness guarantee or the full original campaign recovery endpoint. `compensation_attempts` is zero throughout this cohort. `verification_receipts` counts additional verification queries.

`observer_cpu_seconds` is whole-container observation CPU over the enrolled window; `executor_wall_seconds` is invocation wall time; `executor_cpu_seconds` is invocation-process CPU; `transport_lifetime_cpu_seconds` is persistent transport-process CPU. Boundaries differ and are not additive. JSON summaries group the retained rows. Final `PAIRED_COSTS` files contain arm-minus-baseline differences within block; negative differences do not imply a population speedup. Missingness is retained, not imputed as zero.
