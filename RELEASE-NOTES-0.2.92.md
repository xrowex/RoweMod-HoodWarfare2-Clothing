# Studio 0.2.92 — Clear publishing status and saved clothing compatibility

Studio now shows **Google connected ✓** after connecting your publishing
account. Posting approval remains a separate check. The submission preview and
size stay visible after preparation instead of being replaced by a late progress
message. Upload errors include the HTTP status; an oversized upload explains that
the prepared files remain saved and nothing was confirmed sent.

The website's multipart upload limit now matches the gear route's 32 MiB limit.
Previously a framework preflight rejected packages above 1 MiB before the gear
route could process them. A real 7,263,151-byte garment package passed the built
production Worker test, including an idempotent retry and private pending download.

Older sealed wardrobe versions reopen when their original metadata predates an
optional fabric provenance field. This compatibility path applies only to the
empty, previously absent field; populated provenance and all existing payload
hashes remain verified. A damaged saved version reports its own error without
hiding the rest of My clothes. Original versions, seals and artwork are preserved.

Validation: 19 existing saved wardrobe versions reopened; six isolated compatibility
and integrity checks preserved all 17 original files; 11 publishing/recovery UI
checks, 44 image import checks, 191 Studio checks and 67 updater checks passed.
Real Google sign-in and approved native Studio connection were verified with the
user. The final live submission is verified separately in the publication receipt.
No new friend-PC or gameplay acceptance is claimed. Existing ImageSharp dependency
advisory warnings remain documented in the 0.2.90 notes.
