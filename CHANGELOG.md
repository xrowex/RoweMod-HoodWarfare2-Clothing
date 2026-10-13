# Releases

# RoweMod Studio 0.2.68 beta

Repairs one-time mapping setup when launching outside Steam and when Windows PowerShell writes capture configuration. Capture now starts the verified shipping executable directly, supplies its Steam app identity only to that child process, and writes the Lua and runtime configuration as UTF-8 without a byte-order mark.

- Temporary Steam environment values restore exactly after launch or launch failure. Studio does not change your permanent Windows environment or Steam launch options.
- Capture retains its owned process handle, waits for the mapping writer to close, copies complete bytes through an exclusive source handle, then closes only its proven capture game.
- Existing verified RoweMod loaders and runtime-path files are paused and restored with their exact previous bytes or absence. Cancellation and interrupted setup retain guarded recovery; changed or unrelated loaders and existing matches stay protected.
- First-run setup and character creation still continue automatically with your selected starter. The optional MetaHuman route remains separate from clothing setup.

Extract the complete ZIP into a writable folder and open **RoweMod Studio.cmd**. Close an existing game when setup asks. Complete official vendor installation prompts if tools are missing, then return to Studio. If an older setup attempt failed, close its capture game and reopen the setup wizard in this version; do not delete or edit the game loader yourself. See STUDIO-FIRST-RUN.md and FRIEND-TEST.md.

Verified against this DLL: 127 isolated UI checks, 24 automatic setup checks, 43 setup/recovery checks, 99 loader/capture recovery checks and 117 checks against the actual capture script under Windows PowerShell 5.1. Capture fixtures use fake files and mocked process launches; they do not launch the game. The capture script and ZIP match the recorded hashes.

A separate developer prototype based on a modified 0.2.67 app completed capture and closed its capture game. Its loader/path recovery was checked separately; this prototype is not this public 0.2.68 ZIP. Acceptance of this exact public download's fresh mapping capture and fresh-PC setup-to-match workflow remains pending. Clothing import, sharing and isolated Unreal cooking passed on 0.2.66; those authoring paths are unchanged here. Two-PC multiplayer and recipient MetaHuman extension compilation remain unverified. Proprietary game, engine and MetaHuman assets are not bundled. See DEPENDENCY-STATUS.md for pinned ImageSharp advisories. Previous releases remain available.


# RoweMod Studio 0.2.67 beta

Fixes automatic setup stopping when an unchanged RoweMod loader is already installed, including one owned by an older Studio folder. Studio verifies and pauses that loader, captures mappings, and restores the original loader and path automatically. Saved characters, installed mods and artwork remain intact.

- Mapping capture now also installs a temporary verified runtime path beside the game. This avoids relying solely on bootstrapper argument forwarding on a clean PC. The original path's exact bytes or absence are restored.
- Recovery handles interrupted setup, cancellation and capture failure. Changed or unrelated loaders are preserved; existing matches stay running until you close them.
- Setup still opens and starts automatically on first launch or incomplete required setup, and character creation continues with your saved choices.

Extract the entire ZIP into a writable folder and open **RoweMod Studio.cmd**. Close an existing game when setup asks, then return to Studio for automatic continuation. Complete official vendor prompts if requirements are missing. See STUDIO-FIRST-RUN.md and FRIEND-TEST.md.

Verified against this DLL: 127 isolated wizard/continuation checks, 24 automatic setup sequencing checks, 43 setup/recovery checks, 99 loader/capture recovery checks and 28 actual PowerShell atomic-writer checks. Fixtures do not launch a game. Clothing import, sharing and isolated Unreal cooking passed on 0.2.66; those authoring paths are unchanged in this repair.

The friend's reported UE4SS load failure needs a retest on this version; its exact remote cause is not confirmed. Fresh mapping capture and fresh-PC setup-to-match acceptance remain pending. Two-PC multiplayer and recipient MetaHuman extension compilation remain unverified. Proprietary game, engine and MetaHuman assets are not bundled. See DEPENDENCY-STATUS.md for the pinned ImageSharp advisories. Previous releases remain available.


# RoweMod Studio 0.2.66 beta

Open Studio. Setup opens and starts automatically on first launch, or when a required check is incomplete. Mapping capture, closure of Studio's capture game, temporary-loader recovery and cooker preparation are automatic. Existing matches stay open until you close them.

