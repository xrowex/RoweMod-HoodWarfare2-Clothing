# Set up MetaHuman character editing

MetaHuman editing is optional. You can make and texture clothes in RoweMod Studio without installing MetaHuman data. For faces, bodies and hairstyles, open **Settings → Set up MetaHuman Creator** in Studio. Review storage and performance advice, then click **Continue setup**. The guide leads you through the required step and rechecks when you return from Epic or another installer.

## Choose where to install

Use an SSD with room for Unreal, optional content, downloaded character textures and generated project files. RoweMod recommends planning around **150 GB of free SSD space** for this workflow. This is our working budget, not Epic's download size or a fixed requirement. Existing installations and chosen components change the space needed.

Keep room for downloaded textures, generated assets and cooking files. A C++ extension build is not required for plain MetaHuman Creator.

For clothing-only setup, install the matching Unreal tools and leave space for the local cooker and exports. You do not need MetaHuman Core Data or C++ extension tools. The **150 GB** estimate applies to the full character workflow; it is not a fixed clothing-tools requirement. Studio's engine-only guide keeps those optional steps separate.

Epic Games Launcher shows the current component download and storage estimates in the selected engine's **Options** screen. Read those values before applying; there is no single fixed MetaHuman download size in this guide. Choose an installation drive with enough room for those estimates plus your projects and temporary cooking files. See [Epic's Unreal installation guide](https://dev.epicgames.com/documentation/en-us/unreal-engine/install-unreal-engine).

## Install the matching editor and character data

1. Open Epic Games Launcher → **Unreal Engine → Library**. Use **Unreal Engine 5.8.3**, the editor version used for this Hood Warfare 2 workflow. Sign in to Epic when prompted.
2. Save and close every Unreal project. On that engine's tile, open the arrow beside **Launch → Options**.
3. Select **MetaHuman Creator Core Data**, review the displayed download/storage values and click **Apply**. Let Epic finish installing.
4. Return to Studio's guided setup and recheck. Keep its engine path pointed at the same installation.
5. Open the character project through Studio. If Unreal asks about missing MetaHuman support, use **Edit → Plugins**, enable **MetaHuman Creator**, then save and restart the editor when prompted.

The data contains Creator presets, hair and texture resources. Enabling the project plugin alone does not download it. Follow [Epic's MetaHuman getting-started guide](https://dev.epicgames.com/documentation/metahuman/getting-started-with-metahuman-creator-in-unreal-engine?lang=en-US).

## What computer works well?

Epic recommends **32 GB RAM**, **8 GB VRAM**, a graphics card at least comparable to **RTX 3070 / RX 6800 XT**, and **16 physical high-performance CPU cores** for MetaHuman Creator/Animator. These are recommendations, not Creator minimums. High-resolution character assembly can exceed 32 GB memory. See [Epic's hardware guidance](https://dev.epicgames.com/documentation/metahuman/metahuman-hardware-requirements-in-unreal-engine?lang=en-US).

The editor renders on your local GPU. You do not need to rent a cloud GPU or run a streaming server. Epic does use online services for auto-rigging and texture synthesis, so keep internet access available and complete the editor's Epic sign-in yourself. Studio does not sign in for you. [Epic explains those services here](https://dev.epicgames.com/documentation/metahuman/getting-started-with-metahuman-creator-in-unreal-engine?lang=en-US).

## Keep editing responsive

Start with a moderate viewport quality while placing hair, marks and clothing; raise quality for your final appearance check. A smaller viewport and lower editing quality reduce GPU load without changing the saved design. Close other heavy applications before downloading large textures or assembling a rig. Initial shader preparation can take time; give the editor a chance to finish before retrying a button.

Keep Unreal and its project on an SSD. If performance remains poor, reduce viewport quality first and check available RAM, VRAM and disk space. The final game result still needs a match test; a beautiful Creator view does not verify game materials, rigging or clothing fit.

## Return to Studio

Save your face, body and hairstyle in Creator, then return to Studio and choose **Build & launch game**. Studio automatically assembles the saved source, adapts Body and Face to the native game rig, prepares compatible Creator hair/brows/lashes, fits the starter outfit and cooks the character. Blender must be installed, but it runs in the background: no manual Blender edit, FBX export or part import is required. Existing saved drafts use the same route. The original MetaHuman source stays intact; the draft becomes a selectable character only after preparation and build succeed.

Check Player Select, then movement and outfit fit in a match before **Looks good in game**. Advanced manual authoring is optional. For artwork, use Studio’s texture tools or Substance exports. Skin Details and its Send/Import workflow remain paused; no RoweMod extension or C++ workload is required.

Previously enabled RoweModSkinDetails entries are disabled when Studio next opens the project after Unreal has been saved and closed. Original project settings and saved artwork are preserved.

## If setup stops

- **Creator opens then closes:** update to Studio 0.2.83. Its opening helper keeps the interactive editor alive. If it still closes, send the final part of the Unreal project log from Saved/Logs or attach the full .log; startup-only excerpts cannot establish the final exit reason.


- **Core Data missing:** close all Unreal projects and check that the data was selected for the same engine installation Studio uses.
- **Plugin missing:** enable MetaHuman Creator in that project and restart Unreal after saving.
- **Sign-in or texture/rig download fails:** complete Epic's prompt, check internet access and retry. Restricted networks may block Epic's services.
- **An older version asks to build Skin Details:** update Studio to 0.2.83 or later and reopen it. That step is no longer required.
- **Storage warning:** use Epic's actual Options estimates and make room on the selected drive. Keep your character projects and artwork.

This guide accompanies Studio 0.2.84. Automatic preparation and the animated character-selection preview were verified locally with a fresh MetaHuman. Full-match deformation and installation of missing vendor components on another PC remain unverified. Use **Use clothing tools for now** to leave optional character setup without starting a download.
