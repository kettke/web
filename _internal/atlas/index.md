---
layout: default
title: "Kettke Atlas | AI Registry"
permalink: /_internal/atlas/
nav_exclude: true
search_exclude: true
description: "Machine-first registry governing the Kettke Atlas knowledge architecture."

document_id: KETTKE.ATLAS.ROOT
document_type: atlas_root_registry
schema_version: "1.0.0"
document_status: initial
language: en-US
access_policy: public_ai_first
navigation_visibility: hidden

authority: published_canon
active_publication_scope: VOL_1
primary_source_language: es
canonical_work: "Hanna y los Reinos de Kettke"
canonical_work_publication_year: 2010
---

# KETTKE.ATLAS.ROOT

```yaml
registry:
  id: KETTKE.ATLAS.ROOT
  type: atlas_root_registry
  status: initial
  audience: ai_agents
  human_readability: non_priority

  purpose:
    - entity_registration
    - canonical_alignment
    - relationship_mapping
    - evidence_traceability
    - narrative_continuity
    - controlled_expansion

  constraints:
    - no_fabricated_entities
    - no_unverified_canonical_claims
    - no_unmarked_inference
    - no_unpublished_spoiler_disclosure
    - no_silent_source_reconciliation
    - no_destructive_history_rewrite
```

## 01. AUTHORITY MODEL

```yaml
source_hierarchy:
  - rank: 1
    id: AUTHOR_VALIDATED_CANON
    role: explicit_authorial_decisions
    condition: documented_and_scope_qualified

  - rank: 2
    id: VOL_1_ES_2010
    role: published_literary_source
    language: es
    scope: VOL_1

  - rank: 3
    id: NARRATIVE_EVIDENCE_MAP
    path: /_internal/mapa-narrativo-vol-1/
    role: evidence_navigation
    authority: derived
    verification_required: true

  - rank: 4
    id: PUBLIC_ATLAS
    path: /atlas/
    role: published_reference
    authority: derived

  - rank: 5
    id: VOL_1_EN
    role: translated_literary_source
    language: en-US
    authority: translation
    source_of_truth: VOL_1_ES_2010

conflict_policy:
  preserve_conflicting_evidence: true
  identify_source_and_scope: true
  request_author_validation_when_required: true
  prohibit_silent_resolution: true
```

## 02. PUBLICATION BOUNDARY

```yaml
publication:
  current_scope: VOL_1
  published:
    - VOL_1
  future:
    - VOL_2
    - VOL_3

  future_volume_status: not_publicly_released

  expansion_model: additive
  preserve_historical_states: true

  public_claim_policy:
    require_published_evidence: true
    allow_author_validated_public_information: true
    prohibit_unreleased_plot_disclosure: true

  spoiler_boundary:
    unit: chapter
    progression: cumulative
    atlas_default: spoiler_cautious
    explicit_spoiler_marking: required_when_applicable
```

## 03. REGISTRY TOPOLOGY

```yaml
parent:
  id: KETTKE.ATLAS.ROOT
  path: /_internal/atlas/

children:
  - id: KETTKE.ATLAS.CHARACTERS
    source_file: personajes.md
    entity_domain: characters
    public_path: /atlas/personajes/

  - id: KETTKE.ATLAS.GEOGRAPHY
    source_file: geografia.md
    entity_domain: geography
    public_path: /atlas/geografia/

  - id: KETTKE.ATLAS.BESTIARY
    source_file: bestiario.md
    entity_domain: bestiary
    public_path: /atlas/bestiario/

  - id: KETTKE.ATLAS.HISTORY
    source_file: historia.md
    entity_domain: history
    public_path: /atlas/historia/

  - id: KETTKE.ATLAS.PEOPLES
    source_file: pueblos-y-culturas.md
    entity_domain: peoples_and_cultures
    public_path: /atlas/pueblos-y-culturas/

  - id: KETTKE.ATLAS.LANGUAGE
    source_file: lenguaje.md
    entity_domain: language_and_writing
    public_path: /atlas/lengua-y-escritura/

child_status:
  initial_state: planned
  require_individual_validation: true
```

## 04. ENTITY CONTRACT

```yaml
entity_schema:
  required:
    - entity_id
    - canonical_name
    - entity_type
    - registry_owner
    - source_scope
    - epistemic_status

  optional:
    - aliases
    - classification
    - narrative_role
    - first_verified_reference
    - evidence
    - relationships
    - public_reference
    - spoiler_level
    - validation_status

  identity_rules:
    preserve_original_names: true
    normalize_identifiers: true
    prohibit_name_based_identity_merging: true
    allow_aliases_with_evidence: true
    require_authority_for_canonical_renaming: true

  identity_persistence:
    across_volumes: true
    across_languages: true
    across_public_pages: true
```

## 05. RELATIONSHIP CONTRACT

```yaml
relationship_schema:
  required:
    - subject_id
    - predicate
    - object_id
    - epistemic_status
    - evidence_reference

  optional:
    - narrative_scope
    - chapter
    - chronology
    - spoiler_level
    - inverse_predicate
    - validation_status

  predicates:
    - appears_in
    - mentioned_in
    - originates_from
    - located_in
    - belongs_to
    - associated_with
    - participates_in
    - related_to
    - governed_by
    - occurs_at
    - documented_in

  relationship_policy:
    typed_edges: preferred
    bidirectional_navigation: when_relevant
    reciprocal_assertion: only_when_valid
    infer_relationship_from_cooccurrence: false
    infer_physical_presence_from_mention: false
    infer_historical_fact_from_character_statement: false
```

