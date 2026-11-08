# Final 50-unit cohort results

All 50 independent raw re-audits passed. All 11 blocks completed with cleanup and independent final absence checks passed.

| Study | Arm | Condition | Units | Units with wrong response | Final ten correct | Wrong slots | Unavailable slots |
|---|---|---|---:|---:|---:|---:|---:|
| fallback | FM | no_writer | 3 | 0 | 3 | 0 | 0 |
| fallback | VC-original | no_writer | 3 | 0 | 3 | 0 | 0 |
| fallback | VC-fallback | no_writer | 3 | 0 | 3 | 0 | 0 |
| fallback | FM | later_routing_writer | 3 | 3 | 0 | 201 | 37 |
| fallback | VC-original | later_routing_writer | 3 | 3 | 0 | 190 | 37 |
| fallback | VC-fallback | later_routing_writer | 3 | 3 | 0 | 193 | 36 |
| enforcement | FM-unprotected | routing_writer | 3 | 3 | 0 | 204 | 63 |
| enforcement | FM-enforced | routing_writer | 3 | 0 | 3 | 0 | 12 |
| enforcement | FM-unprotected | annotation_writer | 3 | 0 | 3 | 0 | 10 |
| enforcement | FM-enforced | annotation_writer | 3 | 0 | 3 | 0 | 10 |
| verification | 0 | normal_case | 5 | 0 | 5 | 0 | 30 |
| verification | 5 | normal_case | 5 | 0 | 5 | 0 | 34 |
| verification | 10 | normal_case | 5 | 0 | 5 | 0 | 35 |
| verification | 20 | normal_case | 5 | 0 | 5 | 0 | 35 |

Descriptive fixed cyclic block allocation, not randomization. Slots are repeated observations within units, not independent incidents. Observer whole-container CPU, executor invocation CPU and transport lifetime CPU have distinct boundaries; do not combine into pure guard CPU. No population or causal per-request claim.

All 50 units had zero compensation attempts. The fallback later-writer runs therefore do not demonstrate compensation effectiveness: their finite verification passed before the later wrong responses. Verification normal-case results establish sampled recovery, not continuous correctness.