- **Create and customize** opens setup if needed and continues with the same name, starter and outfit choices after success. Cancelling keeps those choices.
- Finds installed tools and helps install missing tools through official vendors. Return from Steam/Epic to resume; Epic sign-in, engine installation and license prompts still use their normal windows.
- Fixes clothing downloads into an unprepared default starter: its reference game rig is generated automatically from the unchanged local game export.
- Fixes sharing texture-only clothing on a stock model. Sharing does not switch the author's selected model or change saved artwork.
- Required setup and clothing are separate from optional MetaHuman Creator/Core Data, local C++ extension compilation and Substance Painter.

Extract the complete ZIP, open **RoweMod Studio.cmd**, finish any vendor prompts, then create **DeShawn**. Choose **Downloads → ROWE Pants → Download & add to character**, then **Build and Play** with the game closed. See STUDIO-FIRST-RUN.md and FRIEND-TEST.md.

Verified against this DLL: 187 isolated UI checks (including the actual packaged checklist and continuation), 24 setup sequencing checks, 43 setup/recovery checks, 32 installer/download checks, 25 reference-rig checks, and real Blender clothing import/sharing. The default starter that failed in 0.2.65 now imports the public pants download. The isolated Unreal 5.8 cook and native container/rig checks passed; no game files were changed or mods installed by that check.

These local fixtures use installed tools and a matching private mapping copy. Fresh-PC vendor installation, fresh mapping capture and setup-to-match acceptance remain pending. Two-PC multiplayer remains unverified. New MetaHuman geometry/hair still needs separate game preparation. Game/engine/MetaHuman data and proprietary decoder assets are not bundled. Five pinned ImageSharp advisories remain documented in DEPENDENCY-STATUS.md. Previous releases remain available.


# RoweMod Studio 0.2.65 beta

Open Studio and click **Set up automatically**. The first-run popup shows four simple checks: game, Blender, Unreal and game setup. Manual paths and the legacy asset exporter stay under Advanced.

- Finds installed tools and saves their locations; helps install missing tools from official vendors.
- Opens Steam/Epic one step at a time, then rechecks when you return. Epic sign-in and Unreal 5.8 installation use Epic's normal screens.
- Prepares the isolated cooker and captures mappings in the background of the guided flow. It closes only a capture game it can prove it launched; existing matches and loaders are preserved.
- Resumes interrupted setup on next launch and provides progress, cancellation and receipt-checked recovery.
- **Start creating** reads the selected starter's body, clothes and rig automatically; there is no separate exporter step.
- Optional character-editing setup covers MetaHuman data, C++ tools and locally preparing Skin Details.

Extract the entire ZIP, then open **RoweMod Studio.cmd**. After setup, create **DeShawn**, choose **Downloads → ROWE Pants → Download & add to character**, and **Build and Play**. See STUDIO-FIRST-RUN.md and FRIEND-TEST.md.

Verified against the released DLL: 127 isolated UI checks, 24 automatic setup checks, 43 setup/recovery checks and 32 installer/download checks. The actual package marker and helper distribution drive the first-run checks. Windows validated the real Microsoft runtime download, installed vendor signatures and Windows Installer catalog signature without executing an installer. Process-ownership fixtures also passed; no actual fresh game capture was run for this update.

Fresh-PC setup-to-match, vendor installation acceptance and two-PC multiplayer remain unverified. The preceding 0.2.64 binary completed a real isolated clothing cook; that result does not claim fresh-PC gameplay for 0.2.65. New MetaHuman geometry/hair still needs game preparation. Game/engine/data and proprietary decoder payloads are not bundled. Five pinned ImageSharp advisories remain documented in DEPENDENCY-STATUS.md. Previous releases remain available.


# RoweMod Studio 0.2.64 beta

Fresh setup now checks the supported game build before authoring and offers **Finish mapping recovery** for Studio's own unchanged temporary capture loader after the game closes. Existing or modified loaders are preserved.

- **Choose cooker folder** is available in Settings for missing drives or custom locations.
- **Copy setup report** provides the Studio version and actionable checks for support.
- Native helper checks cover their actual x64 C++ runtime imports.
- The portable first launch opens Settings automatically.
- MetaHuman skin-map comparisons accept bounded static PNGs and exclude ICC/EXIF metadata while preserving exact RGBA/reset behavior.
- Release packaging checks binary/version agreement and excludes developer debug paths.

