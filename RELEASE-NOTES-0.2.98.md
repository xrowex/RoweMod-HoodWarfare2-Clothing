# Studio 0.2.98 beta — Outfit rendering repairs

Keep cached cosmetic assets tied to their exact Unreal object path. A valid
object wrapper reused after a map change can no longer be mistaken for the
requested shoes, clothing mesh, pose or texture.

Keep replacement hair and native masks attached to their recorded owner.
Visibility maintenance updates only changed state and avoids loading assets
during idle play. Stock wardrobe changes also respect the selected local body.

Reusable clothing now retains supported native fabric materials in its private
game build. The material, functions and textures are cooked into the garment's
own namespace, with skeletal mesh and morph support. Edited artwork continues
through its separate material path. Currently this native fabric preparation
supports the MetaHuman M_fabric_simpler graph; other graphs need validation.

Local validation: one newly authored pants download rendered on Tyreese,
DeShawn, Darnell and Bri in Player Select. Bri wore that same package after a
map change and respawn, with the expected blue fabric, shoes and hair visible
at the normal third-person camera distance and both shoulders. This is a bounded
local test, not acceptance of every body, slot, hairstyle or another PC.

Includes the 0.2.97 recurring catalog-reload hitch repair. A separate 45-second
steady private-match capture using Bri's saved outfit recorded 3,983 frames,
none over 50 ms; the slowest was 48.5 ms. Initial spawn and map loading still
take time. These captures do not guarantee stutter-free play on every PC.

Universal clothing remains a preview. Strict fitting checks can refuse an
invalid garment and retain the prior outfit. Remaining slots, arbitrary custom
bodies and the complete publishing/download workflow still need gameplay tests.
One's MetaHuman issue still requires confirmation on his PC.

Close the game before updating, then relaunch through Studio to refresh the
cosmetic runtime. Existing saved projects, character sources and artwork remain
preserved. Rebuild older hair to receive the distance-LOD recipe from 0.2.96.
