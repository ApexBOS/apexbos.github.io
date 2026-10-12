# ApexBOS — download site and app update manifest

ApexBOS (Business Operating System · လုပ်ငန်းလည်ပတ်မှုစနစ်) — this repository is served by GitHub
Pages at **https://apexbos.github.io** (branch `main`, root).

- `index.html` — the download page (Myanmar by default, English toggle; no tracking, no external scripts).
- `update-manifest.json` — read by release builds of the app (Settings → App updates → Check).
  Format: `{ version, minSupportedVersion?, publishedAt, notes: { my, en }, platforms: { android: { url, sha256 } } }`;
  Android `url` must be the signed `ApexBOS-<version>-release.apk`.
- APKs are attached to the GitHub Release `v<version>` of this repository.

Latest: **0.2.23** (versionCode 223) — `ApexBOS-0.2.23-release.apk`, SHA-256 `b45b0057ad440f41136661ddbfe026b28a699439b88b7d6fbf2a31d6bc021dfc`.
Signing certificate SHA-256: `A8:4E:29:13:C5:FD:52:1D:7E:A0:34:25:03:EB:AD:98:38:DE:88:70:2C:EF:7B:DB:40:B5:F2:1E:47:D4:60:5D`.

Before updating: make a Backup, and update every device of a business together.