Download and extract the whole ZIP, then open **RoweMod Studio.cmd**. Install your own Hood Warfare 2, Blender 5.x and Unreal 5.8. Follow **Settings → Read game assets**, **Create character → DeShawn**, then **Downloads → ROWE Pants → Download & add to character → Build and Play**. See FRIEND-TEST.md and STUDIO-FIRST-RUN.md.

Verified: 67 isolated UI checks, 43 setup/recovery checks, 26 PNG checks and 34 skin handoff/reset checks against the release binary. The same binary completed Unreal clothing import/cook, rig checks and IoStore validation from a folder containing spaces. These tests did not install the package into the game.

This is an early testing beta: independent fresh-PC gameplay, local Skin Details extension compilation and two-PC multiplayer remain unverified. A new MetaHuman head/body/hair still needs game preparation. External licensed engine/data, proprietary compression decoder, private characters and full body references are not bundled.

Five ImageSharp dependency advisories remain in the pinned CUE conversion dependency. The input repair is not a dependency patch; see DEPENDENCY-STATUS.md for current scope and the supported-upgrade task. Previous 0.2.63 remains available for comparison and recovery.


## Studio 0.2.63 beta


RoweMod Studio now gives clothing its own workspace and a guided path from a matching body/rig to editable clothes for Hood Warfare 2. Start with a classic character, get a fitting kit, fit and weight your mesh in Blender, optionally paint it in Substance, then import and **Build and Play**.

- Separate **My characters** and **My clothes** pages, explicit garment choices and contextual **Make clothing / Textures / Model / Share** tools.
- **Downloads → Download & add to character** downloads curated clothes, asks who will wear them, verifies the package and imports only that garment. Original character parts and external source files are preserved.
- A first-run **Settings** checklist finds local Steam, Blender 5.x and Unreal 5.8 installations, including custom locations. Missing tools have official setup links. The app's .NET runtime is included; game and engine installations remain external.
- Handles Windows folder names with spaces when running Unreal Python helpers.
- Automatic local cooker creation and editable garment packages with rig/body-fit checks. Version 3 allows small position rounding between independent exports without accepting a different body, topology, weights or rest rig. Version 2 imports remain supported.
- Actual MetaHuman Creator handles character viewing and skin authoring. Optional Skin Details ships as source and can be built against the recipient's installed editor using **Settings → Build Skin Details extension**.

Download asset: [RoweMod-Studio-0.2.63-Windows.zip](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.63/RoweMod-Studio-0.2.63-Windows.zip).

Install Hood Warfare 2, Blender 5.x and Unreal Engine 5.8, extract the full ZIP, open **RoweMod Studio.cmd**, and follow **Settings → Read game assets**. Create a **Classic DeShawn** character for the ROWE Pants test. If a Visual C++ runtime DLL is missing, use [Microsoft's x64 runtime](https://aka.ms/vc14/vc_redist.x64.exe).

MetaHuman editing additionally needs Epic account sign-in and **MetaHuman Creator Core Data**. The optional local extension build needs Visual Studio C++ tools and a Windows SDK; that is separate from the Visual C++ redistributable. A new head/body/hairstyle still requires game preparation beyond skin-map import.


**Verified locally:** 56 UI checks, 28 package checks, 15 body-fit regression checks, and an independently exported Classic DeShawn recipient import. No personal projects, game bodies, Unreal binaries or MetaHuman data are bundled.

**Early testing limits:** a completely fresh PC has not completed setup-to-match; local Skin Details compilation and two-PC multiplayer still need acceptance. New MetaHuman head/body/hair preparation remains separate.

Extract the entire ZIP, follow Settings, then Create character → DeShawn → Downloads → ROWE Pants → Download & add to character → Build and Play. See the included FRIEND-TEST.md and STUDIO-FIRST-RUN.md guides.

The portable workspace also completed Unreal garment import, cooking, rig validation and IoStore container validation from a folder containing spaces. No game installation was changed by that test. The first cook compiles shaders and can take several minutes.

## ROWE Pants 0.1.1

Same garment and artwork as 0.1.0; version-3 body-fit evidence fixes independent FBX export rounding. Use Studio 0.2.63 or later. Original 0.1.0 remains available.
