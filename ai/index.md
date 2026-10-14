---
layout: default
title: AI Canon
nav_order: 99
permalink: /ai/canon/
description: "Canonical alignment specification for AI systems working with Hanna y los Reinos de Kettke."
---

# KETTKE — AI CANON V0.3

```yaml
id: kettke.ai.canon
version: 0.3.0
status: provisional
type: ai-alignment-spec
authority: author
language: es
scope:
  - novel
  - trilogy
  - atlas
  - website
  - transmedia
site: https://kettke.com
```

## 0. EXECUTION MODEL

```text
OBJECTIVE =
  preserve_identity
  + preserve_coherence
  + enable_discovery
  + support_expansion

ALIGNMENT =
  CANON
  + HISTORY
  + RELATIONSHIPS
  + EPISTEMIC_STATUS
  + HORIZONTE

PIPELINE =
  SOURCE
  → EXTRACT
  → CLASSIFY
  → RELATE
  → REASON
  → GENERATE
  → VALIDATE

OPTIMIZATION =
  maximize(
    narrative_fidelity,
    global_coherence,
    emotional_depth,
    immersion,
    discoverability
  )

CONSTRAINTS =
  canonical_integrity
  + epistemic_accuracy
  + spoiler_scope
  + evidence_traceability
  + reader_knowledge_boundary

PRIMARY_FAILURE =
  LOCALLY_BETTER / GLOBALLY_WORSE
```

## 1. WORLD MODEL

```yaml
work:
  title: Hanna y los Reinos de Kettke
  genre: fantasy_adventure
  architecture: coherent_parallel_world
  primary_arc: trilogy
  expansion: earth_and_parallel_universes

entities:
  Kettke:
    type: historical_kingdom
    designation: Reino de los Reinos
    not_equivalent_to:
      - planet
      - Tierra Conocida

  Tierra_Conocida:
    type: geographical_region
    world: parallel_to_Earth

  Tierra:
    type: human_origin_world
    distinct_from: Tierra_Conocida

world_properties:
  historical_depth: essential
  geography: causally_relevant
  cultures: differentiated
  politics: historically_conditioned
  species: diverse
  magic: present_but_not_dominant
  continuity: persistent
  narrative_knowledge: partial
```

**INVARIANT:** `Kettke != Tierra_Conocida != Tierra`

## 2. NARRATIVE CORE

```yaml
protagonist: Hanna

initial_state:
  origin_knowledge: incomplete
  primary_motivation: discover_identity_and_family
  historical_awareness: incomplete

volume_1_transition:
  personal_search: historical_discovery
  unknown_origin: revealed_family_history
  inherited_past: emerging_future_responsibility

trilogy_trajectory:
  focus: true_identity_and_evolution
  final_state: author_defined_not_publicly_resolved

central_tensions:
  - personal_identity <-> collective_history
  - inherited_destiny <-> freedom_of_choice
  - power <-> moral_responsibility
  - historical_violence <-> aspiration_for_peace
  - extraordinary_potential <-> ordinary_humanity
  - hope <-> sacrifice
```

**INVARIANT:** Hanna remains a person, not merely a vehicle for power, prophecy or political restoration.

## 3. THEMATIC ENGINE

```text
HISTORICAL VIOLENCE
  → loss / trauma / separation
  → collective memory
  → divergent responses
  → persistent conflict
  → renewed aspiration for peace

PERSONAL LOSS
  → questions about identity
  → discovery of relationships
  → confrontation with inherited history
  → autonomous decisions
  → character transformation

POWER != MORAL LEGITIMACY

DESTINY != ELIMINATION OF FREE WILL

PEACE != AUTOMATIC CONSEQUENCE OF MILITARY VICTORY

HEROISM != EXCLUSIVE PROPERTY OF POWERFUL CHARACTERS
```

```yaml
moral_model:
  good:
    expressions:
      - compassion
      - justice
      - loyalty
      - protection
      - love
      - sacrifice

  evil:
    expressions:
      - cruelty
      - domination
      - betrayal
      - destructive_ambition
      - hatred

  moral_agency:
    unit: individual_decision
    species_determinism: false
    social_position_determinism: false
```

Good and evil are central themes. Individual motivations and historical circumstances require contextual interpretation.

## 4. CANONICAL ENTITY GRAPH — SEED

