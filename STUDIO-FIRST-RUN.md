# Set up RoweMod Studio on your PC

Use [Studio 0.2.64 for Windows](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.64/RoweMod-Studio-0.2.64-Windows.zip). Extract the complete ZIP into a folder you can write to, then open **RoweMod Studio.cmd**. Keep the app, tools and guides together. The portable app includes its .NET runtime; you do not need Codex or a separate .NET installation.

Open **Settings** and review the setup checklist:

1. Install **Hood Warfare 2** through [Steam](https://store.steampowered.com/app/5155360/). Studio looks through your Steam libraries. If it does not find your copy, choose the folder containing `HW2` and the game's executable. Setup also checks the approved unprotected game build **25888787**. If it reports an unsupported/protected build, keep your artwork and use normal Steam play; capture and cosmetic installation remain disabled. Choose **Copy setup report** when asking for support.
2. Install [Blender 5.x](https://www.blender.org/download/). Blender 5.1 is the verified authoring version. Standard installations are found automatically; for a portable/custom installation, choose its `blender.exe` in Settings.
3. Install **Unreal Engine 5.8** through the [Epic Games Launcher](https://www.unrealengine.com/download). Epic sign-in is required. Choose 5.8 explicitly, rather than an older engine or another major/minor version. Studio detects the Epic installation wherever you installed it; it does not require an E: drive.
4. If you want MetaHuman character/skin editing, enable **MetaHuman Creator Core Data** in that engine's **Options**. [Epic's installation guide](https://dev.epicgames.com/documentation/metahuman/getting-started-with-metahuman-creator-in-unreal-engine?lang=en-US). This data and the Unreal engine are obtained from Epic, not included in the Studio ZIP.
5. Review **Skin Details extension** status. Studio ships its own extension source rather than Epic-linked editor binaries. To build it on your PC, install [Visual Studio or Build Tools](https://visualstudio.microsoft.com/downloads/) with **Desktop development with C++**, MSVC x64 tools and a Windows SDK. Save and close Unreal, then choose **Build Skin Details** in Settings. Studio builds against your installed Unreal 5.8, checks the exact engine BuildId and keeps any previous binaries in a recovery folder. The first C++ build can take several minutes. Clothing editing does not require this optional extension build.
6. Choose **Read game assets**. Capture the game's mappings once if requested: close your match, start the temporary capture, stay at the main menu, then close the capture game when finished. If keeping the game-content window open, click **Scan game** afterward. Studio reads the selected classic starter automatically when you create it. Bodies, game rigs and original clothing are obtained from your own installed game.

If Setup reports missing C++ runtime libraries, or Windows names `VCRUNTIME140`, `VCRUNTIME140_1` or an `MSVCP140` variant, install Microsoft's [Visual C++ v14 x64 runtime](https://aka.ms/vc14/vc_redist.x64.exe), then reopen Studio/the game. Studio checks all five runtime variants imported by its shipped helpers. This is separate from the C++ development tools needed for the optional Skin Details build. [Microsoft runtime instructions](https://learn.microsoft.com/en-us/cpp/windows/latest-supported-vc-redist?view=msvc-170).

Studio creates its isolated cooker folder automatically on your first **Build and Play**. A fresh portable setup stores it inside the Studio workspace. Existing explicitly chosen cooker folders stay selected; if that drive is unavailable, use **Settings → Choose cooker folder** and select a local folder dedicated to RoweMod. The first cook compiles shaders and can take several minutes; check **Details** for progress or use **Cancel** to stop safely.

The checklist inspects your PC without installing tools, changing game files or writing settings. Folder choices are saved only when you choose them. MetaHuman core-data detection does not sign you into Epic or prove its online services are available; Creator handles that sign-in when you open it.

## If mapping capture stops or fails

Close Hood Warfare 2, return to **Settings**, and choose **Refresh setup checks → Finish mapping recovery** when it is available. This removes only the unchanged temporary capture proxy recorded by this Studio workspace and its ownership receipt. Then retry **Read game assets → Capture mappings**. If recovery refuses a changed loader or a different game folder, keep those files and use **Copy setup report** plus the exact **Details** text when asking for help. An unavailable recovery button means Studio has no valid owned capture to remove; it does not authorize deleting another loader manually.

## Try the ROWE pants first

1. Choose **Create character**, select **DeShawn**, and name your new character. Keep his classic body for this test; Aqua and other reshaped bodies need clothes fitted separately.
2. Choose **Downloads → ROWE Pants → Download & add to character**. Select the DeShawn character you just created. Studio verifies the download and imports only its Pants item.
3. Close the game and choose **Build and Play**. Importing a download alone does not install it.
4. Select your separate custom character in the game. Check both teams, then walking, jumping, aiming, reloading and firing in third person. Restart once to check the saved selection.

To make your own clothes, use **My clothes → character → item → Make clothing → Get fitting kit**. The kit includes the matching body and rig plus a beginner guide. Fit and weight the garment in Blender, import the finished mesh, and optionally paint its final UVs in Substance before importing its Base Color and DirectX Normal textures.

The release has local authoring and game checkpoints; a completely fresh PC has not yet completed the full setup-to-match test. Creating a brand-new MetaHuman head/body/hair and preparing all of it for the game is not an automatic skin-map import. Two-PC character visibility is also still unverified. See [the friend test checklist](FRIEND-TEST.md).

## Check creation recovery safely

Use a disposable, disabled test copy: **My characters → your test creation → More… → Delete…**. Confirm its name before deleting. Then choose **My characters → Recently deleted → Restore creation**. The restored creation returns as a disabled draft; it is not installed automatically. Recovery artwork is kept in `dumps/deleted-mods` inside the extracted Studio folder. Keep that folder if moving Studio. If deleting an installed test creation, close the game first and restart afterward when Studio requests it. Keep your main character and original source files separate from this check.
