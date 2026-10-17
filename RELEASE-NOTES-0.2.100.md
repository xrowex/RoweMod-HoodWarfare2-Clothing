# RoweMod Studio 0.2.100 beta — Unreal process check repair

Fixes `Access is denied` while Build & launch waits for Unreal to close. Studio now uses the Windows process snapshot without opening each editor's process handle. A detected editor still keeps the build waiting; its exit is picked up by the next check. No administrator launch is required by this fix.

Includes 0.2.99's generic MetaHuman groom-name fix, event-driven cosmetics and character-specific outfit workflow. Saved projects and artwork are preserved.

Validation: the built process-check method is exercised against a real Windows editor-named process and its exit. The exact release ZIP is checked with the previous Studio updater. One's own build retry remains required; this release does not establish friend-PC or two-PC gameplay acceptance.

Use Settings → Check for updates, then close Studio, Unreal and the game normally so the update can apply. Retry Build & launch afterward.
