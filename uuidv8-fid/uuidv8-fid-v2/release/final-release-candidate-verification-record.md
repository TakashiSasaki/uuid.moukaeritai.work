# Final Release Candidate Verification Record

This document is strictly non-normative.
This document does not declare a final release.

## Execution Record

| Command | Status | Exit code | Warning status | Notes |
|---|---|---|---|---|
| `python uuidv8-fid-v2/tools/assemble_single_file.py --check` | pass | 0 | none |  |
| `python uuidv8-fid-v2/tools/assemble_single_file.py --stdout > /tmp/uuidv8-fid-v2-single-file.md` | pass | 0 | none |  |
| `python uuidv8-fid-v2/tools/test_assemble_single_file.py` | pass | 0 | none |  |
| `python uuidv8-fid-v2/tools/check_consistency.py` | pass | 0 | none |  |
| `python uuidv8-fid-v2/tools/check_consistency.py --fail-on-warnings` | pass | 0 | none |  |
| `python uuidv8-fid-v2/tools/test_check_consistency.py` | pass | 0 | none |  |
