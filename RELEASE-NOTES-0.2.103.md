# RoweMod Studio 0.2.103 beta — saved MetaHuman groom inspection

Fixes the hair-export failure `SpawnMetaHumanActor ... not added for editing`, followed by `The saved character groom components could not be inspected`. Studio now registers the saved source character for editing before creating its transient groom-inspection actor.

All generic groom names share one inspection session. Studio destroys its temporary actor and releases only the editing registration it created. Existing editor registrations remain owned by their original session. Registration, spawn, lookup and cleanup failures retain the original diagnostic and preserve saved artwork.

Twelve focused tests cover registration order, refusal, actor failure, existing editor ownership, ambiguous names, cleanup and shared lookup. The Unreal 5.8 API contract is checked against the installed editor headers. Native Cameron export and One's updated retry remain pending; this release does not claim completed character export or gameplay acceptance.

Use Settings → Check for updates. Studio applies ready updates when idle; the updater waits for the game and Unreal to close. Reopen your saved Cameron character and retry Build & launch. Send to Rowe if a new failure occurs.