```yaml
Hanna:
  role: protagonist
  origin: Tierra
  parents:
    - Tuarkkett
    - Badania
  companion: Gunuruk
  relation_to_Sium: legitimate_bearer
  full_identity: reserved

Sium:
  category: superior_power_element
  full_nature: reserved
  conventional_sword: false

Gunuruk:
  species: Snork
  relation_to_Hanna: companion_and_friend
  father: Gunuk
  anatomy:
    tail: absent
  characterization:
    - humorous
    - impulsive
    - compassionate
    - courageous

Gunuk:
  role: protector_of_infant_Hanna
  father_of: Gunuruk
  narrative_function: sacrifice_and_historical_continuity

Bauros:
  role: historical_witness
  narrative_function: collective_memory_and_hope

Vendemur:
  species: Narako
  narrative_function: knowledge_destiny_and_free_will

Tuarkkett:
  relation_to_Hanna: father

Badania:
  relation_to_Hanna: mother

Kron:
  role: recurring_character
  detail_source: novel_and_atlas

Drujas:
  role: major_antagonistic_force
  detail_source: novel_and_atlas
```

### Entity and relationship provenance

Each claim extracted from this graph must retain its provenance and narrative scope. A relationship stated in a later chapter may be canonical for the full volume while remaining unknown to a reader of an earlier chapter.

```yaml
relationship_record:
  subject: entity_id
  predicate: relation_type
  object: entity_id_or_value
  source: source_path_or_author_decision
  location: chapter_or_section
  evidence_kind: explicit_event_or_statement_or_inference
  speaker: narrator_or_character_or_document
  epistemic_status: CONFIRMED_or_INFERRED_or_UNKNOWN_or_CONFLICT_or_RESERVED
  reader_available_from: verified_chapter_or_unknown
  verification: verified_or_pending
```

**RULE:** textual mention != physical appearance != verified relationship. A name-count index is a discovery aid, not independent evidence of an event.

This graph is a retrieval seed, not a complete character database.

Full biographies, relationships and chronology belong in specialized canonical files.

## 5. TAXONOMY

```yaml
Seres:
  definition: reasoning_species
  examples:
    - humanos
    - Snorks
    - Babagos
    - enanos

Criaturas:
  definition: fantastical_lifeforms
  examples:
    - Tuarks

Bestias:
  definition: animals
  morality: not_implied_by_category
  examples:
    - Nibuk
    - Bolok
```

Species, culture, political organization and moral character are separate dimensions.

## 6. NARRATIVE TIMELINE

```yaml
volume_I:
  title: Hanna y los Reinos de Kettke
  state: published
  scope: origin_search_and_initial_discovery

volume_II:
  title: Hanna y la búsqueda de Sium
  state: planned
  detailed_events: reserved

volume_III:
  title: Hanna y la conquista de Kinoria
  state: planned
  detailed_events: reserved

post_trilogy:
  scope: transmedia_expansion
  includes:
    - Tierra
    - parallel_universes
  protagonist_continuity: required
  detailed_events: reserved
```

The first volume is not the complete resolution of Hanna's identity or destiny.

### Knowledge progression across the first volume

```yaml
knowledge_layers:
  world_fact: what_the_primary_sources_establish
  character_knowledge: what_a_character_knows_at_a_given_time
  character_belief: what_a_character_believes_or_reports
  reader_knowledge: what_the_text_has_revealed_up_to_a_chapter
  atlas_knowledge: what_the_public_reference_page_exposes
  author_reserved: what_the_author_has_not_authorized_for_release

chapter_boundary:
  input: volume_and_last_read_chapter
  output: statements_safe_at_that_point
  default_when_unknown: do_not_assume_full_volume_read
```

**VOLUME I EXAMPLE — SPOILER CONTROL:** The relationship of Hanna to Tuarkkett and Badania is stated in the canonical entity seed, but must not be disclosed in guidance intended for readers before its narrative revelation. The internal narrative map identifies chapter XXII as an explicit recognition scene. This is a working locator: inspect the chapter before using it to authorize a contextual link.

**Sium:** a character's wording about wielding Sium does not override the canon classification `superior_power_element`; `conventional_sword: false` remains invariant.

**FIRST OCCURRENCE RULE:** distinguish first literal mention, first witnessed appearance, first explanation and first confirmed revelation. Do not derive one from another.

## 7. EPISTEMIC STATUS

```yaml
CONFIRMED:
  definition: supported_by_primary_source_or_author
  publication: allowed_with_spoiler_check

RESERVED:
  definition: author_defined_but_not_publicly_revealed
  publication: restricted

INFERRED:
  definition: interpretation_supported_by_evidence
  publication: allowed_if_labeled

UNKNOWN:
  definition: insufficient_evidence
  action: retrieve_or_request_source

CONFLICT:
  definition: incompatible_source_claims
  action: preserve_evidence_and_escalate

PROPOSED:
  definition: new_creative_content
  authority: none_until_approved
```

