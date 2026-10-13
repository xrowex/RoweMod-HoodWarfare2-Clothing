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

## Automatic updates

Studio checks and downloads verified updates in the background when it opens. Close Studio when ready; it waits for the game and Unreal Editor to close, updates program files and reopens Studio. Creations, artwork, settings and exports remain saved. Interrupted updates use guarded rollback. Settings provides Keep Studio updated automatically and Check for updates. Studio 0.2.70 and newer receive this update automatically when enabled. Versions earlier than 0.2.70 need one manual download.

## Downloaded local acceptance and 0.2.70 team repair

The actual public 0.2.68 download passed automatic mapping setup/cleanup, classic DeShawn creation, catalog pants import, Unreal cooking and installation from an empty Studio workspace on the developer PC with tools already installed. Its Bloods target exposed a clothing issue; 0.2.70 corrects that target with 33 isolated creator checks. The exact final cosmetic Lua was tested in the modified public 0.2.68 workspace on both teams, after a restart and in a user-confirmed Bloods match. A first helper test preserved 532 user/generated files with mocked publisher responses. A separate production HTTP test then fetched the live public feed and ZIP, preserved 61 existing files and reopened normal Studio with the saved character. Public 0.2.70 also passed fresh setup and mapping capture on this PC. Full untouched 0.2.70 authoring-to-match, another PC with missing vendor tools and multiplayer remain unverified.

## Public 0.2.70 acceptance update

The unchanged public ZIP passed first-run setup and real mapping capture from an empty Studio workspace on the developer PC, using already-installed vendor tools. The capture game closed automatically and its temporary loader/path changes were restored automatically. Two native game saves changed while the game was running; the test coordinator preserved those generated versions and manually restored the protected originals. Studio does not automatically restore native saves.

A separate upgrade from a 0.2.69 fixture used the shipped production HTTP transport to fetch the live release feed and this exact public ZIP. The real updater helper completed all seven installation/preservation checks, kept 61 existing user/generated files byte-identical, retained recoverable old program files and reopened normal Studio. The saved character, enabled automatic-updates setting and up-to-date status were observed in that restarted GUI.

This verifies public 0.2.70 setup/capture and live update/helper/restart on the developer PC. It does not verify an untouched full 0.2.70 authoring-to-match workflow, missing-vendor installation on another PC or multiplayer. Earlier 0.2.68 authoring/cook/install and exact final cosmetic Lua tests remain separate evidence. The ZIP and DLL hashes are unchanged.

## Guided MetaHuman setup

In Studio 0.2.71 open **Settings → Set up MetaHuman Creator**. Review storage/performance advice before continuing, then complete the required Epic or compiler step and return for a recheck. Choose **Use clothing tools for now** to skip optional character editing. [MetaHuman setup guide](METAHUMAN-SETUP-GUIDE.md) explains matching engine data, plugins, sign-in, local extension tools and recovery. Exact install sizes come from Epic Options; 150 GB is a RoweMod planning estimate. The successful 0.2.70 local setup/updater tests above remain separate from the new guide UI checks and unverified missing-vendor installation on another PC.

The final 0.2.71 guide was visibly checked through Settings, the initial review and Continue. Actual local BuildPlugin compilation succeeded and the matching extension was installed, with Unreal 5.8.3, Creator Core Data and C++ tools already present. A real helper update from a 0.2.70 fixture reopened Studio and preserved 13 user/generated files; staging used mocked publisher HTTP responses. Missing-vendor installation, Epic sign-in and a newly published live 0.2.71 update remain unverified.

## Clear next steps in Studio 0.2.72

Open **My characters → Customize → Start here**.
- Choose **Edit character** for MetaHuman, skin maps and the return/import steps.
- Choose **Choose clothes**, select the item, then pick **Repaint**, **Make a new mesh**, or **Add a clothing package**. Follow only that path.
- Finish with **Build and Play** at the top right. Editing files does not install the mod by itself.

Starting outfit and advanced model choices are under **Starting outfit & advanced options** when creating a draft. Your existing characters and artwork stay saved.
