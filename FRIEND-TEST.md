# Friend test — RoweMod Studio

Download the current [Windows Studio beta](https://rowemods.com/studio). This is the complete portable app and clothing workflow; you do not need Codex, a .NET SDK or files from the developer's PC.

## Start

1. Extract the entire ZIP into a writable folder, then open **RoweMod Studio.cmd**.
2. The setup screen opens and starts automatically. Complete any official installer/license prompts. In Epic, sign in and install **Unreal Engine 5.8** when requested, then return to Studio. The checklist rechecks and continues. Close an existing game match before the one-time game setup. Mapping capture, capture-game closure and temporary-loader recovery are automatic.
3. Studio opens character creation when setup finishes. Select classic **DeShawn**, name your new character and click **Create and customize**. Studio exports its body, clothes and rig automatically from your own game. If setup needs attention, this button opens it and continues with your choices when ready.
4. Choose **Downloads → ROWE Pants → Download & add to character** and pick that character.
5. Close the game, choose **Build and Play**, then select your custom character in game.

The ROWE pants fit Classic DeShawn; Aqua needs a different fit. Their authored orange color should remain on both teams. First-time shader preparation can take several minutes; progress and Cancel remain available. The matching game version is checked before mapping capture or cosmetic installation.

## Tell us what happens

Check both teams, then walking, jumping, aiming, reloading and firing in third person. Check a respawn and close/reopen the game to verify saved selection. Confirm stock characters are still available. Send the Studio version, the checklist result and whether the pants stay correct in the match.

If something fails, open **Setup details** or **Settings → Advanced setup → Copy setup report** and include the exact message. Interrupted mapping setup recovers through the same **Set up automatically** button once the game closes. An unchanged existing RoweMod loader is paused and restored automatically. Changed or unowned loaders are preserved.

## Test making clothes next

Open **My clothes → your wearer → garment → Make clothing → Get fitting kit**. Follow `START-HERE.html` in the exported kit. Fit your garment to the included body, transfer and check weights in Blender, then import the finished mesh into the same Studio garment. You can paint its final UVs in Substance and import Base Color and DirectX Normal PNGs. Keep the existing Mask; the clothing shader does not use Substance ORM or Emissive. Build and repeat the movement checks.

To exchange a garment, use **Share → Export package**. Import it into another compatible wearer. A different body or rig needs a fitting kit for that wearer. The in-app Downloads catalog contains curated releases; it does not automatically publish a friend's artwork.

## Recovery and optional editing

Use a disposable disabled creation for deletion: **My characters → test creation → More… → Delete…**, then **Recently deleted → Restore creation**. The restored draft should stay disabled. Keep your main artwork untouched. Recovery files remain under `dumps/deleted-mods`; preserve that folder if moving Studio.

The setup wizard's **Character editing (optional)** section covers MetaHuman Core Data and the locally built Skin Details extension. Clothing testing does not require it. See [STUDIO-FIRST-RUN.md](STUDIO-FIRST-RUN.md) for that route. A brand-new MetaHuman head/body/hair still needs game preparation; a skin-map import alone does not complete it.

This fresh-PC setup-to-match test is the remaining clothing acceptance gate. Multiplayer needs a separate two-PC test; local success does not verify network visibility. See [DEPENDENCY-STATUS.md](DEPENDENCY-STATUS.md) for the beta's dependency limitations.

## Mapping launch repair in 0.2.68

This version gives the capture game its Steam identity only during its own launch, then restores the process environment. You do not need to enter Steam launch options or change Windows environment variables. Capture configuration is written without a UTF-8 byte-order mark. After a failed older attempt, close the capture game and reopen the setup wizard; Studio verifies the recorded loader and runtime path before recovery. Never delete a changed or unrelated loader to force setup. This public ZIP still needs independent fresh-PC setup and match acceptance.
