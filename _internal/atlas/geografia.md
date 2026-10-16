
---
layout: default
title: "Kettke Atlas | Geography Registry"
permalink: /_internal/atlas/geografia/
nav_exclude: true
search_exclude: true
description: "AI-first geographic registry for Volume I of Hanna and the Kettke Kingdoms."
document_id: KETTKE.ATLAS.GEOGRAPHY
document_type: geography_registry
schema_version: "1.0.0"
language: en-US
access_policy: public_ai_first
parent_document: KETTKE.ATLAS.ROOT
source_scope: VOL_1
verification_status: provisional
---

# KETTKE.ATLAS.GEOGRAPHY

## 1. Purpose and authority

This document is the master geographic registry for Volume I of *Hanna and the Kettke Kingdoms*.

It records:

- All 26 distinct place names identified on the published map of Kett Vurk.
- Additional geographic locations identified in the Spanish narrative.
- Primary and secondary geographic entities.
- Political territories, settlements, natural features, buildings, and historical locations.
- Geographic relationships supported by the published material.
- The distinction between mapped locations and text-only locations.

The original Spanish novel and its published map are the authoritative sources.

The English translation is not an independent source of canon.

A place does not need to be mentioned in the narrative to belong to the published geographic canon if it appears on the original map.

Conversely, a place does not need to appear on the map to belong to the canon if it is identified in the narrative.

This registry must not introduce unpublished information from later volumes.

## 2. Cartographic orientation

The original map uses the following orientation:

```yaml
cartographic_orientation:
  north: TOP
  south: BOTTOM
  east: LEFT
  west: RIGHT

  interpretation:
    upper_left: NORTHEAST
    upper_right: NORTHWEST
    lower_left: SOUTHEAST
    lower_right: SOUTHWEST

  authority: AUTHOR_CONFIRMED

  constraints:
    - "Never assume east is on the right."
    - "Never reverse the author's stated orientation."
    - "Do not infer exact distances from label positions."
    - "Do not infer political borders without supporting evidence."
    - "Do not treat approximate map positions as geographic coordinates."
```

All relative geographic directions must respect this orientation.

The position of a printed label is not necessarily the exact center of the territory it identifies.

## 3. Geographic identity model

```yaml
registry:
  id: KETTKE.ATLAS.GEOGRAPHY
  authority:
    - VOL_1_ORIGINAL_MAP
    - VOL_1_SPANISH_NARRATIVE
    - AUTHOR_CONFIRMED_CLARIFICATIONS

  mapped_toponym_count: 26

  geographic_classification:
    PRIMARY:
      meaning: "Author-approved location requiring an individual public Atlas profile."
    SECONDARY:
      meaning: "Location documented in the general public geography index."

  evidence_types:
    MAP:
      meaning: "Identified on the published map."
    TEXT:
      meaning: "Identified in the Spanish narrative."
    BOTH:
      meaning: "Supported by the map and the narrative."
    AUTHOR:
      meaning: "Explicitly clarified by the author."

  geographic_types:
    - WORLD_REGION
    - KINGDOM
    - TERRITORY
    - REGION
    - CITY
    - SETTLEMENT
    - ISLAND
    - FOREST
    - DESERT
    - MOUNTAIN
    - MOUNTAIN_RANGE
    - VOLCANO
    - CLIFFS
    - LAKE
    - SEA
    - MARSH
    - PALACE
    - BUILDING
    - HISTORICAL_TERRITORY
    - COLLECTIVE_REGION
    - UNRESOLVED

  temporal_context:
    PRESENT: "Relevant to the main narrative period."
    PAST: "Known primarily through historical accounts."
    BOTH: "Referenced in both contemporary and historical contexts."
    UNRESOLVED: "Temporal context requires verification."

  rules:
    - "One stable ID per distinct geographic entity."
    - "A kingdom and a city with the same name may be separate entities."
    - "A territory and a natural feature with the same name may be separate entities."
    - "Do not merge entities solely because their names are similar."
    - "Do not invent political affiliation, borders, or distances."
    - "Do not confuse narrative mention with direct travel."
    - "Preserve historical changes in territorial identity."
    - "Do not treat absence from the map as evidence of nonexistence."
    - "Do not treat absence from the text as evidence of nonexistence."
    - "Use canonical proper names in all languages."

  completeness: PROVISIONAL
```

