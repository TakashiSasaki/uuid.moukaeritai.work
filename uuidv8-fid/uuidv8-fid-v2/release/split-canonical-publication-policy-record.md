# Split-Canonical Publication Policy Record

This document is non-normative and does not declare a final release.

Split-Canonical Publication Simplification: This document records the shift from a dual-form publication candidate policy to a split-canonical publication policy.

| Item | Previous candidate state | New policy | Notes |
| :--- | :--- | :--- | :--- |
| Publication Model | Dual-form publication candidate | Split-canonical maintained publication | The split files are the canonical source and the only maintained publication form. |
| Single-file Artifact | Exactly one committed generated single-file artifact | No generated single-file Markdown artifact is maintained in the repository | A single-file document may be generated on demand using `tools/assemble_single_file.py`. |
| Assembly Tooling | Used to verify the generated artifact | Remains available for on-demand local generation | It is a local convenience tool. |
| Release Status | Undeclared | Final release remains undeclared | This repository state does not declare a final release. |

Reason for the policy shift: To avoid duplicated-maintenance and stale generated artifact risk.
