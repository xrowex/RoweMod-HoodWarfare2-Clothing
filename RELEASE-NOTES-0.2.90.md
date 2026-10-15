# Studio 0.2.90 — Clear errors, image imports and creator publishing

Texture import accepts PNG, JPEG, TGA, TIFF, BMP and WebP. Use **Import image** on
an artwork card or **Import texture set** for several maps. Studio validates the
entire selection, keeps external originals, and stores project-owned PNGs. A bad
map leaves the saved selection unchanged. Missing texture slots can be repaired
with any supported image. PNGs remain byte-identical; conversion does not resize
images or guess packed channels. Use lossless maps and DirectX orientation for
normals; converting JPEG cannot restore detail already lost to compression.

Errors explain common memory, Epic texture sign-in, long path, unsupported fabric,
clothing-mask conflict, package, download and access failures. Full exceptions
remain in Task details and private diagnostic reports. Guided failures now offer
**Send to Rowe** directly, including after the saved project reloads.

**Downloads → Share gear / Creator access** opens the website. Creators sign in
with the site's existing account system and request access. Rowe approves the
stable account identity under **Admin → Creators & gear publishing**. Optional
Discord handles are self-reported contact details, not verified Discord links.
Approved creators upload a `.roweclothes` package, preview and fit information;
an optional matching `.roweplay` export enables Subscribe after review. Uploads
remain private until Rowe publishes them. The combined upload limit is 32 MiB;
previews are PNG/JPEG up to 4 MiB and 4096 pixels per side.

Taking down an item removes its public listing and downloads. Revoking a creator
also hides their published gear and blocks new uploads. Installed user copies,
artwork and local projects are preserved. ROWE Pants has been withdrawn from
public discovery; existing release archives remain available for recovery.

Validation covers real image conversion/preservation and catalog URL boundaries,
plus local D1/R2 application, approval, upload, review, publication, download,
revocation and take-down. Synthetic local identities are used only on loopback;
these checks do not claim independent creator-PC or gameplay acceptance.

The existing CUE4Parse dependency pins ImageSharp 3.1.12 and still emits its prior
NuGet advisory warnings. An attempted newer dependency requires a separate vendor
license and was not adopted. Import sizes and decoded dimensions are bounded.
