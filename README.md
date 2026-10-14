# RoweMod Studio — Hood Warfare 2

Download clothes, dress your existing players, or create something new. **Hood Warfare 2 is the first supported game.** No Codex is needed.

[Download Studio 0.2.82 for Windows](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.82/RoweMod-Studio-0.2.82-Windows.zip) · [Studio website](https://rowemods.com/studio) · [Releases](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases)

## Just want to play?

1. Extract the complete ZIP into a writable folder and open **RoweMod Studio.cmd**.
2. Choose **Set up for playing**. Have the game installed through Steam and closed for setup.
3. Open **Downloads → ROWE Pants → Subscribe**. Studio verifies the prepared item and its compatible wearer.
4. In **My characters**, choose that wearer → **Choose an outfit → Play with outfit**. Select the matching player in the game's Player Select screen, then open its **Wardrobe** for compatible stock/prepared clothes.

Prepared downloads need no Epic, Unreal, Blender or mapping capture. **Creator files available** means editable sources need creator tools and a build before playing.

## Your workspace

| Page | Use it for |
| --- | --- |
| **My characters** | The three stock players and your prepared custom characters. Open one to customize it or choose an outfit. |
| **My clothes** | Individual clothing items, with their prepared source fits grouped under the same item. |
| **Downloads** | Subscribe to curated ready-to-play items or get editable creator files. |
| **Create** | Choose Play mods, Edit textures, Make clothes or Make a character from picture cards. |
| **Settings** | Setup, updates, optional MetaHuman tools and diagnostic reports. |

Character cards use model illustrations, never UV sheets. Custom portraits are generated from saved models when creator tools are available; **Refresh character previews** updates them. A labeled placeholder is shown while a portrait is unavailable. Illustrations are not proof of game appearance.

Existing prepared custom characters appear dynamically. Scratch clothing projects are not player identities. Recoverable library classification keeps saved source files and artwork; it does not delete hidden legacy drafts.

## Make clothes — save once, build from that file

Use **Create → Make clothes → starter → clothing slot**. Follow four stages:

1. **Prepare once → Prepare fitting kit.** The kit includes the wearer reference, garment and game rig. Green bodies and weight sources are references. Body profiles in the same kit are labeled and separated.
2. **Edit & save.** Open the working file in Blender, fit your garment and transfer/check full weights. Save that same `Clothing-fitting-kit.blend`.
3. **Build & Play → Build & launch game.** Studio remembers the working file and reads only the selected garment/body fit automatically before cooking. No second FBX export, manual mesh import or required Substance roundtrip.
4. **Check in game → Looks good in game.** Walk, jump, aim and reload; check joints, hands, feet, textures and clipping before confirming.

**Already fitted and weighted your file?** Choose **Use an existing Blender file**. For Save As, use **Choose another saved file** once. Your original stays intact; Studio creates its own editable import. A moved file prompts you to choose its location instead of exporting another kit.

**Optional · textures, Substance & sharing** exposes painting, matching PNG imports, Substance exports and editable packages. Existing good textures stay in place. [Substance guide](SUBSTANCE-GUIDE.md).

One item can contain several source fits. **My clothes → item → Add another body fit** groups another prepared fit under that clothing identity. A prepared source fit still needs Build and an in-game check. Studio does not automatically resize or weight new geometry to another body. Ambiguous multi-body or whole-scene imports are refused; green references stay out of garment imports.

Changed Blender saves or artwork invalidate previous build/game-check completion. Failed or canceled work does not count as success. The checklist never treats launching the game as passing a visual test.

## Textures and characters

**Edit textures:** **Create → Edit textures → starter → item → Export model & textures**. Paint/import on **Artwork**, then **Use saved artwork & continue → Build & launch game**. Base is shown first; **Advanced · Normal & Mask** reveals surface maps. No new character is needed.

**Make a new character:** **Create → Make a character → name → Create new MetaHuman** creates a fresh, uniquely named MetaHuman source. It starts with Epic’s Bruce preset; choose a different preset and adjust face/body/hair in Creator. Studio does not clone the stock players or an existing custom character.

The source remains an inactive draft under **Create → Continue MetaHuman draft**. **Open in MetaHuman Creator** edits it. Skin Details is paused; plain Creator does not need the RoweMod extension or a C++ build. Use Studio texture tools or Substance for artwork. To make it a game player, use **Prepare Body & Face for the game rig**: export the new MetaHuman geometry in Unreal, adapt both meshes to the supplied native game rig, and import both parts. Only a complete compatible Body/Face import and native build can activate it; hair needs separate binding/preparation. This is an explicit authoring workflow, not automatic MetaHuman-to-game geometry conversion.

**Edit a stock player:** **My characters → Tyreese / DeShawn / Darnell → Edit this game character**. Choose **Edit textures**, **Edit meshes** or **Choose an outfit**. Body, Head & face and clothing cards lead to the selected tools. Stock edits keep that player’s original identity and do not mint another avatar. Prepared custom characters keep their existing editing workflow.

Creator setup finds installed tools, guides missing official installs and handles one-time mapping capture. Blender and matching Unreal **5.8.3** are creator tools. MetaHuman data/build tools are optional for character editing. [First-run guide](STUDIO-FIRST-RUN.md).

## ROWE Pants and sharing

Custom UVs and artwork by **One**, fitted to classic DeShawn. The public prepared asset remains `ROWE-Pants-0.1.1.roweplay`:

- [Ready-to-play pants](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/clothing-rowe-pants-v0.1.2/ROWE-Pants-0.1.1.roweplay).
- [Editable creator files](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/rowe-pants-v0.1.1/ROWE-Pants-0.1.1.roweclothes).

Different body shapes need their own fit. Editable `.roweclothes` packages are sources, not installed mods. Send the collection owner a finished package, author name, fit, version, screenshots and sharing permission. A curated `.roweplay` additionally needs a verified cook and exact game/body/rig profile. There is no public upload account or automatic fitting service. Asset rights remain with their owners; there is no new open-source license for game or third-party content. The repository owner confirmed permission to share the ROWE artwork and game-derived pants mesh/rig on October 12, 2026; source-package rights notices are retained.

## Updates and verification

Studio downloads verified updates when enabled. Close Studio, the game and Unreal to apply, then reopen; projects, artwork and settings remain. Settings provides update controls and setup reports. Mod subscriptions check published updates; equip updated assets with the game closed.

This beta changes Studio's libraries and authoring tools. Shipped native cosmetic runtime and prepared clothing payloads remain pinned to the prior portable release; authoring scripts and guides have changed. Prior developer-PC local wardrobe acceptance remains separate. Independent friend-PC setup-to-match, extended movement stress testing and two-PC multiplayer remain unverified.

Follow [FRIEND-TEST.md](FRIEND-TEST.md). Include version, exact error and **Settings → Advanced setup → Copy setup report** for support. Preserve original art and old folders. Historical evidence is in [CHANGELOG.md](CHANGELOG.md); [dependency status](DEPENDENCY-STATUS.md) is a separate record.

Saved wardrobe garments also appear in **My clothes** automatically. Choose the card to wear it on its original character or **Equip & edit**. Repeated saves share one card with selectable versions.