## 4. Primary geography

The following 20 geographic entries have been selected for individual public Atlas profiles.

This is an editorial classification, not a ranking of political importance or geographic size.

```yaml
primary_geography:
  - id: KETTKE.GEO.KETTKE
    name: "Kettke"
    type: TERRITORY
    evidence: BOTH
    temporal_context: BOTH
    context: "Central political and historical location associated with the Kingdom of Kingdoms."
    proposed_public_profile: /atlas/geografia/kettke/

  - id: KETTKE.GEO.ANTRAKA
    name: "Antraka"
    map_name: "Reino de Antraka"
    type: KINGDOM
    evidence: BOTH
    temporal_context: PRESENT
    context: "Kingdom associated with the Snorks and Hanna's journey."
    proposed_public_profile: /atlas/geografia/antraka/

  - id: KETTKE.GEO.AKADOR
    name: "Ákador"
    map_name: "Reino de Ákador"
    type: KINGDOM
    evidence: BOTH
    temporal_context: BOTH
    context: "Kingdom associated with Koyan and important historical accounts."
    proposed_public_profile: /atlas/geografia/akador/

  - id: KETTKE.GEO.YRANDIA
    name: "Yrandia"
    type: KINGDOM
    evidence: TEXT
    temporal_context: PRESENT
    context: "Hidden kingdom reached during Hanna's journey."
    proposed_public_profile: /atlas/geografia/yrandia/

  - id: KETTKE.GEO.ARGON
    name: "Argon"
    type: TERRITORY
    evidence: TEXT
    temporal_context: PRESENT
    context: "Territory associated with the Mibuks and the route toward Yrandia."
    proposed_public_profile: /atlas/geografia/argon/

  - id: KETTKE.GEO.KALAM
    name: "Kalam"
    type: HISTORICAL_TERRITORY
    evidence: TEXT
    temporal_context: BOTH
    context: "Former kingdom whose name is also associated with a desert."
    identity_note: "The former kingdom and the desert may require separate geographic records."
    proposed_public_profile: /atlas/geografia/kalam/

  - id: KETTKE.GEO.ORDOKA
    name: "Órdoka"
    type: TERRITORY
    evidence: MAP
    temporal_context: BOTH
    context: "Mapped territory associated in historical accounts with the Bábagos."
    proposed_public_profile: /atlas/geografia/ordoka/

  - id: KETTKE.GEO.VERVEKA
    name: "Vérveka"
    map_name: "Reino de Vérveka"
    type: KINGDOM
    evidence: BOTH
    temporal_context: BOTH
    context: "Kingdom associated with Terian and the history of Kettke."
    proposed_public_profile: /atlas/geografia/verveka/

  - id: KETTKE.GEO.BELONIA
    name: "Belonia"
    type: TERRITORY
    evidence: BOTH
    temporal_context: PRESENT
    context: "Mapped location associated with trade and maritime geography."
    proposed_public_profile: /atlas/geografia/belonia/

  - id: KETTKE.GEO.DORIA
    name: "Doria"
    type: TERRITORY
    evidence: BOTH
    temporal_context: PRESENT
    context: "Mapped location associated with the commercial geography of Kett Vurk."
    proposed_public_profile: /atlas/geografia/doria/

  - id: KETTKE.GEO.BOSQUE_OSCURO
    name: "Bosque Oscuro"
    type: FOREST
    evidence: BOTH
    temporal_context: PRESENT
    context: "Named forest represented on the published map."
    proposed_public_profile: /atlas/geografia/bosque-oscuro/

  - id: KETTKE.GEO.TOVER
    name: "Tover"
    alternate_names:
      - "Isla de las Rocas"
    type: ISLAND
    evidence: BOTH
    temporal_context: PRESENT
    context: "Island identified by the names Tover and Isla de las Rocas."
    proposed_public_profile: /atlas/geografia/tover/

  - id: KETTKE.GEO.KINORIA
    name: "Kinoria"
    type: PALACE
    evidence: TEXT
    temporal_context: BOTH
    context: "Palace carved into the rock of Ikettar."
    proposed_public_profile: /atlas/geografia/kinoria/

  - id: KETTKE.GEO.KEMORAS
    name: "Kémoras"
    type: PALACE
    evidence: TEXT
    temporal_context: BOTH
    context: "Palace associated with Ákador."
    proposed_public_profile: /atlas/geografia/kemoras/

  - id: KETTKE.GEO.KALAMNIA
    name: "Kalamnia"
    type: PALACE
    evidence: TEXT
    temporal_context: PRESENT
    context: "Palace of Yrandia, named in memory of Kalam."
    proposed_public_profile: /atlas/geografia/kalamnia/

  - id: KETTKE.GEO.BETTNUK
    name: "Bettnuk"
    type: SETTLEMENT
    evidence: TEXT
    temporal_context: PRESENT
    context: "Settlement associated with the Antraka narrative."
    proposed_public_profile: /atlas/geografia/bettnuk/

  - id: KETTKE.GEO.BAKALIA
    name: "Bakalia"
    type: SETTLEMENT
    evidence: TEXT
    temporal_context: BOTH
    context: "Former capital of Antraka, situated on the western slope of Ultur."
    proposed_public_profile: /atlas/geografia/bakalia/

  - id: KETTKE.GEO.MAR_DULCE
    name: "Mar Dulce"
    type: LAKE
    evidence: TEXT
    temporal_context: PRESENT
    context: "Named freshwater body distinguished in the narrative from Imurum."
    proposed_public_profile: /atlas/geografia/mar-dulce/

  - id: KETTKE.GEO.BRADIA
    name: "Bradia"
    type: TERRITORY
    evidence: BOTH
    temporal_context: BOTH
    context: "Mapped location whose name is also associated with a mountain."
    identity_note: "Bradia and the mountain of Bradia must not automatically be treated as one entity."
    proposed_public_profile: /atlas/geografia/bradia/

  - id: KETTKE.GEO.KAZUM_CLIFFS
    name: "Acantilados de Kazum"
    type: CLIFFS
    evidence: TEXT
    temporal_context: PAST
    context: "Cliffs mentioned in historical accounts near the mountain of Bradia."
    proposed_public_profile: /atlas/geografia/acantilados-de-kazum/
```

