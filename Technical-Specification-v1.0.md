# Technical Specification v1.0

## 1. Overview

This document defines the technical rules and intended mechanics of the project.

The purpose of this specification is to provide a clear, publicly verifiable reference for how the project's transaction and distribution rules are intended to operate.

This specification may be updated through future documented versions.

---

## 2. Core Rules

### 2.1 5× Rule

The 5× rule is designed to limit excessive accumulation or repeated use of the same allocation.

A wallet or eligible participant must comply with the defined 5× limitation before additional activity is permitted.

The implementation should apply the rule consistently and transparently.

---

### 2.2 25% Hourly Rule

A maximum of 25% of the applicable allocation or permitted amount may be processed within a given one-hour period.

This restriction is intended to distribute activity over time rather than allowing the entire permitted amount to be processed immediately.

The applicable amount and calculation method should be determined by the smart-contract implementation.

---

## 3. Transfers

Transfers between wallets are subject to the project's applicable rules.

The system should distinguish between:

- Standard wallet-to-wallet transfers
- Buys
- Sells
- Contract interactions
- Other transactions defined by the implementation

Where applicable, transfer activity must not be used to bypass the project's restrictions.

---

## 4. Multiple Buys

Multiple purchases by the same participant or related wallets are subject to the applicable allocation and transaction limits.

The system is intended to prevent repeated purchases from being used to circumvent the 5× rule or the 25% hourly restriction.

Any implementation-specific treatment of multiple purchases must be documented in the corresponding smart-contract documentation.

---

## 5. Anti-Bypass Mechanism

The project's rules are intended to prevent circumvention through:

- Repeated transactions
- Splitting transactions into smaller amounts
- Using multiple wallets
- Transferring allocations between wallets
- Other transaction patterns designed to avoid applicable limits

The exact enforcement mechanism depends on the final smart-contract implementation.

---

## 6. Transparency

All material changes to the project's rules should be documented publicly.

Changes should use a new specification version where appropriate.

Example:

- `Technical-Specification-v1.0.md`
- `Technical-Specification-v1.1.md`
- `Technical-Specification-v2.0.md`

Previous versions should remain available when practical to preserve an auditable history.

---

## 7. Smart Contract Implementation

The final smart contract is the authoritative source for on-chain enforcement of these rules.

This document describes the intended technical behavior and should be read together with the deployed contract and its verified source code.

If there is a discrepancy between this document and the deployed smart contract, the actual on-chain implementation should be independently verified and the documentation updated accordingly.

---

## 8. Version

**Specification Version:** 1.0  
**Status:** Initial Public Specification  
**Repository:** Public  
**Document Type:** Technical Specification
