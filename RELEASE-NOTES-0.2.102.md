# RoweMod Studio 0.2.102 beta — automatic update restart and editor close

When automatic updates are enabled and a verified update has finished downloading, Studio closes normally and reopens through the updater. Active tasks, painting and setup dialogs defer that restart. The updater still waits for the game and Unreal to close before replacing shared runtime files; it does not interrupt an active match.

Build & launch now requests a normal close of open Unreal Editor windows when the saved MetaHuman must be copied. Unreal's Save/Cancel prompts remain active; a refused close leaves the build waiting. Studio never kills Unreal. Windows privilege restrictions produce a clear instruction to close the editor normally instead of crashing.

Includes the per-operation diagnostics and durable reporting in 0.2.101, the access-denied repair and generic groom export fix. Validation: 38 reporting/restart checks, 10 Windows editor lifecycle checks and an actual previous-version archive upgrade. One's own updated build/gameplay test remains pending.
