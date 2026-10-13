# RoweMod Studio — Hood Warfare 2

Play curated clothing mods, keep clothes on one character, or make your own. **Hood Warfare 2 is the first supported game.** No Codex is needed.

[Download Studio 0.2.75 for Windows](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.75/RoweMod-Studio-0.2.75-Windows.zip) · [Studio website](https://rowemods.com/studio) · [Releases](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases)

## Just want to play?

1. Extract the complete ZIP into a writable folder and open **RoweMod Studio.cmd**.
2. Choose **Set up for playing**. Have the game installed in Steam and closed for setup.
3. Open **Browse mods → ROWE Pants → Subscribe**. Studio downloads the verified ready-to-play item and prepares its matching classic wearer.
4. Open **Wardrobe**, choose that wearer, then **Play with outfit**. In the game's Player Select screen, select the matching player and open **Wardrobe** to choose compatible prepared or stock clothes.

Prepared player downloads need **no Epic Launcher, Unreal, Blender or mapping capture**. Items marked **Creator files available** need creator tools and a build before playing.

## Your workspace

| Page | Use it for |
| --- | --- |
| **Browse mods** | Subscribe to ready-to-play items or get editable creator files. |
| **My mods** | Find downloads, update subscriptions, equip items or edit creator files. |
| **Wardrobe** | Dress an existing classic/custom wearer. Authored characters also support **Keep current item** and named **Save outfit** presets. |
| **Create** | Choose **Edit textures**, **Make clothing** or **Make a character**. |

Changing clothes keeps the same character identity. Wardrobe choices and outfit presets are local. A garment must match the body, native slot and game rig; there is no automatic fitting to another body or verified multiplayer wardrobe synchronization.

## ROWE Pants

Custom UVs and artwork by **One**, fitted to classic DeShawn. Release 0.1.2 adds player delivery; the unchanged prepared asset retains its filename `ROWE-Pants-0.1.1.roweplay`.

- [Ready-to-play pants](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/clothing-rowe-pants-v0.1.2/ROWE-Pants-0.1.1.roweplay): already cooked for compatible players.
- [Editable creator files](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/rowe-pants-v0.1.1/ROWE-Pants-0.1.1.roweclothes): garment FBX, Base color, DirectX Normal and fit evidence.

The thumbnail renders the actual garment and textures under studio lighting; it is not an in-game screenshot. Aqua and other reshaped bodies require a different fit.

## Create something

**Edit textures:** **Create → Start texture edit → choose an item → Export FBX & textures**. Paint its existing UVs in Substance, then **Textures → Import texture set → Build & test**. No new character or mesh import is needed. [Substance guide](SUBSTANCE-GUIDE.md).

**Make clothing:** **Create → Start clothing mesh → choose a starter → Export body & fitting kit**. Fit and weight your garment around the supplied body in Blender, keep the game rig, then **Import finished mesh**, add the painted maps and **Build & test**. Fitting and full weights remain authoring work.

**Make a character:** **Create → Start character**. Use MetaHuman Creator for face, hair and Skin Details, then send/import the edits back to Studio. Changed body/head geometry and hair still need game preparation separately from skin-map import.

Creator setup finds tools, handles mapping capture and guides missing official installations. Matching Unreal **5.8.3** and Blender are creator tools. MetaHuman data and extension build tools are optional for character editing. [First-run guide](STUDIO-FIRST-RUN.md) · [MetaHuman setup](METAHUMAN-SETUP-GUIDE.md).

## Updates, support and verification

Studio downloads verified updates in the background. Close Studio, the game and Unreal when ready to let them apply; projects, artwork and settings are retained. Settings provides update controls and setup reports. Subscriptions check for mod updates; equip updated assets with the game closed.

Local native wardrobe acceptance is verified on the supported Steam build on the developer PC: Player Select stock/ROWE switching, saved selection after restart, and a DeShawn Crips match with black ROWE pants, orange cuffs and correct feet after spawn, aiming, firing, reloading and brief movement/jump taps. Extended movement stress testing remains outstanding. Exact-assembly package/ownership/rollback and optional-map checks passed; these are separate from gameplay. Independent friend-PC setup-to-match and two-PC multiplayer remain unverified.

Follow [FRIEND-TEST.md](FRIEND-TEST.md). For failures, include the Studio version, exact message and **Settings → Advanced setup → Copy setup report**. Keep existing artwork and old folders while resolving missing references.

## Share a mod

Send the collection owner your finished creator package, author name, compatible body, screenshots, version and sharing permission. A curated ready-to-play `.roweplay` also needs a verified cook, exact game/body/rig profile and publisher acceptance. Editable `.roweclothes` files are authoring sources, not ready-to-play mods. There is no public upload account or automatic fit service.

The repository owner confirmed permission to share the ROWE artwork and game-derived pants mesh/rig on October 12, 2026. Underlying assets retain their owners' rights; game/third-party content has no new open-source license here. Previous releases remain available. Historical validation is in [CHANGELOG.md](CHANGELOG.md); [dependency status](DEPENDENCY-STATUS.md) is a separate record.
