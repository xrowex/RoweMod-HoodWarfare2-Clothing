# Rowe Studio 0.2.120 beta

## Faster, cleaner Studio

Studio now uses compact rows, smaller previews, charcoal panels and orange navigation throughout the character library, Downloads, My mods, Profiles, Wardrobe and creator tools. The existing Rowe Studio logo, icon and character-specific clothing workflow are retained.

- Large libraries create controls for visible rows and reuse unchanged previews and character pages. Returning to a library preserves its chosen row and scroll position.
- Refreshing a virtual list no longer jumps to unrelated rows. Replacing a changed row restores keyboard focus and selection.
- Profile inventory, profile import review, wardrobe discovery, saved stock edits and creator-file wearer selection run as cancellable background reads. Navigation stays available while they load, and late results cannot replace the page you opened next.
- Failed or cancelled profile reads offer a clear retry. An imported profile retries that same review. Applying profiles, builds, installs and interrupted-install recovery remain protected, exclusive operations.
- Preview decoding uses bounded caching and safe image disposal. Progress messages arrive in bounded batches; hidden windows avoid unnecessary control updates. Short wardrobe lists shrink to their content.

## Local validation

In the same generated 300-character fixture, initial library readiness measured 36.7 seconds in the preserved 0.2.116 baseline and 0.75 seconds in this candidate; Create-and-back navigation measured 41.7 seconds and 0.86 seconds. Initial controls fell from 2,148 to 75. These are single-PC, offscreen WinForms measurements, not a general performance or game-FPS guarantee.

The exact candidate passed 60 style layouts, six scale layouts, 18 mod-manager layouts, four profile layouts, keyboard/focus and row-lifetime checks, delayed/cancelled/failed profile reads, progress batching, thumbnail-cache checks, 81 profile/recovery checks, 81 clothing isolation checks, 13 deletion checks and retained texture/painting workflow checks. Generated artwork, meshes, rigs and 300 saved project definitions were preserved by the fixtures. The complete release ZIP and the upgrade from the previously published Studio are checked before promoting the update feed.

The 0.2.117 clothing material isolation repair remains included. Existing characters, artwork, downloads and settings are preserved. This update retains C#/WinForms and character-specific fitting; it adds no universal fitting, short-character scaling or game/anti-cheat changes.

## After updating

Let Studio finish updating and reopen. Browse your saved characters and mods, try scrolling and resizing, and use Tab, arrows, Home/End and PageUp/PageDown. Existing customized clothing can be rebuilt with its saved Base texture enabled. Send to Rowe from a failed operation if a problem remains.

Physical mixed-monitor DPI, loaded native-preview/GPU behavior, recipient clothing retry and two-PC multiplayer acceptance remain separate user checks. Controller support and remote performance telemetry were assessed but are not added in this release. The portable ZIP excludes user projects, game/MetaHuman assets, private reports, XERJ and the local tattoo plugin. Existing dependency advisory status is documented in DEPENDENCY-STATUS.md.
