# External

Version manifest and offset snapshots consumed by the client at startup.

## Contents

| Path | Purpose |
|---|---|
| `manifest.json` | Current app/offset versions, immutable release URLs and `sha256` hashes |
| `core/offsets/offsets.seed.json` | Offset snapshot for the current Roblox build |

## Release assets

Payloads referenced by `manifest.json` are published as **immutable release assets**, never as
files on a branch. Always verify `sha256` before use.

`main` is the branch the client reads at startup. Do not rewrite it.
