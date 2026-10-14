# RoweMod Studio 0.2.82 beta

Fix a Studio updater/package mismatch. The 0.2.77–0.2.81 ZIPs placed stock character-preview images in assets/characters, outside the updater's accepted program paths. An older Studio therefore rejected the downloaded archive and kept running its old Skin Details workflow.

The same three stock portraits now ship beneath assets/brand/characters, which older updaters already accept. The current updater also recognizes exactly those three legacy paths so existing 0.2.77–0.2.81 inventories can be read and migrated safely. General user assets remain outside updater ownership. Unsupported future program paths now identify the file in the error message.

Skin Details remains paused: plain MetaHuman setup requires no extension or C++ build. Saved wardrobe items, character portraits, user artwork, settings and game files stay preserved. Native runtime and authoring helpers are unchanged.

If a newer copy cannot read its own old inventory, close Studio and manually extract the complete current ZIP into a new folder once. Keep the previous folder and its projects/Studio/exports/downloads intact. Open RoweMod Studio.cmd from the new extracted folder. Do not merge or delete saved work while troubleshooting. Users whose older updater accepts its current inventory can check for updates normally.

Package acceptance is tested with actual older and current application assemblies and an isolated file transaction. This does not establish friend-PC acceptance, a newly opened editor session or gameplay.

[Download](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.82/RoweMod-Studio-0.2.82-Windows.zip) · [Guide](README.md)
