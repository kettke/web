
---
layout: default
title: "Kettke Atlas | Character Registry"
permalink: /_internal/atlas/personajes/
nav_exclude: true
search_exclude: true
description: "AI-first character inventory for the published first volume."
document_id: KETTKE.ATLAS.CHARACTERS
document_type: character_registry
schema_version: "1.0.0"
language: en-US
access_policy: public_ai_first
parent_document: KETTKE.ATLAS.ROOT
source_baseline: web-main-71
source_scope: VOL_1
verification_status: provisional
---

# KETTKE.ATLAS.CHARACTERS

## Registry semantics

```yaml
registry:
  id: KETTKE.ATLAS.CHARACTERS
  authority: VOL_1_ES_2010
  source_baseline: web-main-71
  source_directory: /novela/vol-1-hanna-y-los-reinos-de-kettke/
  chapter_index: "00 = opening; 01-22 = numbered chapters"
  entry_rule: "One record per distinct named character, with original names preserved."
  chapter_matching: "Literal, case-insensitive whole-name matches in source Markdown; aliases included."
  chapter_matching_limitations:
    - "A name match does not prove physical appearance or participation."
    - "Absence of a name match does not prove narrative absence."
    - "The listed chapters are mentions, not verified scene-level appearances."
  narrative_layers:
    PRESENT: "Associated primarily with Hanna’s narrated journey or its contemporary frame."
    PAST: "Associated primarily with narrated history, memory, or legend."
    BOTH: "Associated with the present narrative frame and accounts of the past; does not imply physical presence in both."
    UNRESOLVED: "Narrative layer not yet validated."
  editorial_classification: author_reviewed_20_primary
  completeness: not_certified
  public_character_index: /atlas/personajes/
  public_profile_paths: proposed_not_yet_published
  epistemic_rule: "Descriptions and narrative layers are provisional until passage-level review."
```

## Named character inventory

