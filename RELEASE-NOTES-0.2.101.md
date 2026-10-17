# RoweMod Studio 0.2.101 beta — complete operation diagnostics

Send to Rowe now leads with the current operation: random installation/run IDs, last exact progress message and duration, running Studio version, executable/assembly files on disk, helper hashes and complete redacted exception chain. Historical errors remain separately labeled. A retry links to the previous failure and records its own outcome.

Failed sends retain the exact redacted payload and receipt ID in the local diagnostics outbox. Reopening the report control offers Retry saved report for the same operation. Green success requires a matching server acknowledgement. Oversized reports remain saved locally and are explicitly refused instead of silently dropping the beginning of the error.

The owner/admin reporting service adds direct ID-based report tools, bounded text reads with explicit continuation offsets and full-report checksum/length verification. Public visitors cannot read these reports. Existing private full-text downloads remain available. Reports remain diagnostic text only; no artwork or model files are uploaded.

Includes the 0.2.100 Unreal access-denied fix and 0.2.99 hair export fix. Tests cover controlled failures, full exception chains, retry linkage, redaction, durable failed delivery, restored retry controls, unauthorized reads and complete Unicode report reconstruction. One's real updated retry remains pending; no friend-PC success is claimed.

Update through Settings → Check for updates. Close Studio, Unreal and the game normally to apply it; then retry Build & launch and press Send to Rowe if it fails.
