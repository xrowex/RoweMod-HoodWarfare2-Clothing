# RoweMod Studio 0.2.105 beta — hair visibility

Fixes custom MetaHuman hair disappearing during small third-person camera rotations or when the camera moves farther from the character. Studio gives the custom head and its bound scalp groom enough render bounds for replacement hairstyles. This applies when the automatic character hairstyle is assigned; it adds no repeated idle bounds writes. Stock heads, other actors and facial detail grooms keep their existing settings. Unequipping restores the previous bounds, preserving later native or creator changes.

Cameron's braids passed the previously failing camera rotation in a local match, confirmed by the player. Runtime diagnostics confirmed bounds scale 2 on that match's custom head and scalp groom. All 44 focused ownership, restoration and groom-slot checks passed. One's earlier 0.2.104 build repair was confirmed by the user; this new hair fix has not yet been independently tested on One's PC. Two-PC multiplayer acceptance remains pending.

Update through Settings → Check for updates. Close Hood Warfare 2 when the updater needs to replace its runtime, then launch the game again. Existing prepared characters do not need rebuilding for this component-level repair. Saved characters, projects and artwork are preserved. Outfits remain fitted to one character.
