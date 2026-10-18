# RoweMod Studio 0.2.109 beta — saved facial-hair selections

Fix the build failure for Goatee_L_Wavy and other grooms whose asset names do not identify a slot. Studio reads the saved character's wardrobe selections and their native groom bindings, so a goatee selected for Beard stays in Beard after assembly. This works for all six supported groom slots and copied custom names without loading a second Creator preview actor.

Resolve slots and reject ambiguous or duplicate bindings before generating transfer meshes. Reports include the saved selections and assembled binding identities when a slot cannot be resolved. Original characters, artwork and the previous working game build remain preserved.

Guided pages now distinguish hairstyle-slot errors, failed hairstyle export, missing Studio helpers and Blender preparation failures instead of hiding these behind a generic step-failed message. Full tracebacks remain available in Task details and support reports.

Fix editable face exports containing auxiliary materials such as MI_Face_LacrimalFluid, which has only a Normal map. Export the actual available channels, retain untextured utility materials such as M_Hide and their slot positions, and keep the existing independent FBX geometry/UV/weight verification. Do not fabricate blank Base or Mask files. Referenced editable-export logs now accompany the current operation in Send to Rowe, including logs from an earlier client after an update.

The updater can stage a verified same-version repair when an inventory-owned program file is missing. Modified program files and unlisted user content remain protected by the existing update transaction. Portable packaging also checks that runtime Python helpers referenced by Studio and their local imports are included, preventing another omitted Blender helper.

This changes export preparation and installation repair. Verification of One's next full Build & launch retry remains necessary.
