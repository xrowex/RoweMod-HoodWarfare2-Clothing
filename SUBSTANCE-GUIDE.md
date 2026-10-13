# Paint clothing in Substance Painter

You can change clothes on an existing saved character. You do not need a new character or rigging for a texture edit. Duplicate the character only if you want both outfits available as separate selectable versions. Clothing currently belongs to the saved character; independent wardrobe slots are not implemented.

## 1. Get the matching files

In Studio 0.2.73 or newer: **My characters → Customize → Start here → Choose clothes → choose item → Repaint item → Export FBX & textures**.

Studio opens the export folder. Open the selected item folder, then **Mesh** for its FBX and **Textures** for its PNGs. The export includes only that item, plus a `START-HERE-Substance.txt` guide. Keep the FBX's original UVs and material names. If the garment has several materials, its PNGs are prefixed by material number; match each group to the corresponding Painter texture set.

## 2. Open it in Painter

1. **File → New**: select the garment FBX. Use **DirectX** normals, **Compute tangent space per fragment** on and **Auto-unwrap** off.
2. Import the matching **Base** and **Normal** PNGs as **texture** resources into this project.
3. Add a fill layer. Assign the Base PNG to **Base Color** and Normal PNG to **Normal**, with UV scale **1**. Paint in layers above it. For several materials, repeat for each texture set.

Embedded FBX textures do not replace this layer setup. Do not also load the same Normal into the baked mesh-map slot: that would apply it twice. The original clothing Mask controls game-specific regions; keep it for the return step. It is not a generic Substance occlusion/roughness/metallic map.

## 3. Return the painted maps

Export separate PNG **Base Color** and **Normal DirectX** for each material, at the original texture resolution. The combined Normal DirectX output includes normal/height work. The current clothing shader does not import Substance ORM or Emissive; those channels are not a full PBR roundtrip.

Return to **the same saved character → Clothes → the same item → Textures → Import texture set**. Choose the matching material, select the exported Base and Normal PNGs, and keep the existing Mask. Studio copies the chosen maps into the saved creation. Do not import the FBX again for a texture-only change.

Choose **Build and Play** to apply the maps, then check the character in game. Editing or importing files alone does not install them. To share a compatible finished item, use that item's **Share → Export package**.

If something looks wrong, send the Studio and Painter versions, the item name, and cropped screenshots of Painter's viewport/Texture Set List and Studio's Task details. Do not send passwords or login codes.

Official Adobe references: [Project creation](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/getting-started/project-creation), [Normal-map painting](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/painting/advanced-channel-painting/normal-map-painting), [Output templates](https://experienceleague.adobe.com/en/docs/substance-3d-painter/using/export/export-window/output-templates).
