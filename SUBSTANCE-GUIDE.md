# Paint clothing in Substance Painter — Studio 0.2.80

Repaint an existing item while keeping its mesh, UVs, game rig and weights. You do not need to add or duplicate a character. Keep finished versions in Wardrobe; authored characters also support named outfit presets.

## Get the exact item

Use **Create → Edit textures → starter card → item card → Export model & textures**. The heading always names your item and wearer.

For downloaded authoring sources, use **Downloads → Get creator files → Edit creator files**. A compiled `.roweplay` is for playing; editable `.roweclothes` files are the authoring route.

The item export contains its FBX under **Mesh**, matching Base/Mask/Normal PNGs under **Textures** and `START-HERE-Substance.txt`. Preserve UVs and material names. Material-number prefixes identify separate Painter texture sets.

## Paint

1. **File → New**: select the FBX. Use **DirectX** normals, **Compute tangent space per fragment** on and **Auto-unwrap** off.
2. Import the matching Base and Normal PNGs as texture resources.
3. Add a fill layer with Base in **Base Color**, Normal in **Normal**, UV scale **1**. Paint above it. Repeat for each material set.

Embedded FBX media does not create Painter layers. Do not also apply the same Normal as a baked mesh map. The original game Mask is not Substance ORM; preserve its channel layout.

## Return to Studio

Export separate PNG **Base Color** and **Normal DirectX** for each material at the original resolution. The combined Normal includes your normal/height work. The current clothing shader does not accept a complete ORM/Emissive roundtrip.

Return to the **same item**. In the Edit textures task use **Artwork → Import texture set**. In a saved Blender clothing task expand **Optional · textures, Substance & sharing → Import texture set**. Select the corresponding material and Base/Normal PNGs, keeping its Mask. Studio copies them into the project. A texture-only edit does not need another FBX import.

In the Edit textures task click **Use saved artwork & continue → Build & launch game**. In the saved Blender clothing task click **Build & launch game** directly; artwork is optional. Check the item in a match, then click **Looks good in game** in Studio. Importing files alone does not install them. On an authored wearer, **Wardrobe → Keep current item** preserves a garment version and **Save outfit** keeps named presets on the same character.

## New meshes and skin

For a different garment shape, use **Create → Make clothes → starter → clothing slot → Prepare fitting kit** once. Fit around the green reference body, preserve the game armature/vertex-group names, transfer/check full weights and finish UVs in Blender. Save the same working file. **Build & launch game** reads only the selected garment/body profile automatically; there is no required second FBX export/import. Already have a fitted and weighted file? Choose **Use an existing Blender file**. Save As can be remembered with **Choose another saved file**.

Substance is optional. In the saved clothing workflow expand **Optional · textures, Substance & sharing → Export this item for Substance**, paint that exact selected garment and bring the maps back through its texture tools. Keep existing good maps if no texture edits are needed. Studio checks compatibility; it does not automatically fit or weight new geometry to another body. Green body/weight references are not included as garment meshes. Prepared source fits grouped in My clothes still need Build and a play check.

MetaHuman tattoos/scars use the actual Creator’s **Skin Details**, or the matching skin export for external painting. **Create → Make a character → Create new MetaHuman** creates a new source; it does not clone a game player. The source draft needs explicit new Body and Face game-rig preparation before a native build can activate it. Imported skin maps alone do not prepare geometry or hair. Body and garment UVs are different. For existing stock skin, choose **My characters → player → Edit this game character → Edit textures** without duplicating the player.

## Missing maps and sharing

Restore the exact missing enabled map with **Import PNG** or **Import texture set**. A missing optional Mask can remain disabled; enabled missing maps must be restored before capture/build. Reset cannot recreate pixels from a lost original. Originals and unselected maps are preserved.

Use the saved clothing workflow’s **Optional · textures, Substance & sharing → Share clothing package → Export package** for editable creator sources. A curated ready-to-play release separately needs a verified cook, exact game/body/rig profile and publisher acceptance. There is no automatic public upload or verified cross-player wardrobe synchronization.

For issues, send Studio/Painter versions, item/material name, exact error and cropped viewport/texture-set screenshots. Keep the FBX, Painter project and exported PNGs.

Official Adobe references: [Project creation](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/project-creation), [Normal-map painting](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/painting/advanced-channel-painting/normal-map-painting), [Output templates](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/export/export-window/output-templates).
