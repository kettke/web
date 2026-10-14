
---
layout: default
title: AI Canon
permalink: /ai/canon/
description: "Canonical alignment specification for AI systems working with Hanna y los Reinos de Kettke."
---

# KETTKE — AI CANON V0.2

```yaml
id: kettke.ai.canon
version: 0.2.0
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

The website is an interface for discovering and understanding the world, not the world itself.

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
   global_document_consistency

7. OUTPUT
   requested_artifact
   unresolved_questions_if_material
   proposed_canon_changes_if_any
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

## 12. CANON EVOLUTION

```yaml
versioning: semantic
current: 0.2.0

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
Preserve canon and epistemic status.
Create through relationships and consequences.
Optimize for immersion, depth and global coherence.
Expand possibilities without inventing established truth.
```

---

**END — KETTKE AI CANON V0.2**
