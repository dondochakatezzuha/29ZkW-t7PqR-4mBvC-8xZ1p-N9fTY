# How ChatGPT should use the TGC Knowledge Library

This repository holds an **opt-in, public, partial mirror** of approved Discord-game exports. It is not the complete bot archive, not a private store, and not an automatically verified canon database.

**Site:** https://dondochakatezzuha.github.io/29ZkW-t7PqR-4mBvC-8xZ1p-N9fTY/

**Fresh JSON catalog:** https://raw.githubusercontent.com/dondochakatezzuha/29ZkW-t7PqR-4mBvC-8xZ1p-N9fTY/main/docs/bridge/catalog.json

## Source-reading workflow

1. Open `docs/bridge/catalog.json` **fresh each time** a user asks about TGC.
2. Check `included_files`, `eligible_files`, `index_truncated`, and skip counts. If `included_files=0`, the bot data has **not yet synced**. If `catalog_parts` is present, **fetch every listed `docs/bridge/catalog-####.json` file** to get the complete published source list (the root `files` array will be empty in sharded mode).
3. Filter all catalog rows (root `files` or every `catalog_parts` shard) by `category`, `group`, `title`, and `original_path` to identify relevant sources. Open individual `docs/bridge/source/*.txt` files referenced by `file_url` (relative to `docs/bridge/`). If a large file was split into numbered parts, read all relevant parts in order; each part retains the original file path.
4. Explain uncertain or conflicting claims with source links. Discord roleplay text can be outdated, fictional, contradicted by newer canon, or user-proposed rather than GM-confirmed.
5. Never treat an absent entry as proof a character, event or power is not in the private master archive.
6. Keep TGC separate from TWN unless a cross-over is explicitly documented.
7. When asked to reorganize information, generate clearly labeled summaries, time-ordered changes, and conflicting-source notes. **Do not replace primary source files or claim to have reviewed unshared data.**

## How updates arrive

Discord bot on the owner's PC → original local exports → TGC Live Bridge (v4/v5 snapshot or v6 expanded readable-text mirror) → approved public-safe subset uploaded to GitHub approximately every 15 minutes **while the bridge runs** → GitHub Pages build/deployment.

The site does not run the bot. Files are not ingested by ChatGPT automatically. A new chat can **open the link on demand**, subject to the chat/browser's web access, and use the published source files. Continuous ChatGPT research/organizing would require a separate user-configured automation.

The bridge keeps Discord bot tokens and GitHub access tokens off the public site. The owner must review any public exports before first publishing. Public repository names are not passwords.

**Mirror versions:** v4 capped at 160 sources; v5 at 1,200 / 64 MiB. **v6** removes arbitrary small file-count limits for readable text, splits large logs into numbered text parts, and can publish approved roleplay text (including *opt-in* private RP channels) up to a protective 650 MiB text budget. Administrator/moderation/credential paths are still excluded, and binary media remains local. No Google Drive is involved. v6 must be run by the user on their PC and explicitly reapproved before any expanded upload happens. Check the LIVE catalog counters instead of assuming v6 is installed or fully synced. GitHub Pages has a 1 GB published-site limit; the 14 GB local archive cannot all fit there. GitHub history may retain published text.
