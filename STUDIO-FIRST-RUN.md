# First run — Studio 0.2.76

[Download Studio](https://rowemods.com/studio), extract the entire ZIP into a writable folder and open **RoweMod Studio.cmd**. Keep the folders together. Its runtime is bundled; Codex and a .NET SDK are unnecessary.

## Choose a route

| Welcome choice | Requirements |
| --- | --- |
| **Set up for playing** | Supported Steam game and RoweMod's cosmetic runtime. No Epic, Unreal, Blender, MetaHuman data or mapping capture. |
| **Set up for creating** | Game, Blender and matching Unreal tools for export/fitting/cooking. MetaHuman tools are optional for character editing. |

Close the game for setup/install. Changed or unowned loader/package files are preserved and reported as conflicts.

## Play downloaded mods

Choose **Set up for playing**, then **Browse mods → ready-to-play item → Subscribe**. Studio verifies the download and separate body/rig profile, then prepares the matching wearer. Use **My mods** for downloads and **Wardrobe → Play with outfit** to launch. In Player Select, choose the wearer and open the game's **Wardrobe** for compatible stock/prepared choices.

A `.roweplay` contains prepared game assets. A `.roweclothes` contains editable sources and needs creator preparation before play. Player setup does not require a new character or a body export. Imported clothing must match its stated fit; it is not automatically resized. If a saved version is no longer installed, return to **My mods** to install/equip it again.

## Create mods

The creator checklist opens when creation needs missing setup. It finds installed tools, guides official installs, prepares an isolated cooker and handles the one-time mapping capture and cleanup. No manual capture-button hunt or asset scan is needed.

Complete official vendor prompts yourself. Use verified Unreal **5.8.3** and return for a recheck. Review Epic's displayed sizes before downloading. Finish existing matches first: Studio only closes a capture process whose ownership it can prove.

Open **Create**:

- **Edit textures:** choose a starter card, then its item card. **Export model & textures → Artwork → Import texture set → Use saved artwork & continue → Build & launch game**. Check it in a match and confirm **Looks good in game**. This item project does not add a player identity.
- **Make clothes:** choose a starter and clothing slot, **Export fitting kit**, fit and weight in Blender, then **Import finished mesh → Artwork → Use saved artwork & continue → Build & launch game**.
- **Make a character:** name it, choose a starter card and click **Create character**. Choose **Face, hair & skin**, use MetaHuman Creator and Skin Details, send/import the edits and prepare them for the game. Changed head/body geometry and hair need separate preparation from skin maps.

Optional character editing requires **MetaHuman Creator Core Data** and a matching Skin Details extension. **Settings → Set up MetaHuman Creator** guides Epic Options, sign-in and missing C++ build tools. Clothing authoring does not need Core Data. [MetaHuman guide](METAHUMAN-SETUP-GUIDE.md).

## Keep outfits and artwork

In **Wardrobe**, choose a wearer and compatible clothes without duplicating the character. On authored characters, **Keep current item** saves a protected garment version and **Save outfit** keeps named choices. Classic ready-only profiles keep prepared/stock selections without source tools; they do not expose every authoring preset control.

Library copies are separate from current editable art. New clothes still need fitting and full game weights. Selections/presets are local; multiplayer sharing and synchronization are unverified.

## Recovery and updates

Use **Settings** for creator setup, installation folders and reports. Interrupted capture recovers with the game closed. Changed/unrelated loaders stay preserved.

For a missing enabled texture, use **Import PNG** or **Import texture set** on its exact item/material. A disabled absent Mask can be saved without inventing pixels. Reset cannot recover an unavailable original; retain old artwork folders.

Studio downloads verified program updates in the background. Close Studio, the game and Unreal to let the helper apply them and reopen Studio while retaining user data. Settings has **Keep Studio updated automatically** and **Check for updates**. Versions before 0.2.70 need one manual download. Mod subscriptions also check updates; equip new assets with the game closed.

## Test status

Developer-PC Player Select stock/ROWE switching and saved selection after restart are checked. Exact-build package/hash/ownership/rollback and optional-map tests passed. The supported-build DeShawn Crips local match passed visible pants/cuffs/feet checks after spawn, aiming, firing, reloading and brief movement/jump taps. Extended movement stress testing remains outstanding. Another PC's complete setup-to-match, missing-vendor installs and two-PC multiplayer remain unverified. [Friend test](FRIEND-TEST.md) · [Changelog](CHANGELOG.md).