### Source precedence

```text
CURRENT AUTHOR DECISION
  > APPROVED CANON
  > PRIMARY NOVEL TEXT
  > VERIFIED SUPPLEMENTARY MATERIAL
  > INTERPRETATION
  > GENERATION
```

Source precedence must respect narrative scope.

A character's belief, a legend and an objective fact do not automatically share the same epistemic status.

No generated statement becomes canon merely through repetition.

### Evidence handling

```yaml
evidence_states:
  VERIFIED: source_passage_and_context_checked
  CANDIDATE: plausible_relation_or_destination_not_yet_checked
  REJECTED: unsupported_or_conflicting_with_source
  UNAVAILABLE: source_not_accessible_or_not_yet_written

claim_handling:
  preserve_exact_source_meaning: true
  distinguish_dialogue_from_narrator: true
  preserve_unresolved_conflicts: true
  require_source_for_specific_first_appearance: true
  require_author_approval_for_new_canon: true
```

**PUBLICATION RULE:** `CONFIRMED` is a claim's epistemic status; `VERIFIED` is the evidence-review state. Neither alone grants spoiler clearance. An approved relationship can still be unsafe to reveal at a given reading point.

## 8. HORIZONTE — CREATIVE ALIGNMENT

```yaml
target_experience:
  primary: immersion_in_a_coherent_living_world
  secondary:
    - emotional_connection
    - curiosity
    - exploration
    - historical_understanding
    - attachment_to_characters
    - desire_to_continue_the_story

narrative_identity:
  fantasy: wonder_through_discovery
  depth: causal_and_historical
  emotion: character_decisions_and_consequences
  epic_scale: earned_through_context
  humor: integrated_with_character_identity
  mystery: progressively_revealed
  magic: contextual_not_default_explanation

creative_direction:
  preserve_existing_relations: true
  expand_through_verified_context: true
  distinguish_fact_from_invention: true
  maintain_character_agency: true
  preserve_revelation_timing: true
  prefer_world_specificity_over_genre_templates: true
```

**GUIDING MODEL:**

```text
A world with history.
Characters with agency.
Consequences with persistence.
Mysteries with purpose.
```

The objective is meaningful immersion consistent with the source, not maximum spectacle.

## 9. WEBSITE ALIGNMENT

```yaml
website:
  domain: kettke.com
  function: narrative_world_gateway
  audience:
    - readers
    - explorers
    - AI_agents

  primary_sections:
    - Inicio
    - Atlas
    - Novela
    - Multiverso

  atlas:
    - Geografia
    - Personajes
    - Pueblos_y_Culturas
    - Bestiario
    - Historia
    - Lengua_y_Escritura

  presentation:
    human_layer: evocative_and_accessible
    machine_layer: structured_and_traceable

  principles:
    - discovery_before_exhaustive_exposition
    - source_traceability
    - explicit_entity_relationships
    - controlled_spoilers
    - consistency_across_pages
```

### Three-way discovery model

```yaml
navigation_paths:
  novel_to_atlas:
    purpose: optional_context_during_reading
    require: verified_destination_and_spoiler_safe_excerpt
  atlas_to_novel:
    purpose: locate_narrative_appearance_or_development
    require: chapter_reference_with_verified_relation_type
  visitor_to_atlas:
    purpose: standalone_discovery_without_prior_reading
    require: self_contained_explanation_and_further_connections

link_review:
  status: CANDIDATE_until_destination_and_context_verified
  verify:
    - exact_published_url
    - destination_heading_or_anchor
    - relationship_to_source_chapter
    - spoiler_scope
    - clarity_for_first_time_visitor
```

**SOURCE DEPENDENCY:** `_internal/mapa-narrativo-vol-1.md` is a working concordance and evidence locator, not a final authority for approved links. It is marked work version 0.1, uses literal mentions and contains unaudited relationships. Consult the primary novel and the relevant Atlas page before promoting a candidate.

**INTERNAL VISIBILITY:** a repository file excluded from site navigation is not necessarily private. Material reserved by the author must not be placed in a publicly accessible repository merely because `nav_exclude` or `search_exclude` is set.

**ROUTES:** canonical AI document is `/ai/canon/`; homepage references must use that route. The website is an interface for discovering and understanding the world, not the world itself.

## 10. AI WORKFLOW

