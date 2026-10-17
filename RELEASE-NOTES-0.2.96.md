# Studio 0.2.96 beta — Hair export, clothing and runtime fixes

MetaHuman hair export waits for editor initialization and asset compilation,
then records an explicit completion result. A failed attempt preserves its own
Unreal log, Python traceback, versions and source hashes for Send to Rowe.
Older unrelated export failures no longer substitute for the current attempt.
This fixes locally reproduced startup/completion failures; One's PC still needs
to run the update and submit a fresh report if its build fails.

The cosmetic runtime coalesces callbacks raised by its own mesh update instead
of scheduling another clothing pass. Normal heartbeats avoid detailed groom
property reads; explicit diagnostics retain them. Native changes arriving before
the queued frame still apply. These changes address unnecessary periodic work;
they are not a guarantee against every source of frame stutter.

Imported clothing uses its own material-slot names and packed Base/Normal maps,
including older saved Blender projects. Disabled texture choices stay disabled.
A disabled Normal node is supported. Saved artwork and earlier wardrobe versions
remain preserved. Rebuild an older garment once to refresh its material recipe.

Creator hair bindings include verified distance LOD handling and use a new recipe
so an older cooked hairstyle is rebuilt. Rebuild the character to apply this to
an existing hairstyle; the app update does not silently overwrite installed art.

Shared clothing authoring is a beta preview. New items start from the one-rig
master kit, with Top, Pants, Shoes, Gloves, Mask, Bandana and Hat targets. One
reusable garment can be adapted for a selected supported stock or prepared custom
wearer. Studio checks the exact body, rig and covered surface, caches verified
fits, and preserves the previous outfit when a fit fails. Shared bone names alone
do not establish fit. Strict hand/finger checks can currently refuse gloves;
all-body and all-slot gameplay acceptance is still in progress. Test fit,
animation, first person and map travel before publishing an item.

Validation includes queued skin-change and reentrant callback regression checks,
actor-scoped groom diagnostics, imported-slot dispatch and mesh-pose checks,
native hair export success/failure evidence, native material cooking and updater
ownership checks. Native cooking and isolated checks are distinct from friend-PC
or full gameplay acceptance. Existing ImageSharp dependency advisories remain
documented in DEPENDENCY-STATUS.md.
