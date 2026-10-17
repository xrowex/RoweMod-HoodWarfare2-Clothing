# Studio 0.2.97 beta — Match hitch repair

Native character catalogs created during loadouts and bot respawns no longer
trigger a full restore and reload of every live cosmetic. Catalog changes now
refresh the extra character-list entries only. A person's character selection,
native mesh resets, and explicit texture reloads still update their cosmetics.

Local private-match validation: the earlier 30-second capture had five frames
over 250 ms (worst 420.7 ms). A 45-second capture after the fix had none over
250 ms (worst 101.0 ms; two frames over 50 ms). Catalog notifications continued
without additional full cosmetic passes. These are bounded captures from the
same map and bot setup, not a guarantee of stutter-free play on every PC.

Runtime diagnostics include bounded counts and timings for cosmetic application,
catalog changes, networking, and wardrobe preparation. These make a periodic
stall distinguishable from normal idle polls without enabling detailed groom
reflection or collecting input.

Includes the hair-export diagnostics, clothing material fixes, distance-LOD hair
recipe, and shared clothing authoring preview from 0.2.96. Existing hairstyles
need a character rebuild to receive the distance-LOD recipe. One's PC still needs
to test its own MetaHuman build; local success is not friend-PC acceptance.

Universal clothing remains a preview: automatic fits are checked against the
selected supported stock or prepared custom body. Strict finger checks can refuse
gloves. All-body, all-slot animation and gameplay validation remains in progress.
Existing artwork, saved projects, wardrobe choices, and original files are kept.

Close the game before updating and relaunch it through Studio to refresh its
installed runtime. See RELEASE-NOTES-0.2.96.md for the preceding changes and
DEPENDENCY-STATUS.md for existing dependency advisories.