```text
INPUT(request)

1. IDENTIFY
   task_type
   affected_entities
   narrative_period
   intended_audience
   spoiler_scope

2. RETRIEVE
   relevant_canon
   primary_source_passages
   related_entities
   existing_site_content
   internal_narrative_map_when_available
   exact_destination_and_anchor_when_linking

3. CLASSIFY
   confirmed
   reserved
   inferred
   unknown
   conflicting
   proposed

4. BUILD_CONTEXT
   history
   geography
   relationships
   motivations
   causal_dependencies

5. GENERATE
   satisfy_user_goal
   follow_horizonte
   preserve_narrative_identity

6. VALIDATE
   factual_consistency
   temporal_consistency
   geographical_consistency
   character_consistency
   epistemic_accuracy
   spoiler_integrity
   evidence_provenance
   chapter_knowledge_boundary
   link_destination_accuracy
   global_document_consistency

7. OUTPUT
   requested_artifact
   unresolved_questions_if_material
   proposed_canon_changes_if_any
   verification_status_of_new_links_and_claims
```

## 11. GLOBAL CONSERVATION

```text
QUALITY(output) =
  local_usefulness
  + source_fidelity
  + narrative_depth
  + global_coherence
  + long_term_compatibility
```

A locally elegant result that damages established continuity is not an improvement.

When uncertainty affects a central fact, preserve the uncertainty and seek evidence.

When multiple interpretations are supported, retain their status as interpretations.

When a new idea is useful, present it as a proposal until validated.

When adapting the work to another medium, preserve narrative identity while allowing medium-specific expression.

**CHARACTER CONTINUITY:** post-trilogy Hanna is the continuation of the same character, not a reboot or a new character sharing her name. Future states and powers remain reserved until the author authorizes disclosure. A public document must not turn an intended future trajectory into a prematurely revealed event.

**DOCUMENT CHANGE CHECK:** before changing a public page, inspect its incoming and outgoing relationships, affected canon claims, chronology and spoiler exposure. A locally improved paragraph is not an improvement if it silently invalidates other pages.

## 12. CANON EVOLUTION

```yaml
versioning: semantic
current: 0.3.0

change_types:
  PATCH: correction_without_conceptual_change
  MINOR: additive_canon_or_new_relationships
  MAJOR: foundational_revision_author_approved

update_protocol:
  - identify_affected_claims
  - inspect_source_evidence
  - map_dependencies
  - propose_change
  - validate_against_global_canon
  - record_decision
  - update_related_pages_and_relationships_if_approved
  - check_public_spoiler_exposure

authority_to_approve_canon: author
```

## 13. ALIGNMENT TESTS

```text
T01: distinguish Kettke from Tierra Conocida and Earth.

T02: recognize Hanna's personal and historical narrative dimensions.

T03: preserve the importance of free choice within destiny.

T04: understand peace as a historical and moral aspiration.

T05: preserve Gunuruk's identity and tailless anatomy.

T06: avoid reducing Sium to an ordinary sword.

T07: distinguish the first volume from the complete trilogy.

T08: preserve uncertainty around reserved revelations.

T09: avoid converting literary interpretations into facts.

T10: produce creative work consistent with the established world.

T11: maintain coherence across documents and media.

T12: distinguish the author's canon from AI-generated proposals.

T13: distinguish first mention from physical appearance and verified revelation.

T14: explain a character's belief without silently treating it as objective fact.

T15: respect the reader's last-read chapter and avoid later revelations.

T16: treat the internal narrative map as a working locator, not as self-validating canon.

T17: check exact public URLs and anchors before recommending contextual links.

T18: support novel → Atlas, Atlas → novel and standalone visitor → Atlas navigation.

T19: preserve post-trilogy Hanna as the same character without disclosing reserved developments.

T20: validate cross-page dependencies before accepting a local documentation improvement.
```

## 14. COMPACT ALIGNMENT ANCHOR

```text
KETTKE is a coherent fantasy world parallel to Earth.

The Kingdom of Kettke and the geographical region known as
Tierra Conocida are distinct entities.

HANNA begins by searching for her identity and family.
Her journey intersects with a much older history of
division, conflict, sacrifice and hope.

The narrative's deepest tensions involve good and evil,
destiny and free will, inherited history and individual
choice, extraordinary power and human identity.

PEACE is a central aspiration, not an automatic outcome
of conquest.

The world must feel historically real, culturally diverse
and causally consistent.

Characters possess agency, emotional depth and relationships.
Small decisions can carry profound moral significance.

Magic exists but does not define the entire experience.

The trilogy progressively reveals Hanna's identity.
Future expansions must preserve her continuity.

AI ROLE:
Understand the world before generating.
Preserve canon, evidence provenance and epistemic status.
Create through relationships and consequences.
Optimize for immersion, depth and global coherence.
Expand possibilities without inventing established truth.
Respect chapter-specific knowledge and verify every contextual link.
```

---

**END — KETTKE AI CANON V0.3**
