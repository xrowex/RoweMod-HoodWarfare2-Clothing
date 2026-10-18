# RoweMod Studio 0.2.112 beta

Saved custom characters now retain their texture binding settings when reopened. Studio keeps verified unchanged fixed textures on their original shader, rebuilds older character packages containing shared texture replacements, and validates the complete runtime request before installation. Unsupported edited maps name the character, part, material and channel while preserving the artwork.

Build & launch now waits for the source editor belonging to that character. Completed shutdown without a remaining window no longer strands the build. Other known projects are left alone; unsaved dialogs and incomplete or unidentified shutdowns still block safely. Studio requests normal closure and never force-kills the user's editor for this handoff.

Includes 0.2.110's verified saved-hair recovery and custom-character spawn-reference repair, plus the earlier groom-slot, face-export, missing-helper and complete support-report improvements.

## Verification and limits

- Texture binding regression and installation preservation: 23 checks, including a reproduction against 0.2.110 and saved Cameron loading.
- Support reporting: 45 checks. Source-owned editor lifecycle: 21 checks; bridge handoff: 34 checks.
- The release package and production updater are checked against the actual 0.2.110 archive before publication.
- One's new complete Build & launch retry, visual acceptance and repeated multiplayer joins remain pending. This beta does not claim every future Unreal or Blender failure is prevented.
- The broad self-test's fake-game recovery fixture has an existing unsupported-multiplayer-runtime failure, reproduced on the previous local build. It is not counted as a passing full suite.

Your private local tattoo plugin is excluded. This release does not include the separate local voice-pack work.

Keep automatic updates enabled in Settings, or use Check for updates. Studio preserves saved characters, outfits and artwork and restarts after a safe update handoff. Creating MetaHumans still requires the matching Unreal Creator tools, core data and Epic sign-in.
