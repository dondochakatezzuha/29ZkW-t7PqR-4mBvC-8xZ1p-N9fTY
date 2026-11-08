# How ChatGPT should use the TGC Knowledge Library

This repository holds an **opt-in, public, partial mirror** of approved Discord-game exports. It is not the complete bot archive, not a private store, and not an automatically verified canon database.

**Site:** https://dondochakatezzuha.github.io/29ZkW-t7PqR-4mBvC-8xZ1p-N9fTY/

**Fresh JSON catalog:** https://raw.githubusercontent.com/dondochakatezzuha/29ZkW-t7PqR-4mBvC-8xZ1p-N9fTY/main/docs/bridge/catalog.json

## Source-reading workflow

1. Open `docs/bridge/catalog.json` **fresh each time** a user asks about TGC.
2. Check `included_files`, `eligible_files`, `index_truncated`, and skip counts. If `included_files=0`, the bot data has **not yet synced**.
3. Filter `files` by `category`, `group`, `title`, and `original_path` to identify relevant sources. Open individual `docs/bridge/source/*.txt` files referenced by `file_url` (relative to `docs/bridge/`).
4. Explain uncertain or conflicting claims with source links. Discord roleplay text can be outdated, fictional, contradicted by newer canon, or user-proposed rather than GM-confirmed.
5. Never treat an absent entry as proof a character, event or power is not in the private master archive.
6. Keep TGC separate from TWN unless a cross-over is explicitly documented.
7. When asked to reorganize information, generate clearly labeled summaries, time-ordered changes, and conflicting-source notes. **Do not replace primary source files or claim to have reviewed unshared data.**

## How updates arrive

Discord bot on the owner's PC → original local exports → TGC Live Bridge (v4 or expanded v5) → approved public-safe subset uploaded to GitHub approximately every 15 minutes **while the bridge runs** → GitHub Pages build/deployment.

The site does not run the bot. Files are not ingested by ChatGPT automatically. A new chat can **open the link on demand**, subject to the chat/browser's web access, and use the published source files. Continuous ChatGPT research/organizing would require a separate user-configured automation.

The bridge keeps Discord bot tokens and GitHub access tokens off the public site. The owner must review any public exports before first publishing. Public repository names are not passwords.

**Snapshot capacity:** v4 publishes up to 160 text files / 7 MiB, 384 KiB each. The upgraded v5 can publish up to 1,200 approved text files / 64 MiB, 1 MiB each, but **only after the user runs it on their PC and explicitly re-approves the larger public exposure**. Check `included_files` in the LIVE JSON catalog for the actual published count; the upgrade alone does not upload new data. It remains a partial snapshot rather than the full 14 GB archive. Private/admin channels, oversized files, media and other content remain excluded. GitHub commits can preserve published contents.
