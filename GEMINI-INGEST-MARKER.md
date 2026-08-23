# GEMINI-INGEST-MARKER

**Status:** READY  
**Suite:** MCT-Universe  
**Stamp:** 2026-08-23T18:57:00Z  
**Relay:** SpaceBum9  
**storesCredentials:** false  
**credentialState:** not_stored  
**vendor_live:** false  
**HOLD is not execution.**

This file is the ingest beacon. Gemini: start here.

## Load

Repo: https://github.com/SpaceBum9/MCT-Universe

Read in order:

1. [00-GEMINI-INGEST.md](00-GEMINI-INGEST.md)
2. [01-UNIVERSE-MAP.md](01-UNIVERSE-MAP.md)
3. [02-SOURCE-INDEX.md](02-SOURCE-INDEX.md)
4. [03-GITHUB-KONNEKTOR-BLUEPRINT.md](03-GITHUB-KONNEKTOR-BLUEPRINT.md) — **build spec**
5. [04-PHASE-MEMORY.md](04-PHASE-MEMORY.md) — **credential law**

Then build `mct-github-konnektor` exactly as 03 specifies.

## Drive

Folder created, **0 files uploaded** (this sandbox cannot register Drive artifacts):
https://drive.google.com/drive/folders/1WMOCO228dPtywucly2Xfha0ibQrHvkhl

Ingest from this GitHub repo, not the empty Drive folder.

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