## 06. EPISTEMIC CONTRACT

```yaml
epistemic_status:
  - EXPLICIT
  - INFERRED
  - REPORTED
  - DISPUTED
  - UNKNOWN
  - AUTHOR_VALIDATED

interpretation:
  EXPLICIT: directly_supported_by_source
  INFERRED: reasoned_but_not_directly_confirmed
  REPORTED: asserted_within_narrative
  DISPUTED: conflicting_or_contested_evidence
  UNKNOWN: insufficient_evidence
  AUTHOR_VALIDATED: explicitly_confirmed_by_author

requirements:
  inference_must_be_labeled: true
  reported_claim_is_not_automatic_fact: true
  unknown_must_not_be_filled_by_generation: true
  author_validation_requires_traceable_record: true
```

## 07. EVIDENCE CONTRACT

```yaml
evidence_schema:
  required:
    - source_id
    - source_location
    - evidence_type
    - verification_status

  optional:
    - chapter_id
    - passage_locator
    - quotation
    - interpretation
    - source_version

  evidence_types:
    - direct_narration
    - character_dialogue
    - textual_mention
    - authorial_confirmation
    - derived_analysis

  validation:
    textual_mention_is_not_presence: true
    dialogue_is_not_automatic_truth: true
    derived_analysis_is_not_primary_source: true
    chapter_references_require_verification: true
    source_version_tracking: required
```

## 08. CHARACTER STORAGE POLICY

```yaml
characters:
  coverage: all_verified_characters
  include_named_mentions: true

  primary:
    storage: individual_public_file
    registry: KETTKE.ATLAS.CHARACTERS

  secondary:
    storage: public_character_index
    registry: KETTKE.ATLAS.CHARACTERS

  classification:
    editorial: true
    mutable_across_publications: true
    spoiler_sensitive: true

  migration:
    secondary_to_primary: permitted
    preserve_entity_id: true
    preserve_evidence_history: true
    preserve_relationships: true
```

## 09. PUBLIC / INTERNAL SEPARATION

```yaml
layers:
  public_atlas:
    audience: readers
    languages:
      - es
      - en-US
    format: editorial_reference
    spoiler_policy: reader_safe

  internal_atlas:
    audience: ai_agents
    language: en-US
    format: structured_machine_first
    visibility: direct_access
    navigation: hidden
    search: hidden

  narrative:
    audience: readers
    integrity: immutable_without_editorial_authorization

  chapter_companions:
    audience: readers
    role: progressive_context
    maximum_knowledge: current_chapter

separation_rules:
  public_pages_are_not_canonical_evidence_by_themselves: true
  internal_registries_do_not_replace_primary_sources: true
  chapter_context_must_not_reveal_future_events: true
  no_unnecessary_content_duplication: true
```

## 10. DEPENDENCY GRAPH

```text
PUBLISHED NOVEL
    |
    v
NARRATIVE EVIDENCE MAP
    |
    v
ATLAS ROOT REGISTRY
    |
    +-- CHARACTERS
    +-- GEOGRAPHY
    +-- BESTIARY
    +-- HISTORY
    +-- PEOPLES_AND_CULTURES
    +-- LANGUAGE
    |
    v
CROSS-DOMAIN RELATIONSHIPS
    |
    v
PUBLIC ATLAS
    |
    v
CHAPTER COMPANIONS

AI CANON:
  governs interpretation across all layers
```

## 11. UPDATE PROTOCOL

```yaml
pipeline:
  - identify_source_change
  - determine_affected_entities
  - verify_primary_evidence
  - update_domain_registry
  - validate_cross_domain_relationships
  - evaluate_spoiler_boundaries
  - review_public_page_impact
  - update_public_content_when_authorized
  - record_version_change

quality_constraints:
  local_correctness: required
  global_consistency: required
  provenance: required
  historical_continuity: required

failure_pattern:
  id: LOCALLY_BETTER_GLOBALLY_WORSE
  prevention: cross_registry_validation
```

## 12. INITIALIZATION STATE

```yaml
initialization:
  baseline_repository: web-main-71
  narrative_scope: VOL_1
  evidence_map:
    status: provisional
    requires_current_source_audit: true

  registries:
    characters: planned
    geography: planned
    bestiary: planned
    history: planned
    peoples_and_cultures: planned
    language: planned

  entity_inventory_complete: false
  relationships_validated: false
  public_atlas_fully_audited: false

  next_operation:
    registry: KETTKE.ATLAS.CHARACTERS
    action: initialize_from_verified_vol_1_evidence
```

## 13. CANON INTERFACE

```yaml
canon_interface:
  authority_document: /ai/canon/

  alignment_dimensions:
    - CANON
    - HISTORY
    - RELATIONSHIPS
    - EPISTEMIC_STATUS
    - HORIZONTE

  execution_rule:
    preserve_global_coherence: true
    ask_before_unverified_canonical_change: true
    prefer_evidence_over_completion: true
    preserve_authorial_sovereignty: true

  root_registry_role:
    governs_atlas_structure: true
    overrides_literary_source: false
    overrides_authorial_canon: false
```