The proposed public profile paths are reserved identifiers. They do not establish that the corresponding pages already exist.

## 5. Complete published-map inventory

All 26 names below refer to distinct places, as confirmed by the author.

The geographic positions are approximate and must be interpreted using the canonical map orientation.

```yaml
published_map:
  map_id: KETTKE.MAP.KETT_VURK
  map_name: "Kett Vurk"
  map_description: "The Known Land"
  place_count: 26
  orientation:
    north: TOP
    east: LEFT
    south: BOTTOM
    west: RIGHT

  places:
    - name: "Órdoka"
      id: KETTKE.GEO.ORDOKA
      editorial_class: PRIMARY
      map_zone: UPPER_LEFT

    - name: "Dresia"
      id: KETTKE.GEO.DRESIA
      editorial_class: SECONDARY
      map_zone: NORTHERN

    - name: "Yvura"
      id: KETTKE.GEO.YVURA
      editorial_class: SECONDARY
      map_zone: NORTHERN

    - name: "Keria"
      id: KETTKE.GEO.KERIA
      editorial_class: SECONDARY
      map_zone: UPPER_LEFT

    - name: "Reino de Ýmala"
      id: KETTKE.GEO.YMALA
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: CENTRAL_LEFT

    - name: "Reino de Bógotra"
      id: KETTKE.GEO.BOGOTRA
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: UPPER_CENTRAL

    - name: "Belonia"
      id: KETTKE.GEO.BELONIA
      editorial_class: PRIMARY
      map_zone: CENTRAL_LEFT

    - name: "Bosque Oscuro"
      id: KETTKE.GEO.BOSQUE_OSCURO
      editorial_class: PRIMARY
      type: FOREST
      map_zone: CENTRAL_LEFT

    - name: "Reino de Rilavia"
      id: KETTKE.GEO.RILAVIA
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: UPPER_CENTRAL

    - name: "Tover"
      id: KETTKE.GEO.TOVER
      editorial_class: PRIMARY
      type: ISLAND
      map_zone: CENTRAL_LEFT

    - name: "Reino de Ákador"
      id: KETTKE.GEO.AKADOR
      editorial_class: PRIMARY
      type: KINGDOM
      map_zone: LOWER_LEFT

    - name: "Reino de Íkore"
      id: KETTKE.GEO.IKORE
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: LOWER_LEFT

    - name: "Kettke"
      id: KETTKE.GEO.KETTKE
      editorial_class: PRIMARY
      map_zone: UPPER_CENTRAL

    - name: "Doria"
      id: KETTKE.GEO.DORIA
      editorial_class: PRIMARY
      map_zone: LOWER_CENTRAL

    - name: "Reino de Antraka"
      id: KETTKE.GEO.ANTRAKA
      editorial_class: PRIMARY
      type: KINGDOM
      map_zone: LOWER_CENTRAL_LEFT

    - name: "Bradia"
      id: KETTKE.GEO.BRADIA
      editorial_class: PRIMARY
      map_zone: SOUTHERN

    - name: "Reino de Térmida"
      id: KETTKE.GEO.TERMIDA
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: UPPER_RIGHT

    - name: "Fintra"
      id: KETTKE.GEO.FINTRA
      editorial_class: SECONDARY
      map_zone: UPPER_CENTRAL_RIGHT

    - name: "Kúroda"
      id: KETTKE.GEO.KURODA
      editorial_class: SECONDARY
      map_zone: UPPER_CENTRAL_RIGHT

    - name: "Sonora"
      id: KETTKE.GEO.SONORA
      editorial_class: SECONDARY
      map_zone: CENTRAL_RIGHT

    - name: "Reino de Darabia"
      id: KETTKE.GEO.DARABIA
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: LOWER_RIGHT

    - name: "Reino de Sudum"
      id: KETTKE.GEO.SUDUM
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: SOUTHERN

    - name: "Reino de Vérveka"
      id: KETTKE.GEO.VERVEKA
      editorial_class: PRIMARY
      type: KINGDOM
      map_zone: LOWER_RIGHT

    - name: "Drókola"
      id: KETTKE.GEO.DROKOLA
      editorial_class: SECONDARY
      map_zone: LOWER_RIGHT

    - name: "Nurukia"
      id: KETTKE.GEO.NURUKIA
      editorial_class: SECONDARY
      map_zone: RIGHT_EDGE

    - name: "Reino de Zórmolas"
      id: KETTKE.GEO.ZORMOLAS
      editorial_class: SECONDARY
      type: KINGDOM
      map_zone: UPPER_RIGHT
```

