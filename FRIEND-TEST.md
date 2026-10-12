# RoweMod Studio: friend clothing test

This Windows x64 package lets you make and exchange clothes for Hood Warfare 2. It includes Studio, the clothing workflow, game-compatible material tools, and the cosmetic loader. Your own installed game supplies its bodies and rigs during setup. The ZIP does not include someone else's characters, game files or Unreal Engine.

## Install once

1. Install Hood Warfare 2 through Steam and launch it normally once.
2. Install [Blender 5.x](https://www.blender.org/download/). Blender 5.1 is the verified authoring version; Blender also handles Studio's package imports.
3. Install Unreal Engine **5.8** through the [Epic Games Launcher](https://www.unrealengine.com/download). Studio uses your installed engine to prepare compatible clothing assets. Do not use 5.4 or 5.7 for this game.
4. Right-click the Studio ZIP → **Extract All**. Put the whole `RoweMod Studio` folder somewhere writable, such as Documents. Keep `app`, `tools`, `docs` and `rowemod.json` together.
5. Open **RoweMod Studio.cmd**. A separate .NET SDK installation is unnecessary; this package contains Studio's runtime.
6. Open **Settings**. Choose your Hood Warfare 2 folder, Blender and the matching `UnrealEditor-Cmd.exe` from your Unreal 5.8 installation. Click **Read game assets** to open the game-content tools and capture mappings if requested. Close the game before mapping capture, and stay at its main menu during the temporary capture launch. Studio must accept the installed game build before loading its cosmetic runtime.

The game-content step reads the game you own. Studio exports the selected classic starter locally when creating your first character. You do not receive extracted game meshes from another person. Studio also obtains its required compression decoder from your own installed matching Unreal engine; that proprietary decoder is not in this ZIP. Keep any setup error or Details text when reporting a problem.

The cosmetic loader also needs Microsoft's Visual C++ v14 runtime. Game or Unreal setup usually installs it. If Setup reports missing runtime libraries or Windows names `VCRUNTIME140`, `VCRUNTIME140_1` or an `MSVCP140` variant, install the **x64** package from [Microsoft's official Visual C++ downloads](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170), then restart the game. Studio checks all five runtime variants imported by its shipped helpers. This runtime is separate from the C++ development tools used for the optional extension build.

Setup requires approved unprotected Steam build **25888787**. An installed-looking but unsupported/protected build stays unavailable for capture and cosmetic installation. Use **Settings → Copy setup report** when reporting that result; preserve your artwork and use normal Steam play while awaiting support.

If mapping capture stops or fails, close the game, return to **Settings → Refresh setup checks → Finish mapping recovery**, then retry **Read game assets → Capture mappings**. Recovery removes only this workspace's recorded, unchanged capture proxy. If it refuses changed/unowned files or another game folder, leave those files intact and report the exact **Details** text. After successful capture, close its game and click **Scan game** if continuing in the game-content window.

The isolated cooker is created automatically. To recover from an unavailable configured drive, use **Settings → Choose cooker folder** and select a local folder dedicated to RoweMod. First-time shader cooking can take several minutes; use **Details** for progress or **Cancel** to stop safely.

## Make your first clothing test

For the shortest first test, choose **Create character → DeShawn** and keep his classic body. Name the character, then choose **Downloads → ROWE Pants → Download & add to character** and pick that new wearer. Studio checks the package's matching body and rig and changes only Pants. Close the game, choose **Build and Play**, then select your new character in the game. The pants keep their authored orange colors on both teams. A custom body such as Aqua is a different fitting target.

Use Studio **0.2.64** for this test with ROWE Pants **0.1.1**. The versioned release assets are [Studio for Windows](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.64/RoweMod-Studio-0.2.64-Windows.zip) and [ROWE Pants](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/rowe-pants-v0.1.1/ROWE-Pants-0.1.1.roweclothes). You can also download the garment file manually and use **My clothes → wearer → Pants → Share → Import Pants package**.

To test editing your own mesh next:

1. Create another character from a classic game starter and give the draft a name such as `My Clothes Test`.
2. Open **My clothes**, choose that character, then choose its garment. Start with pants or a hoodie.
3. Choose **Make clothing → Get fitting kit**. Open the exported `START-HERE.html` guide, then `Clothing-fitting-kit.blend` in Blender. The kit contains the matching body, editable clothing, weight source and exact game rig.
4. Choose **Edit the starter** for a small first edit, or **Bring your own clothing** if you already have a mesh. Follow the included fitting, weight-transfer and moving-pose instructions. Save your finished `.blend`.
5. Return to the same garment in Studio and use **Import finished mesh**. For the first mesh test, leave its original textures in place.
6. Close Hood Warfare 2 and choose **Build and Play**. In the Player menu choose your custom character. Press **C** for third person in a bot-free match; check walking, jumping, aiming and reloading. Test both teams.

## Paint in Substance Painter

Use the finished clothing mesh and its final UVs in Substance. Export Base Color and a **DirectX Normal** PNG. In Studio choose the same garment, then **Import texture set** and the matching material. The current clothing shader does not use Substance ORM or Emissive; keep the existing Mask instead of importing an unrelated packed map.

## Exchange clothes

Use Studio's clothing sharing/export controls to create a clothing package. Another user imports that package into its compatible garment slot. Compatibility checks still apply: a package made for one body/rig does not automatically fit a different body.

Use **Downloads** to browse the curated catalog. A connection failure offers Refresh and the release website; previously imported clothes stay available. Keep original garment/artwork rights separate from game body and rig references. Fitting-kit bodies and MetaHuman source assets stay local; editable garment packages can still contain game-derived clothing/armatures and need permission to share those assets.

## Optional MetaHuman editing

This clothing-test package does **not** include Unreal Editor binaries or a compiled Skin Details extension. It includes RoweMod's extension source for a separately licensed, matching Unreal editor installation. The current extension requires an exact editor build match; installing any Unreal 5.8 patch does not automatically prove compatibility.

Epic's [MetaHuman setup instructions](https://dev.epicgames.com/documentation/metahuman/getting-started-with-metahuman-creator-in-unreal-engine) require MetaHuman Creator Core Data and the MetaHuman Creator plugin. Install that data through Epic's launcher if you want MetaHuman editing later. Classic clothing editing does not require MetaHuman Core Data.

To build the included extension for your own engine, install [Visual Studio 2022](https://visualstudio.microsoft.com/vs/older-downloads/) with **Desktop development with C++**, MSVC v143 and a Windows SDK. Save your character and close Unreal Editor. In Studio, choose **Settings → Build Skin Details extension** after selecting your Unreal 5.8 tools. Studio uses your engine's automation tools to build RoweMod's source locally, then checks that the resulting extension matches your editor. Keep the build's Details output if it fails.

After the build completes, use **Open in MetaHuman Creator** for a character with a linked MetaHuman source. Edit your character there, use Skin Details for tattoos or scars, choose **Send to RoweMod**, then return to Studio and choose **Import skin details**. Face, body and hairstyle changes also require game-rig preparation; importing skin maps alone does not prepare a new character mesh. Starting from a brand-new MetaHuman does not yet provide a complete automatic head/body/hair-to-game workflow. This route still needs a fresh-PC editor and in-game acceptance test. Unreal Engine and editor-tool distribution follow [Epic's licensing terms](https://www.unrealengine.com/eula/unreal); they are external prerequisites, not files copied from the developer's PC.

## What to send back after testing

Before finishing, verify recovery on a disposable, disabled test creation. In **My characters**, uncheck its **Enable in game** box, then choose **More… → Delete…** for that test only. Choose **My characters → Recently deleted → Restore creation** and confirm the restored draft remains disabled. This check does not install the draft. Studio preserves recovery artwork under `dumps/deleted-mods` in its workspace. Keep your primary character and source artwork untouched; deleting an installed test requires closing/restarting the game as requested.

Use **Settings → Copy setup report** and paste it with the failed step and exact **Details** text. Confirm whether setup finds your supported game, the ROWE Pants download imports into a fresh Classic DeShawn character, a fitting kit opens with the matching body, the edited mesh imports, textures appear on the right garment, and the character remains correct while jumping/reloading/firing after a restart. Include the disabled test's delete/restore result. This complete fresh-PC test has not yet been accepted. Two-player visibility needs a separate two-PC check; matching mods on both PCs is a requirement to test, not proof that synchronization works.
