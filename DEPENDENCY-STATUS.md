# Dependency status — Studio 0.2.64 beta

The CUE4Parse conversion package pins ImageSharp 3.1.12. Restore currently reports five advisories for that transitive dependency:

- [ICC profile parsing](https://github.com/advisories/GHSA-gwg2-r3hj-4w44)
- [TIFF/histogram advisory](https://github.com/advisories/GHSA-j3p4-wp97-rph4)
- [TIFF/histogram advisory](https://github.com/advisories/GHSA-j9gm-c75j-xc9q)
- [TIFF/histogram advisory](https://github.com/advisories/GHSA-jjfr-hcj7-qf5w)
- [BigTIFF parsing](https://github.com/advisories/GHSA-wmxv-xphr-5c9g)

This beta does not claim the dependency is patched. Its MetaHuman skin-map comparisons now accept only bounded, static PNGs. The decoder receives only PNG pixel-bearing chunks; ICC, EXIF, color and text metadata are excluded without altering the saved source. TIFF routing is refused. Twenty-six isolated PNG fixtures and thirty-four bridge/reset fixtures pass against the final candidate, including transparent RGB/alpha, metadata exclusion and malformed/oversized input rejection.

Studio does not directly call ImageSharp's TIFF encoder, histogram equalization or ICC entry parsing. Clothing texture import uses its existing PNG validation and System.Drawing; CUE's PNG export uses SkiaSharp. These observed call paths narrow exposure but are not a blanket security signoff for the dependency or arbitrary input.

A supported upgrade remains a wider-release task. The CUE package's exact version constraint needs compatibility work, and newer ImageSharp versions enforce their own licensing requirements. Use the publisher's [licensing and pricing](https://sixlabors.com/pricing/) and [versioned license](https://github.com/SixLabors/ImageSharp/blob/v4.1.2/LICENSE); qualifying users may apply for Community licensing. No license validation or build target has been disabled.

The independent fresh-PC gameplay and optional MetaHuman extension-build gates also remain open. See FRIEND-TEST.md for the beta test route.