Map zones describe visual regions of the original illustration, not precise coordinates.

## 6. Additional narrative geography

The following locations have been identified through the narrative analysis and are not part of the 26-name map inventory.

This section also includes more specific locations whose names are related to mapped territories.

```yaml
narrative_geography:
  - id: KETTKE.GEO.ARGON
    name: "Argon"
    editorial_class: PRIMARY
    type: TERRITORY
    context: "Territory associated with the Mibuks and Hanna's route toward Yrandia."

  - id: KETTKE.GEO.YRANDIA
    name: "Yrandia"
    editorial_class: PRIMARY
    type: KINGDOM
    context: "Hidden kingdom reached during the narrative."

  - id: KETTKE.GEO.KALAM
    name: "Kalam"
    editorial_class: PRIMARY
    type: HISTORICAL_TERRITORY
    context: "Former kingdom associated with a desert and historical memory."

  - id: KETTKE.GEO.KALAM_DESERT
    name: "Desierto de Kalam"
    editorial_class: SECONDARY
    type: DESERT
    context: "Desert associated with the former kingdom of Kalam."
    identity_status: SEPARATE_FEATURE_PENDING_VERIFICATION

  - id: KETTKE.GEO.BETTNUK
    name: "Bettnuk"
    editorial_class: PRIMARY
    type: SETTLEMENT
    context: "Settlement associated with Antraka."

  - id: KETTKE.GEO.BAKALIA
    name: "Bakalia"
    editorial_class: PRIMARY
    type: SETTLEMENT
    context: "Former capital of Antraka."

  - id: KETTKE.GEO.KINORIA
    name: "Kinoria"
    editorial_class: PRIMARY
    type: PALACE
    context: "Palace carved into the rock of Ikettar."

  - id: KETTKE.GEO.KEMORAS
    name: "Kémoras"
    editorial_class: PRIMARY
    type: PALACE
    context: "Palace associated with Ákador."

  - id: KETTKE.GEO.KALAMNIA
    name: "Kalamnia"
    editorial_class: PRIMARY
    type: PALACE
    context: "Palace of Yrandia."

  - id: KETTKE.GEO.MAR_DULCE
    name: "Mar Dulce"
    editorial_class: PRIMARY
    type: LAKE
    context: "Named body of water distinct from Imurum."

  - id: KETTKE.GEO.KAZUM_CLIFFS
    name: "Acantilados de Kazum"
    editorial_class: PRIMARY
    type: CLIFFS
    context: "Cliffs associated with the mountain of Bradia."

  - id: KETTKE.GEO.BRADIA_MOUNTAIN
    name: "Montaña de Bradia"
    editorial_class: SECONDARY
    type: MOUNTAIN
    context: "Mountain described above the cliffs of Kazum."
    identity_status: DISTINCT_FEATURE_PENDING_VERIFICATION

  - id: KETTKE.GEO.IMURUM
    name: "Imurum"
    editorial_class: SECONDARY
    type: LAKE
    context: "Named lagoon distinguished from Mar Dulce."

  - id: KETTKE.GEO.ULTUR
    name: "Ultur"
    editorial_class: SECONDARY
    type: MOUNTAIN_RANGE
    context: "Mountain range associated with Antraka and Bakalia."

  - id: KETTKE.GEO.ISUROM
    name: "Isurom"
    editorial_class: SECONDARY
    type: MOUNTAIN
    context: "Mountain associated with Ákador."

  - id: KETTKE.GEO.IKETTAR
    name: "Ikettar"
    editorial_class: SECONDARY
    type: MOUNTAIN
    context: "Rock formation associated with the palace of Kinoria."
    exact_geographic_type: PENDING_VERIFICATION

  - id: KETTKE.GEO.ISSUK
    name: "Issuk"
    editorial_class: SECONDARY
    type: VOLCANO
    context: "Volcano associated with Órdoka."

  - id: KETTKE.GEO.FARAS
    name: "Faras"
    editorial_class: SECONDARY
    type: LAKE
    context: "Lake associated with the geography of Kettke."

  - id: KETTKE.GEO.LIVOKA
    name: "Lívoka"
    editorial_class: SECONDARY
    type: UNRESOLVED
    context: "Named location in the narrative."
    classification_status: PENDING_VERIFICATION

  - id: KETTKE.GEO.FADIAS
    name: "Fadias"
    editorial_class: SECONDARY
    type: MARSH
    context: "Marshland identified in the narrative."

  - id: KETTKE.GEO.MAR_BELONIA
    name: "Mar de Belonia"
    editorial_class: SECONDARY
    type: SEA
    context: "Maritime area associated with Belonia."

  - id: KETTKE.GEO.EDORAK
    name: "Édorak"
    editorial_class: SECONDARY
    type: TERRITORY
    context: "Location associated with the Antraka geographic context."
    classification_status: PENDING_VERIFICATION

  - id: KETTKE.GEO.DROKOLAS
    name: "Drokolas"
    editorial_class: SECONDARY
    type: HISTORICAL_TERRITORY
    context: "Historical location whose possible relationship with Drókola requires verification."
    identity_status: UNRESOLVED

  - id: KETTKE.GEO.REINOS_AISLADOS
    name: "Reinos Aislados"
    editorial_class: SECONDARY
    type: COLLECTIVE_REGION
    context: "Collective designation appearing in historical accounts."
    identity_status: COLLECTIVE_NOT_SINGLE_KINGDOM
```

