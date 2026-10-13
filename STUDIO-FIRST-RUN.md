# First run — Studio 0.2.77

Extract the entire [Studio ZIP](https://rowemods.com/studio) into a writable folder and open **RoweMod Studio.cmd**. Keep its folders together. Codex and a .NET SDK are unnecessary.

Choose **Set up for playing** for prepared downloads: supported Steam game and cosmetic runtime only. Choose **Set up for creating** for Blender and matching Unreal export/fitting/cooking. Creator setup detects installed tools, guides official installs and automatically handles the one-time mapping capture and cleanup. Complete vendor sign-in/license/install prompts yourself and return to Studio. Use Unreal **5.8.3**. Optional MetaHuman tools are needed only for character editing.

Finish existing matches before setup. Studio only closes capture processes whose ownership it proves, and preserves changed/unowned loaders or packages as conflicts.

## Play

**Downloads → item → Subscribe**, then **My characters → matching wearer → Choose an outfit → Play with outfit**. Select that player in game and use the native Wardrobe for compatible stock/prepared clothes. A `.roweplay` is prepared; a `.roweclothes` contains editable creator sources and needs a build.

## Create

- **Make clothes:** choose a starter and slot, **Prepare fitting kit** once, fit/weight in Blender and save the same working file. **Build & launch game** automatically reads the selected garment before cooking. Already have the fitted file? Choose **Use an existing Blender file**. Use **Choose another saved file** after Save As. Textures/Substance are optional. Confirm **Looks good in game** only after a play check.
- **Edit textures:** starter → item → **Export model & textures → Artwork → Import texture set → Use saved artwork & continue → Build & launch game**.
- **Make a new character:** name it → **Create new MetaHuman**. Then choose Open in MetaHuman Creator; select a preset or adjust face, body and hair in the fresh source. Continue its inactive source draft from Create. Skin import transfers maps only. **Prepare Body & Face for the game rig** requires exporting your new geometry in Unreal, adapting both parts to the native rig, then importing/building them. The draft is not an extra game player until that preparation succeeds; hair needs separate binding. Existing stock/custom players are not cloned.
- **Edit a stock player:** **My characters → player → Edit this game character**. Edit textures or meshes (Body, Head & face or clothes) while retaining the original player identity.

My characters contains stock and installed custom identities. My clothes groups clothing and its prepared source fits. Green body references in fitting kits are not game garments. Several labeled body fits can share one working Blender file; Studio imports the selected profile, not the whole scene. New geometry still needs manual fitting and full rig weights.

**Settings → Set up MetaHuman Creator** guides optional Core Data, sign-in and C++ tools. [MetaHuman guide](METAHUMAN-SETUP-GUIDE.md).

## Recover and update

Changed working files/maps require a new build and play check. Failed/canceled actions do not complete steps. A missing working file offers relocation. Restore a missing enabled PNG using Import PNG/Import texture set on its exact item/material; reset cannot recreate a lost original. Interrupted capture recovers through setup with the game closed. Keep original art and avoid deleting unknown conflicts.

Studio updates retain user data. Close Studio, the game and Unreal to apply. Versions before 0.2.70 need a manual download. Mod updates are separate subscriptions.

Portable/UI/file verification is not fresh-PC gameplay acceptance. Prior local developer wardrobe checks remain version-specific; independent friend-PC setup-to-match, extended movement and two-PC multiplayer remain outstanding. [Friend test](FRIEND-TEST.md) · [Substance](SUBSTANCE-GUIDE.md).
