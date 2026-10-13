# Friend test — Studio 0.2.75

Get the complete [Windows Studio beta](https://rowemods.com/studio), extract the whole ZIP into a writable folder and open **RoweMod Studio.cmd**. No Codex or separate .NET installation is needed.

## Test playing first

1. Install Hood Warfare 2 through Steam and close it.
2. Choose **Set up for playing**. This route needs no Epic, Unreal, Blender or mapping capture.
3. Open **Browse mods → ROWE Pants → Subscribe**. Let the download and matching classic-wearer setup finish.
4. Open **Wardrobe → Dress Classic DeShawn**, choose the pants and **Play with outfit**. Use the wearer/team shown by the item.
5. In Player Select, select that wearer and open the game's **Wardrobe**. Switch stock pants → ROWE pants → stock. Confirm the player identity stays the same.
6. Join a local match. Walk, crouch, jump, aim, reload, fire and respawn. Check the feet, hands, pants and body.
7. Close/reopen the game. Confirm the compatible selection returns and stock players remain available.

**Creator files available** means the item needs an authoring build; its `.roweclothes` source is not an installed mod.

Report your Studio version, setup choice, wearer/team, restart result and match result. Include screenshots and exact Task details for any failure. **Settings → Advanced setup → Copy setup report** supplies setup diagnostics.

This independent friend-PC acceptance is still outstanding. Developer-PC file checks, local wardrobe switching and restart checks are separate evidence. The supported-build local developer test passed stock/ROWE switching, restart retention and a DeShawn Crips match with correct pants/cuffs/feet after spawn, aiming, firing, reloading and brief movement/jump taps. Extended movement stress testing and two-PC multiplayer remain unverified.

## Test creating separately

Use **Create** and follow one path:

- **Start texture edit:** choose an existing item, **Export FBX & textures**, paint the existing UVs in Substance, then **Textures → Import texture set → Build & test**. This does not add a character.
- **Start clothing mesh:** choose a starter, **Export body & fitting kit**, fit and weight it in Blender, then **Import finished mesh**, add matching maps and **Build & test**. There is no automatic body fit.
- **Start character:** edit in MetaHuman Creator, return edits to Studio and prepare them for the game. Optional character data/tools are needed only for authoring.

For an authored character, **Wardrobe → Keep current item** preserves a version and **Save outfit** keeps named presets on the same wearer. Test that switching retains other artwork and does not add a new player. Classic ready-only profiles keep stock/prepared choices; authoring preset controls may be unavailable.

[Setup guide](STUDIO-FIRST-RUN.md) · [Substance guide](SUBSTANCE-GUIDE.md). Creator setup handles its mapping capture and cleanup. Complete vendor sign-in/license/install prompts yourself, then return for Studio's recheck.

Keep your original artwork. Restore a missing enabled PNG through **Import PNG** or **Import texture set** on the exact item/material. An absent optional Mask can remain disabled. Send the exact conflict message rather than deleting unknown loader/package files.