## 7. Geographic relationships

Relationships are recorded separately from the geographic entities themselves.

Only supported relationships may be promoted to confirmed canon.

```yaml
relationships:
  - subject: KETTKE.GEO.KINORIA
    predicate: CARVED_IN
    object: KETTKE.GEO.IKETTAR
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.KEMORAS
    predicate: ASSOCIATED_WITH
    object: KETTKE.GEO.AKADOR
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.KALAMNIA
    predicate: LOCATED_IN
    object: KETTKE.GEO.YRANDIA
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.KALAMNIA
    predicate: NAMED_IN_MEMORY_OF
    object: KETTKE.GEO.KALAM
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.BAKALIA
    predicate: FORMER_CAPITAL_OF
    object: KETTKE.GEO.ANTRAKA
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.BAKALIA
    predicate: LOCATED_ON_WESTERN_SLOPE_OF
    object: KETTKE.GEO.ULTUR
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.KAZUM_CLIFFS
    predicate: GEOGRAPHICALLY_ASSOCIATED_WITH
    object: KETTKE.GEO.BRADIA_MOUNTAIN
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.MAR_DULCE
    predicate: DISTINCT_FROM
    object: KETTKE.GEO.IMURUM
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.ARGON
    predicate: ON_ROUTE_TOWARD
    object: KETTKE.GEO.YRANDIA
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.ISSUK
    predicate: ASSOCIATED_WITH
    object: KETTKE.GEO.ORDOKA
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.MAR_BELONIA
    predicate: ASSOCIATED_WITH
    object: KETTKE.GEO.BELONIA
    epistemic_status: SUPPORTED

  - subject: KETTKE.GEO.DROKOLAS
    predicate: POSSIBLY_RELATED_TO
    object: KETTKE.GEO.DROKOLA
    epistemic_status: UNRESOLVED
```

