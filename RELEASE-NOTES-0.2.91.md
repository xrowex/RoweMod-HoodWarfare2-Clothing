# Studio 0.2.91 — Submit gear from Studio and recover completed exports

Open **My clothes → garment → Submit to gallery** (or **Submit this version** for
a saved wardrobe item). Sign in with Google in your browser, match the connection
code and connect Studio. Rowe approves posting access separately. The Google
account's stable identity identifies the creator; matching an administrator's
email does not grant admin access.

Enter a name, version and description. Confirmation 1 prepares a local copy of
the garment and its preview without uploading. Review the actual preview and
size. Confirmation 2 confirms sharing permission and sends the selected garment,
textures, fit compatibility data and preview to Rowe. No file picker is needed.
The button turns green only after a durable server receipt; retries of the same
submission do not create duplicate posts. Submissions stay private until review.
This is a creator-source submission. A Subscribe download still needs a prepared,
verified playable package. A shared rig does not guarantee body fit.

Studio keeps its scoped publishing session encrypted for the current Windows
user, for up to 30 days. Google credentials are verified on the server and are
not stored by Studio. Sign out revokes the connection. Google sign-in uses only
basic identity, not Gmail or Drive. See https://rowemods.com/gear/privacy.

One's 0.2.89 report showed a completed MetaHuman export followed by an Unreal
access-violation exit during shutdown. Studio can now continue only when the
current export and wrapper receipts both completed, the source matches, and
every declared mesh/texture still matches its hash. Missing, altered or failed
exports remain blocked. The native shutdown diagnostic is preserved. This
recovers the build handoff; it does not claim the underlying Unreal shutdown
fault or One's full game workflow has been independently fixed.

Validation: 11 native recovery/UI checks; 28 website/JWT/storage checks; 23 local
review/publish checks; 17 scoped-session, PKCE, revocation and native-upload checks;
real Blender garment export and preview preparation in an isolated project copy,
with the source project preserved and no upload. Real Google-account sign-in,
One's PC, and new gameplay acceptance still require user testing. Existing
ImageSharp dependency advisory warnings remain documented in 0.2.90 notes.
