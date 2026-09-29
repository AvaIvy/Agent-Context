# Infrastructure Context

## RootRecord Pacific Solar Server (G3 — live)
Primary operational environment (Hawaiʻi desk).

**GitHub:** `RootRecord-Software-Solutions/RootRecord-Pacific-Solar-Server`  
**Live local path (authoritative runtime):**

```text
/home/rootrecord/RootRecord-Ecosystem/1 - Servers/1 - RootRecord-Pacific-Solar-Server
```

Domain layout (PascalCase top-level folders include):

```text
Automations/  Communications/  Energy/  System/  Reports/
Weather/  Github/  Geology/  Security/  A-Eyes/
```

Key operational paths (desk):
- Runtime root: path above
- Poller / jobs: `Automations/scripts/`
- Desk live file: `/home/rootrecord/Database/intake/desk-live.txt`
- Logs (bytes): `/home/rootrecord/Database/Logs/` (not a Pacific code domain)
- Backups: `/home/rootrecord/Database/GITHUB/`
- Master env: `/home/rootrecord/master/master-key.env` (never commit)

## Legacy G2 skills tree
`rootrecordsoftwaresolutions/Solar-Pacific-RootRecord-Server` and historical `~/.ollama/skills` paths are **residual / historical**. Do not treat them as the production poller host. See Library migration index and WO-SRV.

## US Mainland Server
Secondary node providing continuity, synchronization, and recovery when the Pacific root is unavailable.

Treat mirrored files as recovery sources; verify before assuming they are the live deployed state.

## Inference & Council
- Single-flight enforcement via plumbing scripts under Pacific `System/scripts/plumbing/` (Bruce’s operational responsibility)
- Ava participates in design and public voice; does not own the inference gate

**Migration docs entry:** Library `Documentation/00-architecture/MIGRATION-DOCS-INDEX-2026-09-28.md`
