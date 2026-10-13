# Hood Warfare 2 clothing for RoweMod Studio

Download **RoweMod Studio for Windows** and curated, editable clothes for **Hood Warfare 2**, the first supported game. Studio guides you through fitting, texturing, importing and building your own clothing. You do not need Codex.

[Download Studio 0.2.68](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.68/RoweMod-Studio-0.2.68-Windows.zip) · [RoweMods Studio page](https://rowemods.com/studio) · [All releases](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases)

See [setup recovery and support](STUDIO-FIRST-RUN.md) and [dependency status](DEPENDENCY-STATUS.md). This beta still needs independent fresh-PC gameplay acceptance.

## Start here

1. Extract the complete Studio ZIP into a writable folder and open **RoweMod Studio.cmd**.
2. The checklist opens and starts automatically on first launch or when a required check is incomplete. Studio finds your tools, opens missing official installers and handles game mappings and cooker setup. Complete vendor prompts and install Unreal **5.8** in Epic when asked, then return to Studio.
3. When setup finishes, create **DeShawn**, keep his classic body and name your new character. Studio reads its body, clothes and rig automatically from your installed game.
4. Choose **Downloads → ROWE Pants → Download & add to character**, then **Build and Play** with the game closed.

No Codex or .NET SDK is needed. Manual paths and recovery/report tools are under **Settings → Advanced setup**. Existing matches, artwork and stock characters remain preserved. See [the setup guide](STUDIO-FIRST-RUN.md) and [the friend test](FRIEND-TEST.md).

## First download: ROWE Pants

Custom UVs and artwork by **One**. Fits the **classic DeShawn body and game rig**. Includes the garment FBX, Base color and DirectX Normal PNGs. The authored orange ROWE design keeps its colors on both teams.

[Download ROWE Pants 0.1.1](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/rowe-pants-v0.1.1/ROWE-Pants-0.1.1.roweclothes)

Studio's **Downloads** page handles the download and import for you. For a manually downloaded file, choose **My clothes → your Classic DeShawn character → Pants → Share → Import Pants package** and select the `.roweclothes` file, then **Build and Play**.

Importing creates editable copies; it does not install the mod until Build and Play. A different body or rig requires refitting the garment first. Aqua's custom body is a different fitting target. Check walking, crouching, jumping, aiming and reloading after installing.

To customize the design, use **Textures → Export for Substance / Import texture set**. To change its shape, use **Make clothing → Get fitting kit**, open its beginner guide, fit and weight the mesh around the supplied body in Blender, then **Import finished Pants mesh**. Keep the matching UVs, weights, material slots and game rig. Import Base Color and **DirectX Normal** PNGs from Substance; the current editable-clothing shader does not consume ORM or Emissive.

## Optional MetaHuman editing

Clothing editing does not need MetaHuman data. For character and skin authoring, install **MetaHuman Creator Core Data** for your Unreal 5.8 installation using [Epic's instructions](https://dev.epicgames.com/documentation/metahuman/getting-started-with-metahuman-creator-in-unreal-engine). Epic account sign-in is required.

Studio includes its own **Skin Details extension source**, not a compiled Unreal editor extension. To build it locally, install [Visual Studio 2022 / Build Tools](https://visualstudio.microsoft.com/downloads/) with **Desktop development with C++**, MSVC x64 tools and a Windows SDK. Save and close Unreal Editor, then choose **Settings → Run setup wizard → Character editing (optional) → Prepare character editing**. Studio checks that the result matches your exact editor build.

For an existing linked MetaHuman character, use **Open in MetaHuman Creator**, author tattoos/scars in **Skin Details**, choose **Send to RoweMod**, then **Import skin details** in Studio. Skin-map import does not automatically prepare new face/body geometry or hairstyles for the game.

## Publishing more clothing

This is a curated collection. Export an item through Studio's **Share -> Export package**, then provide the `.roweclothes` file, author name, matching body, screenshots, version and asset-sharing permission to the collection owner. Accepted items are published as GitHub Release assets and listed in `catalog.json`. The website reads this catalog; no public upload service is required.

## Compatibility and verification

ROWE Pants 0.1.1 uses clothing-package **version 3** and requires **Studio 0.2.63 or later** with the supported Hood Warfare 2 game build. Studio still imports version 2 packages. Version 3 checks the same indexed body topology, weights and rest rig while allowing export position rounding of less than 10 micrometres per coordinate. Its `Fit/Body.rowefit` file contains cryptographic compatibility evidence, not a body model or readable coordinates. The package also checks the base clothing and payload hashes. Full body/face/hair models, scripts and cooked game containers are excluded.

The new package imported into an independently exported local Classic DeShawn recipient while preserving other character parts. The matching source pants were checked in a local match. A fully fresh-PC setup-to-match test, automatic preparation of a brand-new MetaHuman head/body/hair, and two-PC multiplayer remain unverified. Releases are prereleases for wider testing; compatibility checks do not guarantee that any custom garment will avoid clipping in every animation.

## Asset rights

The repository owner confirmed permission to share this package's custom artwork and game-derived pants mesh/rig on October 12, 2026. Assets remain subject to their respective owners' rights. This repository does not apply an open-source license to game or third-party content.

## Previous release integrity

The original 0.1.0 download remains preserved. SHA-256 for `ROWE-Pants-0.1.0.roweclothes`:

`0a1caa0d126d7c012ce6d68dc0f6e037d52ce01379081ef6baf97249cf079818`
