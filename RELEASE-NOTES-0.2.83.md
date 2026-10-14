# RoweMod Studio 0.2.83 beta

Fix plain MetaHuman Creator opening and then immediately closing. Studio launches Unreal with ExecutePythonScript to open the linked source. The plain opening helper omitted Unreal's keep-Python-script-alive flag, allowing the editor to exit when the helper finished. The helper now sets that flag before loading the source, so the editor also stays available if the source cannot be loaded.

This is a RoweMod launch regression after pausing Skin Details. Skin Details remains paused; no extension or C++ build is restored. Source assets, character maps, clothing, game files and project settings are unchanged by this repair.

Native Unreal 5.8.3 startup testing reproduced the old helper's exit and verified the repaired helper remained alive for five seconds and many subsequent ticks. These isolated tests intentionally use a missing asset to test editor lifetime; they do not verify a real MetaHuman visual on another PC. The supplied friend log was truncated before shutdown, so his exact final exit reason still needs the full log if symptoms persist.

Update through Settings → Check for updates, wait for the download, then close Studio, Unreal and the game before reopening. Stock portrait/updater compatibility from 0.2.82 is retained. If updating fails, extract the full latest ZIP and preserve the old workspace and artwork.

[Download](https://github.com/xrowex/RoweMod-HoodWarfare2-Clothing/releases/download/studio-v0.2.83/RoweMod-Studio-0.2.83-Windows.zip) · [Guide](README.md)
