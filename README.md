# assets — static public asset host (maximise ecosystem)

> ⚠️ **PUBLIC repo.** Everything here is world-readable via `raw.githubusercontent.com`. **Never commit secrets, credentials, tokens, or private/identity-bearing material.** Only generic, shareable static assets.

**Purpose:** permanent, auth-free `https` raw-URL host for static assets that pipelines need to fetch directly (e.g. kie.ai `imageUrls` reference images). Replaces ephemeral upload URLs.

**Raw-URL pattern:**
```
https://raw.githubusercontent.com/maximiser13/assets/main/<stream>/<file>
```

**Convention:** one folder per stream/channel. Keep files small + stable; treat each path as a permanent contract (pipelines hard-code these URLs).

| Folder | Stream | Contents |
|--------|--------|----------|
| `taro/` | P3-YouTube (WM-Shorts) | TARO reference images for kie.ai REFERENCE_2_VIDEO identity-lock |

**Upgrade path** (if traffic scales): dedicated public GCS bucket in the personal-account project `pannaheater-pipeline` (no org Public-Access-Prevention policy). Research parked; not needed now.
