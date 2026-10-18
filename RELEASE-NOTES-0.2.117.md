# Rowe Studio 0.2.117 beta

## Clothing customization

Customized clothing no longer fails because its original material uses a shared game texture. Studio creates a separate garment material and cooked textures for the selected character across every supported clothing slot. Existing artwork stays enabled and saved.

- Editing Base color retains the original Normal and Roughness maps where available. Needed original maps are copied into the garment package, so downloaded gear uses the same appearance.
- Advanced surface maps support explicit Roughness, ORM, RMA, Metallic and Occlusion layouts. Unknown clothing-region masks receive an actionable message before MetaHuman preparation begins.
- Ready-to-play and multiplayer packages carry the material and map settings. Editable clothing packages retain their surface layout, while older packages remain readable.
- Missing or stale clothing cooks trigger a rebuild instead of installing shared texture replacements.

## Studio improvements

- Updated Rowe Studio branding, icon, cached thumbnails and responsive library/catalog loading. Navigation and cancellation remain available during reads, and large libraries create controls only for visible rows.
- Character cards remain visible after window scaling; permanent character, clothing and download deletion controls are retained.
- Mod profiles review package versions, dependencies and compatibility before applying a setup. Interrupted downloads and installs preserve the previous installation, with clearer recovery details in reports.
- Characters and outfits retain their individual fitted bodies; this release does not enable universal clothing fitting or short-character gameplay scaling.

## Test an existing customized garment

Let Studio finish updating and relaunch. Open the existing character, keep the edited Base color enabled, and choose Build and launch. There is no need to reset or recreate the character. If a custom surface map needs a layout, select the layout matching its export in Artwork -> Advanced, then build again. Send to Rowe from the failed operation if it still fails.

## Verification and limits

Local checks passed for clothing isolation and old/new package metadata, a real Unreal 5.8.3 ski-mask cook, independent saved-material/texture readback, UI behavior, scaled layouts and release deletion controls. The complete ZIP is audited and tested through the previously published updater before the feed is promoted. One's updated in-game clothing retry and full two-PC multiplayer appearance/cache acceptance are still pending.

The portable download contains program files and owned helpers only. Game/MetaHuman assets, user projects, private reports, XERJ and the local tattoo plugin are excluded. Existing dependency advisory status is documented in DEPENDENCY-STATUS.md.
