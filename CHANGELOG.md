# Releases

## Studio 0.2.62 beta


RoweMod Studio now gives clothing its own workspace and a guided path from a matching body/rig to editable clothes for Hood Warfare 2. Start with a classic character, get a fitting kit, fit and weight your mesh in Blender, optionally paint it in Substance, then import and **Build and Play**.

- Separate **My characters** and **My clothes** pages, explicit garment choices and contextual **Make clothing / Textures / Model / Share** tools.
- **Downloads → Download & add to character** downloads curated clothes, asks who will wear them, verifies the package and imports only that garment. Original character parts and external source files are preserved.
- A first-run **Settings** checklist finds local Steam, Blender 5.x and Unreal 5.8 installations, including custom locations. Missing tools have official setup links. The app's .NET runtime is included; game and engine installations remain external.
- Automatic local cooker creation and editable garment packages with rig/body-fit checks. Version 3 allows small position rounding between independent exports without accepting a different body, topology, weights or rest rig. Version 2 imports remain supported.
- Actual MetaHuman Creator handles character viewing and skin authoring. Optional Skin Details ships as source and can be built against the recipient's installed editor using **Settings → Build Skin Details extension**.

Download asset: [RoweMod-Studio-0.2.62-Windows.zip](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.62/RoweMod-Studio-0.2.62-Windows.zip).

Install Hood Warfare 2, Blender 5.x and Unreal Engine 5.8, extract the full ZIP, open **RoweMod Studio.cmd**, and follow **Settings → Read game assets**. Create a **Classic DeShawn** character for the ROWE Pants test. If a Visual C++ runtime DLL is missing, use [Microsoft's x64 runtime](https://aka.ms/vc14/vc_redist.x64.exe).

MetaHuman editing additionally needs Epic account sign-in and **MetaHuman Creator Core Data**. The optional local extension build needs Visual Studio C++ tools and a Windows SDK; that is separate from the Visual C++ redistributable. A new head/body/hairstyle still requires game preparation beyond skin-map import.


**Verified locally:** 56 UI checks, 28 package checks, 15 body-fit regression checks, and an independently exported Classic DeShawn recipient import. No personal projects, game bodies, Unreal binaries or MetaHuman data are bundled.

**Early testing limits:** a completely fresh PC has not completed setup-to-match; local Skin Details compilation and two-PC multiplayer still need acceptance. New MetaHuman head/body/hair preparation remains separate.

Extract the entire ZIP, follow Settings, then Create character → DeShawn → Downloads → ROWE Pants → Download & add to character → Build and Play. See the included FRIEND-TEST.md and STUDIO-FIRST-RUN.md guides.

## ROWE Pants 0.1.1

Same garment and artwork as 0.1.0; version-3 body-fit evidence fixes independent FBX export rounding. Use Studio 0.2.62 or later. Original 0.1.0 remains available.
