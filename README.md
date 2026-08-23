# MCT-Universe

Gemini ingest pack for the SpaceBum9 constellation. **No credentials stored.** Phase memory only.

## For Gemini

Read in order:

1. [00-GEMINI-INGEST.md](00-GEMINI-INGEST.md)
2. [01-UNIVERSE-MAP.md](01-UNIVERSE-MAP.md)
3. [02-SOURCE-INDEX.md](02-SOURCE-INDEX.md)
4. [03-GITHUB-KONNEKTOR-BLUEPRINT.md](03-GITHUB-KONNEKTOR-BLUEPRINT.md) — build spec
5. [04-PHASE-MEMORY.md](04-PHASE-MEMORY.md) — credential law

Then build `mct-github-konnektor` as specified in 03.

Prompt: [GEMINI-PROMPT.txt](GEMINI-PROMPT.txt)

## Law

`storesCredentials: false` · `credentialState: "not_stored"` · HOLD is not execution · `vendor_live=false`

Tokens are handed as a 15-minute phase handle in RAM. They never appear in this repo, Drive, traces, or env files.

## Drive

Folder (created, same pack): https://drive.google.com/drive/folders/1WMOCO228dPtywucly2Xfha0ibQrHvkhl
