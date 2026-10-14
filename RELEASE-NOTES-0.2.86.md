# RoweMod Studio 0.2.86 beta

Stock fabric exports now contain a baked Base Color instead of the white DetailTex_Color input. Studio evaluates the installed game material on the selected garment in an isolated Unreal project, preserving all source UV channels and applying its native material inputs. A matching installed Unreal editor and common MetaHuman fabric content are required for this authoring export; the helper is included precompiled.

Existing enabled Base artwork, including intentionally white artwork, stays unchanged. Original meshes, projects, Mask and Normal files are preserved. Exported FBX files embed matching maps and pass independent rig, UV and weight roundtrip checks.

When returning Base Color from Substance, leave **Keep PNG colors exactly (recommended for Substance)** checked in **Import texture set**. This prevents applying team tint twice. Preserve the original region Mask; it is not an ORM map. This is a Base Color bake, not full PBR or lighting parity.

Verified with real Bri pants exports for both native team materials: eight UV channels, 2048px textured Base Color, preserved original maps and independent FBX roundtrips. Custom-artwork preservation and application self-tests also pass. No new Painter UI, friend-PC or gameplay acceptance is claimed. Private Send to Rowe support remains.

Update in Settings, then close Studio, Unreal and the game to apply it. Re-export the garment for Substance; no repainting or refitting is needed.
