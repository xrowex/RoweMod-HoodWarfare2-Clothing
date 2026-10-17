# Character-specific outfits

Universal fitting and the modular in-game clothing selector were canceled on October 17, 2026. Each outfit is now authored for one selected character.

In Studio, choose **Create → Fit an outfit**, choose the character, and open its clothing part. Export its fitting kit, fit and weight the clothes in Blender, save, then use that same character and slot for **Build & launch**. The kit contains one game armature and that character's green body references. Studio does not reshape clothing or transfer its weights automatically. Clothes flagged as needing manual binding must be weighted to this rig before building.

Character and slot tags prevent a saved kit from being imported into a different character. Ready-to-play downloads keep their exact body and game-rig compatibility checks. Shared and multi-character downloads are retired.

Existing artist projects, saved garments, textures, game packages and saves are preserved. Older shared sources remain accessible for manual recovery. The retired source is recoverable in `archive/modular-clothing-20261017/source-before-retirement.zip` and the adjacent `retired` directory.

The public release remains 0.2.98 until a separately verified release is published. Local cleanup builds are 0.2.99 candidates. Build, import and kit tests do not establish that every outfit is correctly fitted; each new outfit still needs movement and clipping checks in game.