The relationships above are a preliminary semantic registry. Passage-level evidence identifiers must be added before a complete source audit can be declared.

## 8. Historical geography

Geographic identity must be preserved across historical periods.

A location may:

- Change its political status.
- Become abandoned or destroyed.
- Change its name.
- Be remembered through another location's name.
- Exist in a historical account without being visited by Hanna.
- Have different physical and political meanings in different periods.

```yaml
historical_geography_rules:
  - "Never assume that a historical kingdom still exists in the same form."
  - "Never infer that a present-day location has the same borders as its historical predecessor."
  - "Keep former capitals distinct from current capitals."
  - "Represent renamed locations through documented identity relationships."
  - "Separate a territory from a natural feature when the source establishes distinct entities."
  - "Do not invent historical dates or chronological sequences."
  - "Do not treat legends as independently verified events."
```

Known historical relationships requiring particular attention:

```yaml
historical_cases:
  - subject: "Kalam"
    issue: "Former kingdom and desert geography."
    status: REQUIRES_ENTITY_LEVEL_REVIEW

  - subject: "Vérveka"
    historical_designation: "Nuevo Kettke"
    status: REQUIRES_CONTEXTUAL_VERIFICATION

  - subject: "Bakalia"
    historical_role: "Former capital of Antraka."
    status: SUPPORTED

  - subject: "Drókola / Drokolas"
    issue: "Possible connection between mapped and historical names."
    status: UNRESOLVED

  - subject: "Bradia / Montaña de Bradia"
    issue: "Shared geographic name with potentially distinct referents."
    status: REQUIRES_ENTITY_LEVEL_REVIEW
```

## 9. Earth geography

Volume I also includes locations on Earth.

These must remain distinct from Kett Vurk.

```yaml
earth_geography:
  - id: KETTKE.GEO.EARTH.NORTH_PARK
    name: "North Park"
    editorial_class: SECONDARY
    world: EARTH
    type: REGION
    context: "Park associated with the passage between Earth and Kettke."
    exact_geographic_type: PENDING_VERIFICATION

  - id: KETTKE.GEO.EARTH.METROPOLITAN_MUSEUM
    name: "Museo Metropolitano"
    editorial_class: SECONDARY
    world: EARTH
    type: BUILDING
    context: "Museum associated with the discovery in the opening narrative."

  - id: KETTKE.GEO.EARTH.ST_JAMES
    name: "St. James"
    editorial_class: SECONDARY
    world: EARTH
    type: UNRESOLVED
    context: "Named location associated with Hanna's life on Earth."
    exact_identity: PENDING_VERIFICATION
```

Earth geography and Kett Vurk geography must not be merged into a single political or cartographic hierarchy.

## 10. Chapter and source evidence

Geographic mentions must eventually be linked to exact passages of the Spanish source.

```yaml
source_evidence_contract:
  source_priority:
    - AUTHOR_CONFIRMED
    - PUBLISHED_ORIGINAL_MAP
    - PUBLISHED_SPANISH_NOVEL

  chapter_identifiers:
    opening: OPENING
    numbered_chapters: C01-C22

  geographic_appearance_types:
    - PHYSICAL_VISIT
    - DIRECT_OBSERVATION
    - DIALOGUE_REFERENCE
    - HISTORICAL_ACCOUNT
    - LEGENDARY_ACCOUNT
    - MAP_ONLY

  required_fields_for_verified_mentions:
    - place_id
    - source_id
    - chapter_id
    - appearance_type
    - evidence_location
    - epistemic_status

  restrictions:
    - "Do not invent chapter numbers."
    - "Do not interpret every name occurrence as a physical visit."
    - "Do not confuse narrated history with present action."
    - "Do not derive exact coordinates from the illustration."
    - "Do not assume that every geographic name is represented on the map."
```

