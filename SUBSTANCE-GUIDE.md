# Paint clothing in Substance Painter — Studio 0.2.75

Repaint an existing item while keeping its mesh, UVs, game rig and weights. You do not need to add or duplicate a character. Keep finished versions in Wardrobe; authored characters also support named outfit presets.

## Get the exact item

Use **Create → Edit textures → Start texture edit**, select a saved character's item or game starter, then **Export FBX & textures** in **Next step**.

For downloaded authoring sources, use **Browse mods → Get creator files → My mods → Edit creator files**. A compiled `.roweplay` is for playing; editable `.roweclothes` files are the authoring route.

The item export contains its FBX under **Mesh**, matching Base/Mask/Normal PNGs under **Textures** and `START-HERE-Substance.txt`. Preserve UVs and material names. Material-number prefixes identify separate Painter texture sets.

## Paint

1. **File → New**: select the FBX. Use **DirectX** normals, **Compute tangent space per fragment** on and **Auto-unwrap** off.
2. Import the matching Base and Normal PNGs as texture resources.
3. Add a fill layer with Base in **Base Color**, Normal in **Normal**, UV scale **1**. Paint above it. Repeat for each material set.

Embedded FBX media does not create Painter layers. Do not also apply the same Normal as a baked mesh map. The original game Mask is not Substance ORM; preserve its channel layout.

## Return to Studio

Export separate PNG **Base Color** and **Normal DirectX** for each material at the original resolution. The combined Normal includes your normal/height work. The current clothing shader does not accept a complete ORM/Emissive roundtrip.

Return to the **same item project → Textures → Import texture set**. Select the corresponding material and Base/Normal PNGs, keeping its Mask. Studio copies them into the project. A texture-only edit does not need another FBX import.

Click **Build & test** to prepare/install the saved changes and check them in game. Importing files alone does not install them. On an authored wearer, **Wardrobe → Keep current item** preserves a garment version and **Save outfit** keeps named presets on the same character.

## New meshes and skin

For a different garment shape, use **Create → Make clothing → Start clothing mesh → Export body & fitting kit**. Fit around the supplied body, preserve the game armature/vertex-group names, transfer and check full weights in Blender, and finish UVs before painting. Use **Import finished mesh**, import its matching maps and **Build & test**. Studio checks compatibility; it does not automatically fit or weight a new mesh to another body.

MetaHuman tattoos/scars use **Create → Make a character → MetaHuman Creator → Skin Details**, or that character's matching skin export for external painting. Body and garment UVs are different. Skin-map handoff alone does not prepare changed head/body geometry or hair.

## Missing maps and sharing

Restore the exact missing enabled map with **Import PNG** or **Import texture set**. A missing optional Mask can remain disabled; enabled missing maps must be restored before capture/build. Reset cannot recreate pixels from a lost original. Originals and unselected maps are preserved.

Use **Share → Export package** for editable creator sources. A curated ready-to-play release separately needs a verified cook, exact game/body/rig profile and publisher acceptance. There is no automatic public upload or verified cross-player wardrobe synchronization.

For issues, send Studio/Painter versions, item/material name, exact error and cropped viewport/texture-set screenshots. Keep the FBX, Painter project and exported PNGs.

Official Adobe references: [Project creation](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/project-creation), [Normal-map painting](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/painting/advanced-channel-painting/normal-map-painting), [Output templates](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/export/export-window/output-templates).
