# Character-specific outfits

Universal fitting and the modular in-game clothing selector were canceled on October 17, 2026. Each outfit is now authored for one selected character.

In Studio, choose **My characters → character → Clothes → Make clothes → Edit in Blender**. Studio prepares and remembers a separate Blender working file for that clothing item inside its project. Later edits reopen the same file. Save and close Blender, then choose **Build & launch**: Studio reads saved changes automatically into a private game-preparation copy. No second FBX export or import picker is needed.

The file contains one game armature, that character's green body/face references and its other clothes as references. Edit or replace the garment inside **EDIT CLOTHING**. New meshes in that collection are recognized automatically for this slot; fit and weight them to the provided rig. Studio does not reshape clothing or transfer its weights automatically.

Read the embedded **ROWE - START HERE** text or open the **ROWE** sidebar in Blender. Tick the manual fit, weight-transfer and movement checks as you complete them. **Check rig & weights** checks for one rig and bone weights on every garment vertex; it cannot prove good deformation or clipping. **Save & close Blender** stores your file and checklist. Test movement and clipping in game after building.

Character and slot tags prevent a saved kit from being imported into a different character. Ready-to-play downloads keep their exact body and game-rig compatibility checks. Shared and multi-character downloads are retired.

Existing artist projects, saved garments, textures, game packages and saves are preserved. Older shared sources remain accessible for manual recovery. The retired source is recoverable in `archive/modular-clothing-20261017/source-before-retirement.zip` and the adjacent `retired` directory.

Build, import and kit tests do not establish that every outfit is correctly fitted; each new outfit still needs movement and clipping checks in game.
