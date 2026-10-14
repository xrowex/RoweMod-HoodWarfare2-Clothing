# RoweMod Studio 0.2.87 beta

MetaHuman Build now detects missing Epic texture/rig prerequisites before issuing hidden cloud requests. It finishes the unattended editor, then makes one visible recovery attempt in the private build copy. Complete Epic sign-in if prompted; Studio requests texture sources and the joint rig, and continues export when Epic reports readiness. A failed request stops with diagnostics instead of repeating login attempts. Existing sources, artwork and previous builds are preserved. This does not bypass Epic authentication or repair an Epic service/network failure.

If Unreal is already open, Build waits for you to save and close its windows, then continues automatically. It does not force-close editors or save over unfinished work. This prevents overlapping editor sessions during preparation.

The Artwork screen no longer shows a stock fabric's white detail input as its finished Base Color. It identifies the active game material. Paint texture prepares its real Base Color before opening paint; preparation alone does not enable a custom edit. Reset restores the native fabric without enabling the white input or deleting artwork. Imported/painted PNGs remain unchanged, and baked paint colors avoid a second team tint.

Send to Rowe reports now include total/available system RAM and Windows committed/limit/peak memory, also logged before Creator launch. These help diagnose Unreal's Not enough memory to load MetaHuman Character error. They do not override Unreal's memory checks or establish that a particular PC meets Creator's requirements. No Windows memory or paging configuration is changed.

Validation includes native prerequisite recovery from a private character with missing textures/rig, vendor success/failure fixtures, real fabric paint preparation and offscreen artwork UI checks, application regressions, support-report checks and the previous updater. One's own memory error and complete friend-PC build/gameplay are not yet accepted.

Update in Settings and close Studio, Unreal and the game to apply it. In Creator, save your design before Build. Complete any Epic prompt in the visible build-copy window. If it still fails, press Send to Rowe; green confirms private receipt.
