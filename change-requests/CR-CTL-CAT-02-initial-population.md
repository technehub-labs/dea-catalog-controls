# CR-CTL-CAT-02: Initial Population

| Field | Value |
|---|---|
| **CR** | CR-CTL-CAT-02 |
| **Title** | Initial population: the twenty IC-mandated controls |
| **Status** | Landed |
| **Layer** | Catalogue (L2 Risk & Compliance) |
| **Programme** | Org-wide catalog advancement (Wave 1) |
| **Repository** | `technehub-labs/dea-catalog-controls` |
| **Author** | Emmanuel A. Otchere |
| **Date** | 2026-11-02 |
| **Depends on** | CR-CTL-CAT-01 (kit); CR-IC-CAT-09 (the citations this population resolves) |
| **Trigger** | The information-classes catalogue's 8 records cite 20 canonical `dea:control-*` ids (27 citations) in `mandated_controls`, with cross-catalogue resolution explicitly deferred (`resolution_active: false`) until this catalogue populates. This is that population. |

## 1. Executive summary

Twenty canonical Control records are admitted, one per distinct `dea:control-*` id cited by the information-classes records. Each record's description quotes the citing class's requirement verbatim and names the citing classes; the evidence source is the citing record set. This gives the information-classes catalogue a resolvable target for every reference and unblocks their `resolution_active` flip (their follow-up CR, not this one).

## 2. Seed selection (FOUNDATIONS D-5)

Every seed is an existing cross-catalogue citation corroborated at admission: the id, the requirement text, and the citing classes all come from committed information-classes records. No controls beyond the cited twenty are admitted; further controls await their own citing evidence or a control-framework CR.

## 3. Scope

In scope: 20 record subtrees (record + README), CATALOG.yaml regeneration, register row, CHANGELOG.

Out of scope: the information-classes `resolution_active` flip and registry fill (their repository's CR); any control taxonomy or framework alignment; metamodel lifecycle backfill (wave boundary).

## 4. Acceptance criteria

1. Gates 1-6 all `Findings: 0` with 20 canonical records.
2. `CATALOG.yaml` counts: entities 20, canonical 20, open_change_requests 0.
3. Every admitted id equals a `dea:control-*` id cited by information-classes records (spot-checkable in the records' evidence).

## 5. NOT-list

1. No controls beyond the twenty cited.
2. No control-framework mappings (NIST/ISO alignment etc.) — a future CR with its own evidence.
3. No changes to information-classes or the metamodel.
