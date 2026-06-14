# OPERATING RULES — OURGANI BRAND SYSTEM

## Purpose

This document defines mandatory operational rules for all brand repositories within the Ourgani ecosystem.

These rules ensure consistency, scalability, and system-level interoperability.

---

## 1. FILE STRUCTURE RULE

Every brand repository MUST follow this structure:

/main-site
/system
/registry
/deploy
/assets
/docs

### Rule:
- `main-site/` is the ONLY publicly deployed folder
- All other folders are internal system logic

---

## 2. DEPLOYMENT RULE

All brands deploy via Cloudflare Pages:

### Required Settings:
- Build command: NONE
- Output directory: `main-site`
- Framework: None

### Rule:
Only `main-site/` is published to production.

---

## 3. SYSTEM ISOLATION RULE

System logic must never mix with presentation logic.

- `/system` → logic, rules, definitions
- `/main-site` → user-facing interface

Violation of this rule breaks system consistency.

---

## 4. REGISTRY RULE

Each brand MUST maintain a registry file:

/registry/brand.json

This file contains:
- Brand name
- Pillar classification
- Role definition
- System linkage metadata

### Rule:
If it is not in the registry, it does not exist in system logic.

---

## 5. CONSISTENCY RULE

All brands must:
- Follow identical structural layout
- Use consistent naming conventions
- Maintain identical deployment architecture

This ensures system-wide interoperability.

---

## 6. INHERITANCE RULE

Brands inherit:
- Architecture from Ourgani System
- Logical structure from ProtoSynthesis (external system layer)
- Registry alignment rules from ecosystem standards

Brands do NOT redefine these systems.

---

## 7. MODIFICATION RULE

Allowed modifications:
- UI/UX inside main-site
- Brand-specific services and content
- Internal business logic

Not allowed:
- Changing system structure
- Renaming core folders
- Breaking deployment model
- Overriding registry format

---

## 8. SCALABILITY RULE

Every brand must be able to scale without structural change.

If scaling requires:
- new folders outside standard structure
- new deployment model
- new system rules

Then the change belongs in the Ourgani System layer, not the brand layer.

---

## END OF RULES