```yaml
characters:
  - id: KETTKE.CHAR.HANNA
    name: "Hanna"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [OPENING, C01, C02, C03, C04, C05, C06, C07, C08, C09, C10, C11, C12, C13, C14, C15, C16, C17, C18, C19, C20, C21, C22]
    context: "Central protagonist of Volume I."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/hanna/
  - id: KETTKE.CHAR.GUNURUK
    name: "Gunuruk"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C05, C06, C07, C08, C09, C10, C11, C12, C13, C14, C15, C16, C17, C18, C19, C20, C21, C22]
    context: "Snork who accompanies Hanna."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/gunuruk/
  - id: KETTKE.CHAR.KRON
    name: "Kron"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C02, C03, C04, C05, C06, C07, C08, C10, C19, C20, C21]
    context: "Animal companion of Hanna."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/kron/
  - id: KETTKE.CHAR.GUNUK
    name: "Gunuk"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [OPENING, C07, C09, C10, C14, C17, C18, C20, C21, C22]
    context: "Opening-sequence figure whose actions shape the narrative."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/gunuk/
  - id: KETTKE.CHAR.BAUROS
    name: "Bauros"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [OPENING, C14, C15, C16, C17, C18, C19, C20, C21, C22]
    context: "Participant in the present-day narrative and teller of historical accounts."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/bauros/
  - id: KETTKE.CHAR.VENDEMUR
    name: "Vendemur"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [OPENING, C07, C08, C09, C10, C15, C16, C17, C20, C21, C22]
    context: "Nárako referenced in the opening and historical accounts."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/vendemur/
  - id: KETTKE.CHAR.TUARKKET
    name: "Tuarkket"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [OPENING, C07, C10, C14, C15, C16, C17, C19, C20, C21, C22]
    context: "Historical king of Kettke; source spelling differs from the current canonical form."
    source_validation: name_match_only
    source_spellings: ["Tuarkkett"]
    proposed_public_profile: /atlas/personajes/tuarkket/
  - id: KETTKE.CHAR.BADANIA
    name: "Badania"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [C15, C16, C17, C19, C20, C22]
    context: "Royal figure in accounts of Kettke’s past."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/badania/
  - id: KETTKE.CHAR.ODDEON
    name: "Oddeon"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [C07, C08, C10, C15, C16, C17, C21]
    context: "King of Kings in historical accounts."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/oddeon/
  - id: KETTKE.CHAR.DRUJAS
    name: "Drujas"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [C04, C09, C10, C12, C15, C16, C17, C22]
    context: "Figure connected to Kettke’s major historical conflicts."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/drujas/
  - id: KETTKE.CHAR.KUDARK
    name: "Kudark"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [OPENING, C12, C15, C16, C17, C20, C22]
    context: "Nárako associated with historical conflicts."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/kudark/
  - id: KETTKE.CHAR.AUREON
    name: "Aureon"
    editorial_class: PRIMARY
    narrative_layer: PAST
    mentioned_in_chapters: [C15]
    context: "Historical bearer of Sium."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/aureon/
  - id: KETTKE.CHAR.KOYAN
    name: "Koyan"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [C14, C17, C19, C20, C21]
    context: "Warrior and former king of Ákador; appears in historical references and the main narrative."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/koyan/
  - id: KETTKE.CHAR.NAKIAN
    name: "Nakian"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C19, C20, C21]
    context: "Son of Koyan."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/nakian/
  - id: KETTKE.CHAR.OMMENORK
    name: "Ómmenork"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C19, C20, C21]
    context: "Companion of Koyan and Nakian."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/ommenork/
  - id: KETTKE.CHAR.AKNUS
    name: "Aknus"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C06, C07, C08, C09, C10, C12, C14, C18]
    context: "Great Chief of Antraka."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/aknus/
  - id: KETTKE.CHAR.YNACK
    name: "Ynack"
    editorial_class: PRIMARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C08, C09, C10, C11, C12, C13, C14, C20, C21]
    context: "Snork known as the traveler."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/ynack/
  - id: KETTKE.CHAR.ELISEA
    name: "Elisea"
    editorial_class: PRIMARY
    narrative_layer: BOTH
    mentioned_in_chapters: [C16, C17, C20, C22]
    context: "Figure in accounts of Oddeon’s family."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/elisea/
  - id: KETTKE.CHAR.SENIA
    name: "Senia"
    editorial_class: PRIMARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Figure in accounts of Oddeon’s family."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/senia/
  - id: KETTKE.CHAR.FESTOR
    name: "Festor"
    editorial_class: PRIMARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Figure in accounts of Oddeon’s family."
    source_validation: name_match_only
    proposed_public_profile: /atlas/personajes/festor/
  - id: KETTKE.CHAR.JOSEPH
    name: "Joseph"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C01, C02, C05, C08, C21]
    context: "Person in Hanna’s life on Earth."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#joseph
  - id: KETTKE.CHAR.FRANK
    name: "Frank"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C01]
    context: "Student in Hanna’s school environment."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#frank
  - id: KETTKE.CHAR.HINGS
    name: "Hings"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C01, C08, C11, C13, C21]
    context: "Teacher in Hanna’s school environment."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#hings
  - id: KETTKE.CHAR.ROWELL
    name: "Rowell"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C01, C21]
    context: "School director."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#rowell
  - id: KETTKE.CHAR.CONERY
    name: "Conery"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C01]
    context: "Teacher."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#conery
  - id: KETTKE.CHAR.HERN
    name: "Hern"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C01, C10]
    context: "Doctor associated with the museum discovery."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#hern
  - id: KETTKE.CHAR.PERKINS
    name: "Perkins"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C02]
    context: "Merchant encountered by Hanna."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#perkins
  - id: KETTKE.CHAR.METTMEK
    name: "Mettmek"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C06, C07, C08]
    context: "Named figure in the Antraka sequence."
    source_validation: name_match_only
    source_spellings: ["Metmek"]
    proposed_public_anchor: /atlas/personajes/#mettmek
  - id: KETTKE.CHAR.YASNEK
    name: "Yasnek"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C06, C07, C08]
    context: "Uru of Bettnuk."
    source_validation: name_match_only
    source_spellings: ["Jasnek"]
    proposed_public_anchor: /atlas/personajes/#yasnek
  - id: KETTKE.CHAR.NARSAK
    name: "Narsak"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C06, C09, C10, C12, C20]
    context: "Uru of Bakalia."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#narsak
  - id: KETTKE.CHAR.URDUK
    name: "Urduk"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C08]
    context: "Master associated with the sawmills."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#urduk
  - id: KETTKE.CHAR.KRULO
    name: "Krulo"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C13, C15]
    context: "Giant encountered in the marshes."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#krulo
  - id: KETTKE.CHAR.DROLO
    name: "Drolo"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C13, C15]
    context: "Giant encountered in the marshes."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#drolo
  - id: KETTKE.CHAR.DOKIAS
    name: "Dokias"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C14, C15]
    context: "Person involved in arranging travel toward Belonia."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#dokias
  - id: KETTKE.CHAR.KRIN
    name: "Krin"
    editorial_class: SECONDARY
    narrative_layer: PRESENT
    mentioned_in_chapters: [C19]
    context: "Dwarf identified in Chapter XIX."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#krin
  - id: KETTKE.CHAR.DEMOLAS
    name: "Démolas"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C15, C16]
    context: "Historical bearer of Sium; son of Aureon."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#demolas
  - id: KETTKE.CHAR.KIRATOR
    name: "Kírator"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Historical bearer of Sium."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#kirator
  - id: KETTKE.CHAR.BALINA
    name: "Balina"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Wife of Oddeon."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#balina
  - id: KETTKE.CHAR.TERIAN
    name: "Terian"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "King of Vérveka and father of Balina."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#terian
  - id: KETTKE.CHAR.ROHO
    name: "Roho"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Warrior and cavalry leader of Kinoria."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#roho
  - id: KETTKE.CHAR.DROKO
    name: "Droko"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Military commander in historical accounts."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#droko
  - id: KETTKE.CHAR.MIDULA
    name: "Mídula"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Wife of Droko."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#midula
  - id: KETTKE.CHAR.BREOK
    name: "Breok"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Figure associated with the origin of Drokolas."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#breok
  - id: KETTKE.CHAR.KRODOR
    name: "Krodor"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C17]
    context: "Father of Badania."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#krodor
  - id: KETTKE.CHAR.ARIAN
    name: "Arian"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C17]
    context: "Mother of Badania."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#arian
  - id: KETTKE.CHAR.IVELOR
    name: "Ívelor"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C17]
    context: "Warrior connected with Badania’s youth."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#ivelor
  - id: KETTKE.CHAR.KADOR
    name: "Kador"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C14]
    context: "Historical king of Ákador."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#kador
  - id: KETTKE.CHAR.DREONTE
    name: "Dreonte"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C14, C17, C19]
    context: "Historical figure in accounts of Koyan."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#dreonte
  - id: KETTKE.CHAR.YLATROK
    name: "Ýlatrok"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C19]
    context: "Identified by Koyan as his father."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#ylatrok
  - id: KETTKE.CHAR.ELAM
    name: "Elam"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C14, C16, C17]
    context: "Son of Bauros."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#elam
  - id: KETTKE.CHAR.FILIAN
    name: "Filian"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C14, C16, C17]
    context: "Son of Bauros."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#filian
  - id: KETTKE.CHAR.KERION
    name: "Kerion"
    editorial_class: SECONDARY
    narrative_layer: PAST
    mentioned_in_chapters: [C16]
    context: "Figure in the historical accounts of Oddeon’s descendants."
    source_validation: name_match_only
    proposed_public_anchor: /atlas/personajes/#kerion
```

