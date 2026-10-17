# RoweMod Studio 0.2.99 beta — hair export and event-driven runtime

Fixes MetaHuman builds that stop with `The assembled groom slot is not recognized: GroomAsset_0`. Generic groom names now resolve from the saved character's named hair, eyebrow, eyelash, beard, mustache and peach-fuzz components. Ambiguous matches stop with an error instead of assigning the wrong slot. Six focused checks pass; One's own retry remains required.

Universal/modular clothing was canceled. Outfits are fitted manually to one selected character.

- Creation starts with a character. Its Blender outfit kit contains one rig and green body references.
- Saved outfit kits reject imports into a different character or slot.
- Automatic body fitting, shared clothing builds and uploads, multi-character download selection, and the in-game clothing switching panel are retired.
- Current character parts are sent directly to the runtime; historical garment versions are preserved without being mounted as a clothing catalog.
- Existing projects, artwork, textures and installed packages are preserved. Gloves remain excluded.

The local build passes 105 workflow, paint, reset, tattoo and clothing-color checks. Aqua's actual kit saves and reopens with one rig; matching import succeeds, and mismatched character/slot imports are rejected. Its existing shirt requires manual weight transfer before a new build.

Native game acceptance is recorded separately in cache/verification/character-outfit147-native-play01. These checks do not establish every outfit or animation.

Local stutter repair: native outfit resets now refresh only the affected actor; detached status JSON formatting and disk writes run on a worker; bot-only rosters avoid repeated empty Steam transport calls. 80 focused regression checks pass. A 45-second private Downtown bot match recorded a 24.41 ms maximum frame interval (baseline 39.67 ms), with effectively unchanged median/P99 and no frames over 50 ms in either capture. The reported persistent chop was not reproduced, so complete stutter resolution remains unconfirmed. Evidence: cache/verification/stutter148/receipt.json.

Event-driven runtime follow-up: removed ten-second cosmetic keepalives and time-based peer expiry. Character selections, roster/replication/lifecycle notifications and changed incoming messages trigger game-frame work. Steam receive calls run only on the worker with a detached validated roster. Windows directory notifications detect request-file changes; unchanged background pumps schedule no game frames. Native idle verification recorded 30 seconds with unchanged frame-work counters, and touching the request file produced exactly one new dispatch. Bot catalog notifications update only new lists. Multiplayer validation with a second human remains pending.

The final 45-second Urban Mall bot capture recorded 4,740 frames, a 9.16 ms median, 18.21 ms P99 and 24.92 ms maximum. No frame exceeded 30 milliseconds in that capture. This limited local capture does not establish all-match performance or friend-PC acceptance.

Update through Settings → Check for updates. Allow Studio, Unreal and the game to close normally for the update to apply. Saved projects and artwork are preserved.
