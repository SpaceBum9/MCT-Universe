# GEMINI-INGEST-MARKER

**Status:** READY  
**Suite:** MCT-Universe  
**Stamp:** 2026-08-23T19:23:00Z  
**Relay:** SpaceBum9  
**Default mode:** `MCT-RC-BILO-ATM-FRAMEWORK-SOS`  
**storesCredentials:** false  
**credentialState:** not_stored  
**vendor_live:** false  
**HOLD is not execution.**

This file is the ingest beacon. Gemini: start here.

Every multimodal prompt loads [05-DEFAULT-MODE.md](05-DEFAULT-MODE.md) as the entry stack. Do not fragment-route first.

## Load (text)

Repo: https://github.com/SpaceBum9/MCT-Universe

Read in order:

1. [00-GEMINI-INGEST.md](00-GEMINI-INGEST.md)
2. [01-UNIVERSE-MAP.md](01-UNIVERSE-MAP.md)
3. [02-SOURCE-INDEX.md](02-SOURCE-INDEX.md)
4. [03-GITHUB-KONNEKTOR-BLUEPRINT.md](03-GITHUB-KONNEKTOR-BLUEPRINT.md) — **build spec**
5. [04-PHASE-MEMORY.md](04-PHASE-MEMORY.md) — **credential law**
6. [05-DEFAULT-MODE.md](05-DEFAULT-MODE.md) — **trigger law**

Then build `mct-github-konnektor` exactly as 03 specifies.

## Load (Drive)

Folder: https://drive.google.com/drive/folders/1WMOCO228dPtywucly2Xfha0ibQrHvkhl

Spoken beacons, same order (no secrets). Text source of truth is this repo.

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
