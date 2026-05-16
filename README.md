# aisbom-action-e2e

End-to-end test repo for the [AIsbom GitHub Action](https://github.com/Lab700xOrg/aisbom).

Each PR scans the `models/` directory (which contains intentionally malicious
mock artifacts from `aisbom generate-test-artifacts`) and posts a single
idempotent comment summarizing findings. Re-running the workflow updates the
existing comment in place — proving the marker-based idempotency works.

