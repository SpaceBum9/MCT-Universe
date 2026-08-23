# GEMINI-INGEST-MARKER

**Status:** READY  
**Suite:** MCT-Universe  
**Stamp:** 2026-08-23T19:12:00Z  
**Relay:** SpaceBum9  
**storesCredentials:** false  
**credentialState:** not_stored  
**vendor_live:** false  
**HOLD is not execution.**

This file is the ingest beacon. Gemini: start here.

## Load (text)

Repo: https://github.com/SpaceBum9/MCT-Universe

Read in order:

1. [00-GEMINI-INGEST.md](00-GEMINI-INGEST.md)
2. [01-UNIVERSE-MAP.md](01-UNIVERSE-MAP.md)
3. [02-SOURCE-INDEX.md](02-SOURCE-INDEX.md)
4. [03-GITHUB-KONNEKTOR-BLUEPRINT.md](03-GITHUB-KONNEKTOR-BLUEPRINT.md) — **build spec**
5. [04-PHASE-MEMORY.md](04-PHASE-MEMORY.md) — **credential law**

Then build `mct-github-konnektor` exactly as 03 specifies.

## Load (Drive)

Folder: https://drive.google.com/drive/folders/1WMOCO228dPtywucly2Xfha0ibQrHvkhl

Spoken beacons, same order (no secrets):

- GEMINI-INGEST-MARKER.mp3
- 00-GEMINI-INGEST.mp3
- 01-UNIVERSE-MAP.mp3
- 02-SOURCE-INDEX.mp3
- 03-GITHUB-KONNEKTOR-BLUEPRINT.mp3
- 04-PHASE-MEMORY.mp3

Text source of truth is this repo. Drive holds the audio beacons so Gemini Gems/Drive ingest has a file to attach.

## Credentials

Handed as a 15-minute phase handle in RAM. Never write tokens to Drive, Git, traces, env, or chat. Gemini sees only `registerId`.

```
CREDENTIAL_PHASE
  registerId: string
  validUntil: ISO-8601
  capability: github.konnektor
  storesCredentials: false
  secret: <RAM only>
```