The current registry records identified geographic entities and preliminary relationships.

A complete chapter-by-chapter geographic evidence index remains pending.

## 11. Public Atlas publication model

```yaml
public_atlas:
  index: /atlas/geografia/

  primary:
    publication_model: INDIVIDUAL_PROFILE
    count: 20
    status: PROPOSED

  secondary:
    publication_model: GENERAL_INDEX_ENTRY
    status: PROPOSED

  rules:
    - "Every geographic entity must appear in the general geographic index."
    - "Primary entities may additionally have dedicated pages."
    - "Secondary entities must remain independently identifiable."
    - "A secondary entity may become primary without changing its canonical ID."
    - "Public profiles must not expose unpublished future-volume information."
    - "Do not assert that proposed profile URLs already exist."
```

## 12. Cross-domain integration

The geography registry must support links to:

```yaml
cross_domain_links:
  characters: KETTKE.ATLAS.CHARACTERS
  history: KETTKE.ATLAS.HISTORY
  peoples_and_cultures: KETTKE.ATLAS.PEOPLES
  bestiary: KETTKE.ATLAS.BESTIARY
  language: KETTKE.ATLAS.LANGUAGE
  narrative_map: KETTKE.NARRATIVE_MAP.VOL_1
```

Examples of relationships to represent after source verification:

- Characters who live in or govern a territory.
- Peoples associated with particular kingdoms.
- Creatures inhabiting geographic regions.
- Historical events occurring at named locations.
- Routes followed by Hanna.
- Geographic names derived from historical events.
- Settlements located within larger territories.
- Changes in political control across time.

Co-occurrence in the same chapter does not establish a geographic relationship.

## 13. Epistemic status and pending audit

```yaml
epistemic_status:
  map_toponym_inventory:
    status: AUTHOR_CONFIRMED
    count: 26
    distinct_entities: true

  map_orientation:
    status: AUTHOR_CONFIRMED

  primary_geography_selection:
    status: AUTHOR_APPROVED
    count: 20

  map_position_descriptions:
    status: APPROXIMATE

  narrative_geography_inventory:
    status: PROVISIONAL
    completeness: NOT_CERTIFIED

  geographic_relationships:
    status: PRELIMINARY
    passage_level_evidence: PENDING

  chapter_appearance_index:
    status: PENDING

  political_borders:
    status: NOT_ESTABLISHED

  exact_distances:
    status: NOT_ESTABLISHED
```

### Pending work

1. Complete an exhaustive chapter-by-chapter extraction of geographic names.
2. Verify spelling and identity against the original Spanish text.
3. Distinguish kingdoms from cities, regions, buildings, and natural features.
4. Resolve the geographic identity of Kalam and its desert.
5. Resolve the relationship between Bradia and the mountain of Bradia.
6. Verify the relationship between Drókola and Drokolas.
7. Verify the historical use of Nuevo Kettke for Vérveka.
8. Add chapter references and passage-level evidence.
9. Identify additional unnamed but narratively significant locations.
10. Validate all proposed public profile URLs.
11. Link places to characters, peoples, history, and bestiary entries.

## 14. Canon preservation rules

The following rules are mandatory:

- Preserve all 26 published map names.
- Preserve the author's unconventional east-west map orientation.
- Include locations appearing only in the novel.
- Include locations appearing only on the map.
- Maintain one stable identity per distinct geographic entity.
- Never merge different places merely because they share a name.
- Never invent geographic coordinates, borders, or distances.
- Preserve historical geography separately from contemporary geography.
- Do not convert a historical account into a verified present-day fact.
- Keep editorial importance separate from geographic type.
- Do not introduce spoilers from unpublished volumes.
- Maintain original canonical proper names in English documentation.
- Prefer explicit uncertainty to unsupported geographic assertions.

---

**Registry status:** Provisional geographic inventory with author-approved primary classification.

**Canonical scope:** Published Volume I, including its original map.

**Next validation stage:** Exhaustive chapter-level geographic evidence and cross-domain relationships.
