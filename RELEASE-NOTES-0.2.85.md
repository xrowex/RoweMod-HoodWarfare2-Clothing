# RoweMod Studio 0.2.85 beta

Press **Send to Rowe** in Studio's bottom bar to send diagnostic text directly to the private RoweMods support inbox. No ZIP creation, file selection or attachment is required. The button turns green and says **Sent to Rowe** only after the server confirms durable receipt. Connection failures offer Retry; an unchanged retry uses the same report ID to avoid duplicate submissions.

Task failures and managed startup/process failures save a local diagnostic snapshot. Failed MetaHuman exports also preserve a bounded native Unreal log tail for the report. Reports include Studio/OS versions and diagnostic text, redact common credential fields, URL query strings, email addresses and personal profile/workspace paths, and exclude model, texture, artwork, settings and project files. Logs can still contain project names. Reports are sent only when the user presses the button. The inbox has admin-only reads, rate/size limits and 30-day retention; it is not a public GitHub issue or Discord upload. Local diagnostic files remain available when offline. Native crashes, power loss and failures before startup cannot always produce a report.

MetaHuman texture-download errors now explain that missing texture sources do not prove a sign-in failure. In Creator, use the Authentication/person icon beside Refresh Preview to inspect the current account. Click **Download Texture Sources**, wait for completion, save the character, then retry **Build & launch game**. Being signed into Epic Launcher alone does not verify the Creator cloud request. Failed downloads may require checking Epic service/network errors.

Automatic character preparation from 0.2.84 remains. Skin Details stays paused. This release does not add complete Creator-outfit transfer or establish new friend-PC, full-match or multiplayer acceptance.

Update using **Settings → Check for updates**, then close Studio, Unreal and the game to apply it. Older releases with the inventory rejection need one full-ZIP manual update, preserving the old workspace and artwork.
