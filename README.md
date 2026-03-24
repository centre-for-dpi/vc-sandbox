# VC Sandbox — CDPI Digital Credentials

An interactive browser-based sandbox that demonstrates how governments and service providers can **issue, store, and verify** digital credentials using open-source Digital Public Goods (DPGs).

No backend required — runs entirely in the browser as a single HTML file.

## What It Does

The sandbox walks through the full lifecycle of Verifiable Credentials (VCs) for Digital Public Infrastructure:

**Issue a Credential** — Pick from 20+ credential types (National ID, Birth Certificate, Education, Health Card, Farmer Registration, etc.), fill in fields, and generate a W3C-compliant VC signed with a DID.

**Bulk Upload** — Upload an Excel or CSV file of citizen data and batch-generate VCs for every row. Download results with VC IDs and QR payloads.

**Mobile Wallet** — See how credentials appear in a citizen's Inji Wallet. Fan view, card list, share via QR / NFC / deep link.

**Online Verification** — Paste a VC and run a full verification: signature check, DID resolution, expiry, revocation, and schema validation.

**Offline Verification** — Sync a trust store once, then verify credentials with zero network calls using cached issuer keys and signed QR codes.

## Open Source Stack

| Component | Role |
|-----------|------|
| **CREDEBL** | Credential issuance and schema management |
| **Inji** | Citizen wallet and verifier apps |
| **Sunbird RC** | Trust registry for issuer authority |
| **MOSIP** | National ID backbone |

## Standards

- W3C VC Data Model 2.0
- OID4VCI / OID4VP
- AnonCreds (zero-knowledge proofs)
- SD-JWT VC (selective disclosure)
- ISO mDL / mdoc (18013-5)

## Running It

Open `index.html` in any modern browser. That's it — no build step, no dependencies, no server.

## License

Open source (LICENSE)[./LICENSE] . Part of the [CDPI](https://cdpi.dev) digital credentials initiative.
