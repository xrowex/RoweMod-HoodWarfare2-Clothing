# RoweMod Studio — Hood Warfare 2

Download clothes, dress your existing players, or create something new. **Hood Warfare 2 is the first supported game.** No Codex is needed.

[Download Studio 0.2.96 beta for Windows](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.96/RoweMod-Studio-0.2.96-Windows.zip) · [Studio website](https://rowemods.com/studio) · [Releases](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases)

## Just want to play?

1. Extract the complete ZIP into a writable folder and open **RoweMod Studio.cmd**.
2. Choose **Set up for playing**. Have the game installed through Steam and closed for setup.
3. Open **Downloads → choose a published item → Subscribe**. Studio verifies the prepared item and its compatible wearer.
4. In **My characters**, choose that wearer → **Choose an outfit → Play with outfit**. Select the matching player in the game's Player Select screen, then open its **Wardrobe** for compatible stock/prepared clothes.

Prepared downloads need no Epic, Unreal, Blender or mapping capture. Browse mods only lists ready-to-play packages. Editable sources are separate: **Create → Get editable clothing files**; these need creator tools and a build before playing.

## Your workspace

| Page | Use it for |
| --- | --- |
| **My characters** | The three stock players and your prepared custom characters. Open one to customize it or choose an outfit. |
| **My clothes** | Individual clothing items, with their prepared source fits grouped under the same item. |
| **Downloads** | Browse ready-to-play mods and Subscribe. Creator-only items stay out of this player library. |
| **Create** | Choose Play mods, Edit textures, Make clothes or Make a character. Get editable clothing files here. |
| **Settings** | Setup, updates, optional MetaHuman tools and diagnostic reports. |

Character cards use model illustrations, never UV sheets. Custom portraits are generated from saved models when creator tools are available; **Refresh character previews** updates them. A labeled placeholder is shown while a portrait is unavailable. Illustrations are not proof of game appearance.

Existing prepared custom characters appear dynamically. Scratch clothing projects are not player identities. Recoverable library classification keeps saved source files and artwork; it does not delete hidden legacy drafts.

## Shared clothing preview

**Create → Make clothes** makes a clothing item independently of a character.
Choose Top, Pants, Shoes, Gloves, Mask, Bandana or Hat. The master kit uses one
authoring rig with green body references. Edit and save the Blender file, then
**Build clothing → Choose character & test**. Studio adapts the item to the
selected supported body and checks its geometry and skinning before equipping.
Failed checks preserve the previous outfit. Hand/finger fitting can currently
refuse gloves; full coverage and gameplay validation remain in progress.

Test movement, first person, clipping, materials and map travel before submitting
through the Google-authorized gallery review. Players receive the approved
ready-to-play item through Downloads; creator files remain separate. A shared
skeleton alone does not prove a correct fit for every body.

## Existing pants bundles

In **My clothes**, open the pants item and choose **Build one pants download · all fits**. Studio includes every current stock/custom body profile only after its fit is prepared and cooked. It names missing fits. Use **Add another body fit** to finish them, then **Submit pants with all fits** for gallery review. Players subscribe once and choose a character; Studio selects the matching variant. A new custom body still needs its own fitted and tested variant.

## Make clothes — save once, build from that file

Existing clothing projects retain their saved working files and four stages:

1. **Prepare once → Prepare fitting kit.** The kit includes the wearer reference, garment and game rig. Green bodies and weight sources are references. Body profiles in the same kit are labeled and separated.
2. **Edit & save.** Open the working file in Blender, fit your garment and transfer/check full weights. Save that same `Clothing-fitting-kit.blend`.
3. **Build & Play → Build & launch game.** Studio remembers the working file and reads only the selected garment/body fit automatically before cooking. No second FBX export, manual mesh import or required Substance roundtrip.
4. **Check in game → Looks good in game.** Walk, jump, aim and reload; check joints, hands, feet, textures and clipping before confirming.

Studio also offers **Create → Make clothes → Open kit in Blender**. This opens a working copy of the master game references, grouped by Tyreese, DeShawn and Darnell, with green clipping bodies and separate original rigs. For installed custom bodies, use the selected item's fitting project. New MetaHuman drafts use the master Top/Pants/Shoes adapter automatically. These references remain local and are not bundled game assets; fitting a garment on one body does not establish compatibility with every character.

**Already fitted and weighted your file?** Choose **Use an existing Blender file**. For Save As, use **Choose another saved file** once. Your original stays intact; Studio creates its own editable import. A moved file prompts you to choose its location instead of exporting another kit.

**Optional · textures, Substance & sharing** exposes painting, matching PNG imports, Substance exports and editable packages. Existing good textures stay in place. [Substance guide](SUBSTANCE-GUIDE.md).

One item can contain several source fits. **My clothes → item → Add another body fit** groups another prepared fit under that clothing identity. A prepared source fit still needs Build and an in-game check. Studio does not automatically resize or weight new geometry to another body. Ambiguous multi-body or whole-scene imports are refused; green references stay out of garment imports.

Changed Blender saves or artwork invalidate previous build/game-check completion. Failed or canceled work does not count as success. The checklist never treats launching the game as passing a visual test.

## Textures and characters

**Edit textures:** **Create → Edit textures → starter → item → Export model & textures**. Paint/import on **Artwork**, then **Use saved artwork & continue → Build & launch game**. Base is shown first; **Advanced · Normal & Mask** reveals surface maps. No new character is needed.

**Make a new character:** **Create → Make a character → name → Create new MetaHuman** creates a fresh, uniquely named MetaHuman source. It starts with Epic’s Bruce preset; choose a different preset and adjust face/body/hair in Creator. Studio does not clone the stock players or an existing custom character.

Open the draft in **MetaHuman Creator**, finish its face, body and hairstyle, and save. Return to Studio and choose **Build & launch game**. Studio assembles the saved character, adapts Body and Face to the native game rig, prepares the Creator hair/brows/lashes, fits the starter outfit and cooks the character automatically. Blender runs in the background; you do not need to open it, export FBX or import each part. Existing saved MetaHuman drafts use the same route. The source stays a draft until the complete build succeeds, and the original Creator asset is preserved.

Check your new character in Player Select and then walk, crouch, jump, aim and reload in a match before confirming **Looks good in game**. Custom clothing authoring still uses the fitting workflow above. Skin Details remains paused; plain Creator does not need the RoweMod extension or a C++ build. Optional advanced mesh and artwork tools remain available.

**Edit a stock player:** **My characters → Tyreese / DeShawn / Darnell → Edit this game character**. Choose **Edit textures**, **Edit meshes** or **Choose an outfit**. Body, Head & face and clothing cards lead to the selected tools. Stock edits keep that player’s original identity and do not mint another avatar. Prepared custom characters keep their existing editing workflow.

Creator setup finds installed tools, guides missing official installs and handles one-time mapping capture. Blender and matching Unreal **5.8.3** are creator tools. MetaHuman data/build tools are optional for character editing. [First-run guide](STUDIO-FIRST-RUN.md).

## Share gear

Open **My clothes → garment → Submit to gallery** (or **Submit this version**
for a saved wardrobe item). Connect your Google account in the browser and match
the code. Studio shows **Google connected ✓**. Once Rowe approves posting access,
enter the item's name, version and description. Confirm preparation, review its
preview and size, then confirm **Send to Rowe**. Studio collects the files itself.
**Sent ✓** means the server stored a receipt; the item stays private until review.

[Sign in and request creator access](https://rowemods.com/gear/upload). Rowe approves your account under [Admin → Creators & gear publishing](https://rowemods.com/admin/gear). Optional Discord handles help identify applicants but are not verified Discord links.

Approved creators upload one Studio `.roweclothes` package, fit information and a preview. Include a matching `.roweplay` export to offer Subscribe after review. Packages stay private until Rowe publishes them. Combined upload limit: 32 MiB; PNG/JPEG previews up to 4 MiB and 4096 pixels per side. Taking down an item or revoking a creator immediately removes public discovery and downloads while preserving installed copies and artwork.

ROWE Pants has been withdrawn from the gallery. Its previous release archives remain available for recovery. Shared rigs do not automatically fit different bodies, and asset rights remain with their owners.

## Updates and verification

Studio downloads verified updates when enabled. Close Studio, the game and Unreal to apply, then reopen; projects, artwork and settings remain. Settings provides update controls and setup reports. Mod subscriptions check published updates; equip updated assets with the game closed.

Version 0.2.88 retains the 0.2.83 Creator keepalive fix and adds automatic MetaHuman preparation plus updated cosmetic hair/wardrobe handling. A freshly saved MetaHuman was exported, adapted, bound, cooked, reopened and visibly checked in the animated game character-selection preview with its hairstyle and fitted outfit. Existing project definitions and sealed wardrobe proofs were preserved. A full match with the new character, independent friend-PC setup-to-match, extended movement and two-PC multiplayer remain unverified.

Follow [FRIEND-TEST.md](FRIEND-TEST.md). Include version, exact error and **Settings → Advanced setup → Copy setup report** for support. Preserve original art and old folders. Historical evidence is in [CHANGELOG.md](CHANGELOG.md); [dependency status](DEPENDENCY-STATUS.md) is a separate record.

Saved wardrobe garments also appear in **My clothes** automatically. Choose the card to wear it on its original character or **Equip & edit**. Repeated saves share one card with selectable versions.

## Need help?

Press **Send to Rowe** in Studio's bottom bar. The button turns green only after the private report is received. Logs are collected automatically; no attachments needed. Reports exclude artwork and models and redact common credentials and personal paths. Nothing uploads until you press the button.


## Submit gear from Studio

My clothes → garment → Submit to gallery → Google sign-in → match the connection code → Rowe approves posting access → prepare and review → confirm Send to Rowe. Studio collects the garment and preview. The button turns green only after receipt. Gear stays private until reviewed. See RELEASE-NOTES-0.2.91.md.
