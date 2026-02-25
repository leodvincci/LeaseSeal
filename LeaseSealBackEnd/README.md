# LeaseSeal 🔏
**Verified lease documents. Tamper-evident. Auditable. Dispute-resistant.**

LeaseSeal turns leases (PDFs, scans, exports) into **verifiable artifacts** with a clear **source of truth**.  
The goal is simple: reduce “who changed what?” chaos by making lease versions **provably intact** and **easy to verify**.

---

## What LeaseSeal does

- **Verify integrity** — detect changes to lease files after upload/signing
- **Version tracking** — track revisions with clear provenance
- **Audit trail** — record key events (upload, verification, updates)
- **Trust layer** — make authenticity obvious for renters, landlords, and property managers

---

## Why this exists

Leases are high-stakes documents that often live as email attachments and PDFs with no provenance.  
When disputes happen, people argue about versions. LeaseSeal is about **ending the ambiguity**.

---

## MVP scope (current focus)

- Upload a lease document
- Compute and store a **cryptographic fingerprint** (hash) for the file
- Display a **verification result** for any uploaded file (match / mismatch)
- Maintain a basic **version timeline** (v1, v2, …) with timestamps
- Log a minimal **audit trail** of events

---

## Planned features

- Document “seals” (shareable verification links / codes)
- Multi-party workflows (landlord + tenant + property manager)
- Role-based access control
- Redaction + secure sharing
- Optional e-sign integration (or “bring your own signature provider”)
- Exportable audit reports (PDF/CSV)

---

## Architecture goals

LeaseSeal is also a portfolio-quality system focused on:
- Clean boundaries (**ports & adapters / hexagonal architecture**)
- Contract-first APIs (no domain leakage)
- Test coverage that catches production-shaped bugs
- Small PRs, documented decisions, and repeatable workflows

---

## Tech stack (initial direction)

- **Backend:** Java + Spring Boot
- **Database:** PostgreSQL
- **Frontend:** React
- **Infra:** Docker (local), deployment TBD

> Stack may evolve as the product sharpens. The boundary discipline won’t.

---

## Getting started (placeholder)

This section will be updated as the repo boots up.

### Prerequisites
- Java (LTS)
- Docker + Docker Compose

### Run locally
```bash
# TODO: add commands once the first service is scaffolded