# Set up RoweMod Studio

Download [Studio for Windows](https://rowemods.com/studio), extract the entire ZIP into a writable folder, then open **RoweMod Studio.cmd**. Keep its folders together. Studio includes its .NET runtime; Codex and a separate .NET installation are unnecessary.

## Automatic setup

The setup screen opens and starts automatically on first launch, or when a required setup check is incomplete. You do not need to open Settings, scan assets or start mapping capture yourself.

Its checklist shows your game, Blender, Unreal Engine and game setup. Studio finds installed tools, saves their locations, prepares its isolated cooker and captures the game's mappings once. It closes only the capture game that it can prove it launched; finish your existing match and close the game before starting setup. Your characters, artwork and stock players stay saved.

If a tool is missing, Studio opens the official installation path. Complete the vendor's license and Windows permission prompts. Unreal Engine **5.8** is installed through Epic Games Launcher: sign in, select that version and start its installation. Return to the setup screen; it checks again and continues when the requirements are ready. The engine and the game are supplied by their vendors, rather than bundled in the Studio ZIP.

When all required items are ready, Studio opens character creation automatically. Select a classic starter and name your character. Studio reads that starter's body, clothes and game rig from your own installed game automatically. If setup is needed after you click **Create and customize**, it opens the checklist, keeps your choices and continues creating when setup finishes.

To reopen setup later, use **Settings → Run setup wizard**. Normal use needs no manual paths. Custom installations, setup reports and recovery tools are under **Settings → Advanced setup**.

## Try the ROWE pants

1. Create a separate character from **DeShawn**, keeping his classic body.
2. Choose **Downloads → ROWE Pants → Download & add to character**, then select your new wearer.
3. Close the game and choose **Build and Play**. Select your custom character in game.

ROWE Pants 0.1.1 fits Classic DeShawn and keeps its authored orange colors on both teams. Aqua and other reshaped bodies need clothes fitted separately. The first build compiles shaders and can take several minutes; progress and Cancel stay available.

To make clothes, choose **My clothes → wearer → garment → Make clothing → Get fitting kit**. Open its `START-HERE.html` guide. The Blender kit contains the matching local body and rig. Fit and weight the garment, import the finished mesh, and optionally paint its final UVs in Substance before importing Base Color and DirectX Normal PNGs. Keep the existing Mask instead of importing an unrelated Substance ORM map.

## Optional character editing

Expand **Character editing (optional)** in setup to prepare MetaHuman editing. Epic supplies **MetaHuman Creator Core Data** through Unreal 5.8's Options. Creator handles Epic sign-in when it opens. Skin Details is built locally from the bundled RoweMod source with your installed Unreal editor and C++ development tools. Follow the optional checklist; save and close Unreal when the extension build asks. Clothing editing does not need these optional tools.

For a linked character, use **Open in MetaHuman Creator**, edit skin details there, then **Send to RoweMod → Import skin details** in Studio. New face/body shapes and hairstyles still need game-rig and hair preparation. Importing skin maps does not automatically prepare a brand-new MetaHuman mesh.

## If setup stops

Cancel stops Studio's current setup step safely; it does not terminate a vendor installer. Finish or close that installer before retrying. For interrupted mapping capture, close the capture game and run the setup wizard again. Studio restores only its recorded, unchanged temporary capture loader. An unchanged RoweMod loader is paused and restored automatically, including one installed by an older Studio folder. Changed or unowned loaders are preserved and reported.

Setup accepts the supported unprotected Steam build **25888787**. Unsupported/protected builds remain unavailable for capture and cosmetic installation; keep your artwork and use normal Steam play. For a failed check, expand **Setup details** or copy the report from **Settings → Advanced setup → Copy setup report**. Include the exact failed step when asking for help.

A fresh second PC still needs to complete setup and a match before this beta receives general release acceptance. Two-PC character visibility also remains unverified. See [FRIEND-TEST.md](FRIEND-TEST.md) for the short acceptance test and [DEPENDENCY-STATUS.md](DEPENDENCY-STATUS.md) for dependency limitations.

## Mapping launch repair in 0.2.68

This version gives the capture game its Steam identity only during its own launch, then restores the process environment. You do not need to enter Steam launch options or change Windows environment variables. Capture configuration is written without a UTF-8 byte-order mark. After a failed older attempt, close the capture game and reopen the setup wizard; Studio verifies the recorded loader and runtime path before recovery. Never delete a changed or unrelated loader to force setup. This public ZIP still needs independent fresh-PC setup and match acceptance.
