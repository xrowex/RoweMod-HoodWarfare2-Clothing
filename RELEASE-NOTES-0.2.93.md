# Studio 0.2.93 — Repair native gear uploads

Studio now quotes multipart field names and filenames when sending gear. The
production server's form parser rejects HttpClient's unquoted field names before
the upload route runs, producing the generic unexpected-reply error. The website
also retains the corrected 32 MiB upload limit.

The failure was reproduced using the exact native serializer and a 7,263,151-byte
garment. The corrected native bytes passed the built production Worker, alongside
the existing browser upload, retry protection and private pending-file checks.
Real live submission acceptance is recorded separately after user confirmation.

Includes 0.2.92's green Google connection status, clearer HTTP upload errors and
compatibility repair for older sealed wardrobe versions. Original projects,
prepared drafts and artwork stay saved. No new gameplay or friend-PC acceptance
is claimed. Existing ImageSharp dependency advisories remain documented in 0.2.90.
