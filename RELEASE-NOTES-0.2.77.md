# RoweMod Studio 0.2.77 beta

Clothing authoring now remembers your Blender working file. Prepare the fitting kit once, fit and transfer/check weights, save, then **Build & launch game**. Studio creates a private garment import from the selected saved fit before cooking. Existing good textures stay in place; Substance/texture edits and sharing are optional. An already fitted file can be selected directly, and Save As needs one new file selection.

The four stages are **Prepare once → Edit & save → Build & Play → Check in game**. Changed source saves or maps invalidate prior build/game checks. Failed/canceled imports cannot launch the game through the guided action. During-cook source changes are guarded before launch. The in-game check needs explicit user confirmation; a successful launch does not mean a garment is accepted.

Fitting kits label several body profiles in one Blender file and display green body/weight references. Imports select the current garment/profile, excluding reference bodies; ambiguous or whole-scene selection is refused. New geometry still needs manual fitting and full game-rig weights. Source fits group under one clothing item and remain distinct from installed, verified game fits.

New character creation now creates a fresh, unique MetaHuman source, rather than copying a stock or saved custom player. The inactive source draft resumes under Create. Skin handoff cannot satisfy geometry readiness: both new Body and Face must be explicitly adapted/imported against the native game rig before a native build activates an avatar. Hair still needs compatible preparation. Stock players have separate texture/mesh editing workspaces that retain their original identity. New-source identity, draft gating and UI callbacks are fixture-tested; a complete new MetaHuman geometry conversion has not been accepted in game.

**My characters / My clothes / Downloads / Create / Settings** separate identities, garments and subscriptions. My characters includes the three stock players and dynamically discovers installed custom characters. Character cards use model illustrations, not UV textures. Stock portraits contain rendered original FBX geometry; unavailable hair grooms and game lighting are not reproduced. Custom portraits are generated/refreshed from saved sources. Legacy scratch records are classified recoverably rather than deleted.

This release changes Studio, authoring scripts, fitting guidance and portrait assets. Shipped native cosmetic runtime files and prepared wardrobe payloads are retained byte-identically from the authoritative 0.2.76 portable baseline; authoring tools have changed. Prior developer-PC native wardrobe acceptance is separate. No new independent friend-PC, Substance UI, full hair-groom, extended movement or two-PC multiplayer acceptance is claimed.

Close Studio, Hood Warfare 2 and Unreal to apply the update. Keep original artwork and saved Blender files. Previous releases remain available.

[Download](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.77/RoweMod-Studio-0.2.77-Windows.zip) · [Guide](README.md) · [Substance](SUBSTANCE-GUIDE.md) · [Friend test](FRIEND-TEST.md)