## Individually identified nonhuman entities

```yaml
cross_registry_candidates:
  - name: "Babuk"
    mentioned_in_chapters: [C16]
    proposed_owner: KETTKE.ATLAS.BESTIARY
    character_identity_status: pending
  - name: "Drácadork"
    mentioned_in_chapters: [C17]
    proposed_owner: KETTKE.ATLAS.BESTIARY
    character_identity_status: pending
```

## Unnamed characters and coverage gaps

```yaml
unresolved:
  - id: KETTKE.CHAR.UNNAMED.BAUROS_SPOUSE
    designation: "Bauros’s wife"
    narrative_layer: PAST
    source_context: "Family accounts involving Bauros"
    chapter_verification: pending
    editorial_class: SECONDARY
  - id: KETTKE.CHAR.UNNAMED.OTHER
    designation: "Other unnamed individuals with distinct narrative agency"
    inventory_status: pending_exhaustive_pass
audit_queue:
  - identify_all_named_characters_not_in_current_registry
  - review_anonymous_characters_for_individual_identity
  - verify_chapter_context_for_each_name_match
  - distinguish historical accounts from present physical appearances
  - validate entity identities and spelling variants
  - verify proposed public URLs before linking
  - add evidence_ids_and_cross_domain_links_after_source_review
```

## Relationship and evidence requirements

```yaml
relationship_contract:
  required: [subject_id, predicate, object_id, evidence_id, epistemic_status]
  allowed_target_domains:
    - KETTKE.ATLAS.CHARACTERS
    - KETTKE.ATLAS.GEOGRAPHY
    - KETTKE.ATLAS.HISTORY
    - KETTKE.ATLAS.PEOPLES
    - KETTKE.ATLAS.BESTIARY
    - KETTKE.ATLAS.LANGUAGE
  constraints:
    - "Do not infer a relationship from chapter co-occurrence alone."
    - "Do not treat a narrated legend as independently verified history."
    - "Do not expose unpublished Volume II or III developments."
    - "Do not convert a proposed URL into an asserted existing page."
    - "Preserve identity across all future published volumes."
  relationship_records: []
  evidence_records: []
```
