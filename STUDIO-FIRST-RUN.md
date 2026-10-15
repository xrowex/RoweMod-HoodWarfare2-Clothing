# First run — Studio 0.2.84

Extract the entire [Studio ZIP](https://rowemods.com/studio) into a writable folder and open **RoweMod Studio.cmd**. Keep its folders together. Codex and a .NET SDK are unnecessary.

Choose **Set up for playing** for prepared downloads: supported Steam game and cosmetic runtime only. Choose **Set up for creating** for Blender and matching Unreal export/fitting/cooking. Creator setup detects installed tools, guides official installs and automatically handles the one-time mapping capture and cleanup. Complete vendor sign-in/license/install prompts yourself and return to Studio. Use Unreal **5.8.3**. Optional MetaHuman tools are needed only for character editing.

Finish existing matches before setup. Studio only closes capture processes whose ownership it proves, and preserves changed/unowned loaders or packages as conflicts.

## Play

**Downloads → item → Subscribe**, then **My characters → matching wearer → Choose an outfit → Play with outfit**. Select that player in game and use the native Wardrobe for compatible stock/prepared clothes. A `.roweplay` is prepared; a `.roweclothes` contains editable creator sources and needs a build.

## Create

- **Make clothes:** **Choose a character**, choose its clothing slot, **Prepare fitting kit** once, fit/weight in Blender and save the same working file. **Build & launch game** automatically reads the selected garment before cooking. Already have the fitted file? Choose **Use an existing Blender file**. Use **Choose another saved file** after Save As. Textures/Substance are optional. Confirm **Looks good in game** only after a play check.
- **Edit textures:** starter → item → **Export model & textures → Artwork → Import texture set → Use saved artwork & continue → Build & launch game**.
- **Make a new character:** name it → **Create new MetaHuman → Open in MetaHuman Creator**. Select a preset and adjust face, body and hair; save, return to Studio and choose **Build & launch game**. Existing saved drafts work too. Studio automatically prepares the game rig, compatible Creator hair and starter outfit, then cooks the character. Blender runs in the background; no manual part export/import is needed. The draft becomes a selectable player only after the build succeeds. Check it in a match before confirming **Looks good in game**.
- **Edit a stock player:** **My characters → player → Edit this game character**. Edit textures or meshes (Body, Head & face or clothes) while retaining the original player identity.

My characters contains stock and installed custom identities. My clothes groups clothing and its prepared source fits. Green body references in fitting kits are not game garments. Several labeled body fits can share one working Blender file; Studio imports the selected profile, not the whole scene. New geometry still needs manual fitting and full rig weights.

Studio 0.2.88 adds **Create → Make clothes → Open kit in Blender** for the master clothing references. Studio prepares them from the installed game and opens an editable copy. Tyreese, DeShawn and Darnell have separate collections and original rigs, with green Body/Face references for clipping. Toggle one character collection at a time. Keep face and clothing rigs separate; matching bone names do not guarantee a matching body fit. Saved custom bodies are available through the item's fitting project. Reference meshes are excluded from clothing imports.

New MetaHuman drafts automatically use the complete master adapter with **Top, Pants and Shoes**. Opening the master in Blender is optional. Existing characters and artwork are preserved; this does not migrate an older character to a different body or rig.

**Settings → Set up MetaHuman Creator** guides optional Core Data and sign-in. Blender is required for background mesh preparation. Skin Details remains paused; no C++ workload is needed. [MetaHuman guide](METAHUMAN-SETUP-GUIDE.md).

## Recover and update

Changed working files/maps require a new build and play check. Failed/canceled actions do not complete steps. A missing working file offers relocation. Restore a missing enabled PNG using Import PNG/Import texture set on its exact item/material; reset cannot recreate a lost original. Interrupted capture recovers through setup with the game closed. Keep original art and avoid deleting unknown conflicts.

Studio updates retain user data. Close Studio, the game and Unreal to apply. Versions before 0.2.70 need a manual download. Mod updates are separate subscriptions.

Portable/UI/file verification is not fresh-PC gameplay acceptance. Prior local developer wardrobe checks remain version-specific; independent friend-PC setup-to-match, extended movement and two-PC multiplayer remain outstanding. [Friend test](FRIEND-TEST.md) · [Substance](SUBSTANCE-GUIDE.md).

If the old updater says **Studio archive contains an unsafe program payload**, update to 0.2.83. If the old inventory itself is rejected, close Studio, extract the full current ZIP into a new folder and launch its RoweMod Studio.cmd once. Keep the old workspace and all saved projects; do not delete or merge artwork to repair an update.
