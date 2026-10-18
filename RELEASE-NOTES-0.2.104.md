# RoweMod Studio 0.2.104 beta — assembled groom identity

Fixes hair preparation when Unreal assembles a selected hairstyle as `GroomAsset_0` and retains the hairstyle name on its native binding. Studio now reads the slot from both the binding and groom, refuses conflicting slots, and uses the existing registered source-component lookup only when both names are generic. This avoids opening a source-inspection actor for the affected sample hairstyle.

The repair passed 16 focused lifecycle and slot checks. A real Unreal export of the previously failing saved character completed with Hair, Eyebrows and Eyelashes. The next local Cameron attempt also completed native hair export and continued into game-asset cooking. Complete local build/game launch and One's updated retry are still being verified; these results do not establish match or multiplayer acceptance.

Save your MetaHuman, then use Build & launch. Studio requests normal editor closure and continues after it closes; respond to any unsaved-work or Epic sign-in prompt. Settings → Check for updates installs this repair through the normal updater. Saved characters and artwork are preserved. Outfits remain fitted to one character; universal clothing is retired.
