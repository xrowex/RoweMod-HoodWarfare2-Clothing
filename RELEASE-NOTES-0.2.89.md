# Studio 0.2.89 — Short MetaHuman build paths

MetaHuman **Build & launch game** now creates its private Unreal job in a short
user-local cache, independent of the Studio installation folder. Deep Downloads
or OneDrive installation paths no longer add their length to generated texture
paths. You do not need to move Studio, your character project or your artwork.
After updating, retry **Build & launch game** on the same saved character.

Each new cache job records its exact workspace, character and source ownership.
Verified complete preparations from earlier versions remain reusable at their
existing locations. Failed builds retry in a new short job. Old source folders,
working files, prepared assets and artwork are preserved.

This update also discards destroyed character-preview references before reading
hair diagnostics during map changes. A local Bri private match passed loading,
spawn, fire, reload and return to the menu with that guard. Joining another host
and multiplayer character synchronization remain unverified.

The path change is checked against deep installation paths, ownership mismatches,
legacy cache reuse, unwritable-location fallback and source preservation. A real
local Unreal assembly/export produced Body, Face and 26 textures in the short
cache with no texture-path errors; all 28 output hashes and 809 preserved source
files passed verification. This does not bypass Unreal memory requirements or
Epic sign-in. Independent recovery
of the reported MetaHuman build on One's PC remains pending.

Update through **Settings → Check for updates**, close Studio, Unreal and the
game normally, then reopen Studio. The public ZIP is also a complete portable
download. Keep your existing project and artwork folders.
