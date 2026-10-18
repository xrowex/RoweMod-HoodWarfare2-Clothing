# RoweMod Studio 0.2.108 beta — save clothing in Blender

Each clothing item now has an Edit in Blender action and its own persistent working file inside its project. Reopening reuses that file. Save and close Blender, then Build & launch automatically reads changed clothing into a private game-preparation copy; no FBX export or import picker is required. Missing files are reported and never silently replaced. Existing explicitly selected working files stay linked.

The kit has one game rig, a dedicated EDIT CLOTHING collection, and the body, face and other clothing as references. Replacement meshes inside EDIT CLOTHING are recognized for that item's slot without manual custom-property editing. Fit and weight garments manually; this does not add missing native slots or automatic cross-character fitting.

Blender includes visible ROWE - START HERE instructions and a ROWE sidebar with persistent manual checkmarks for fitting, weights and posing. Check rig & weights checks for one rig and bone weights on each garment vertex. It does not verify good fit, clipping or animation quality. Save & close Blender stores the work and checklist. Studio refreshes its clothing page when that editor process exits; no periodic scan is added.

Existing source artwork, rig files and saved garment versions are preserved. Manually edited working clothes are excluded from the MetaHuman starter refitting pass. Final movement, appearance and clipping checks in game remain required for each garment.
