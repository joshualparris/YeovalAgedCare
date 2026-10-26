# UPA Aged Care Home Design — Evidence-Based Research Findings

**Research performed:** 26 October 2026  
**Scope:** UPA design principles and documented Yeoval features. This complements `docs/YEOVAL_ARCHITECTURE_EVIDENCE.md`, `docs/RESEARCH_EXECUTION_2026-10-26.md`, and `docs/UPA_YEOVAL_BUILDING_DESIGN_AND_GAMEPLAY_RESEARCH_2026-10-26.md`.

## Executive findings

**1. Yeoval has a documented two-building connection.** A historical firsthand account from a Yeoval care manager explicitly states that renovations joined two formerly separate buildings, demolished and replaced some rooms, and completely rebuilt the dining room. This is direct evidence that the smaller building should not be modelled as an inaccessible isolated block. The actual route, door positions and current condition are still unverified.  
Source: https://www.qpsbenchmarking.com/news/upa-yeoval-gaining-a-competitive-advantage-by-increasing-resident-satisfaction/  
Related primary evidence: https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2012.pdf and https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2016.pdf

**2. Current UPA Yeoval marketing confirms a homelike, mixed-room residential service.** UPA describes both single and shared/double bedrooms, each with ensuite bathroom and emergency-call system, 24-hour support, communal dining, dementia-specific care, co-located home care and community health centre, allied health access and social activities. These facts support room programme and props, **not** precise positions or counts.  
Source: https://www.upa.org.au/locations/dubbo/yeoval-aged-care/

**3. Historic service boundaries should not be mistaken for physical wings.** A 2015/2016-era accreditation report states that the co-located nursing home and hostel were managed as one entity, shared management systems and provided residents access to communal areas, services and activities. That is important for plausible connected interior circulation but is not an as-built plan.  
Source: https://www.agedcarequality.gov.au/sites/default/files/legacy-files/aacqa/files/11/mnt/www-aacqa/publications/reports/YeovalCommunityNursingHome5.pdf

**4. UPA's 2019 western-wing project was a proposal, not confirmed completion.** The provider's regional newsletter proposed reopening Netherwood western wing, expanding dining, and adding six beds and a functional kitchen/lounge area. It also described rear-garden turfing, wheelchair access to a bus, community GP practice rooms and the Acacia Room used for community gatherings. These are valuable historical features but should be labelled as of 2019; do not silently represent all proposed construction as existing in 2026.  
Source: https://www.upa.org.au/wp-content/uploads/2019/04/Western-Region-Mail-April-May-2019.pdf

**5. The historical care model prioritised domestic dining and community participation.** A Yeoval care manager described on-site seasonal meal preparation, family/community lunches, walking groups, school/church activities, community visitors, volunteers and a weekly pain clinic. A realistic model needs social rooms, visitors and a visible dining service, not merely repetitive bedrooms and corridors. This source is historical, not a verified 2026 timetable.  
Source: https://www.qpsbenchmarking.com/news/upa-yeoval-gaining-a-competitive-advantage-by-increasing-resident-satisfaction/

## National evidence-based design framework

The Australian Government's **National Aged Care Design Principles and Guidelines** identifies four linked principles:

| Principle | Design implication for UPA/Yeoval 3D simulation |
|---|---|
| Enable the Person | Provide legible circulation, accessible seating, usable bedrooms and ensuite, assistive supports, low-glare lighting, meaningful choice and orientation cues |
| Cultivate a Home | Domestic-scale lounges, familiar materials, personalisation, privacy, acoustic separation, distinct social and quiet zones |
| Access the Outdoors | Visible daylight, comfortable and accessible paths, garden seating, shade, raised planting beds, safe links between internal and outdoor spaces |
| Connect with Community | Welcoming visitor entry, communal meals, flexible activity room, co-located community health access, community-facing activities |

The guidelines are flexible design guidance, not a substitute for the NCC, Australian Standards, site-specific building approval or fire-safety certification. They explicitly recognise diversity, workforce needs, infection prevention, environmental sustainability and enabling technology.  
Source: https://www.health.gov.au/sites/default/files/2024-08/national-aged-care-design-principles-and-guidelines_0.pdf  
Context: https://www.health.gov.au/our-work/improving-accommodation-in-residential-aged-care

The **strengthened Aged Care Quality Standards** commenced **1 November 2025**. Particularly relevant to the built environment are Standard 4 (Environment), Standard 6 (Food and nutrition) and Standard 7 (Residential community). Other standards cover individual rights, governance, care and clinical quality. A digital reconstruction should reflect the spirit of these outcomes without claiming the actual facility meets every criterion.  
Sources: https://www.agedcarequality.gov.au/providers/quality-standards and https://www.agedcarequality.gov.au/older-australians/your-rights/aged-care-quality-standards

## Practical, room-by-room implementation priorities

| Priority | Feature | Evidence tier | Proposed treatment |
|---|---|---|---|
| P0 | Two physically connected buildings | B | Model continuous sheltered link and passable thresholds; geometry marked illustrative |
| P0 | Accessible route into second wing | B/C | Collision-free traversable route from public entrance; test on mobile and desktop |
| P0 | Single and shared ensuite bedrooms | B | Include both types; do not assign a fictional exact room count |
| P1 | Communal dining | B | Real dining tables, chairs, food service circulation and on-site meal scene |
| P1 | Domestic lounges and activity spaces | B | Distinct furnished social spaces, non-institutional materials |
| P1 | Kitchen | B | Separate cooking/preparation and serving zones; do not imply public access to staff-only areas |
| P1 | Outdoor garden and seating | B | Turf, raised beds, shade and a reachable outdoor sitting area |
| P1 | Co-located home care/community health | B | Separate signposted functions; exact entrance placement unknown |
| P2 | Acacia community room | B (historic 2019) | Illustrative community-use room with provenance label |
| P2 | Netherwood western wing expansion | B for proposal, D for completion | Represent as historically proposed until construction verified |
| P2 | Dementia-friendly wayfinding | C | Contrasting room identities, landmarks, clear signage and uncluttered circulation |
| P2 | Staff support / clinical storage | C | Plausible spaces but avoid presenting invented exact operational layouts |

**Evidence tiers:** A = surveyed drawing/verified measurement; B = primary provider or regulator description; C = standards-supported general design inference; D = unverified artistic assumption.

## Specific QA and visual realism audit

The screenshot shows preview version `e935bb0`, with a brick side elevation, two windows and no apparent door on the smaller building. It proves only that **the photographed side lacks a visible door**. It does not establish whether the structure has a door on its other elevations. The 3D model must:
1. Inspect every exterior elevation and actual placement of door meshes.
2. Ensure both wings have a physically walkable connection, consistent with historical documentation.
3. Match front door visuals with collision apertures, door interaction triggers and interior spawn.
4. Test the route entrance → foyer → covered link → second wing → return to entry.
5. Verify the game returns the player to the same real-world-facing entrance, not through a rear wall.
6. Keep uncertain entrance positions labelled as illustrative, not surveyed.
7. Validate mobile touch controls, visibility, lighting and camera collision.

## Research gaps and next verification work

- Obtain historical renovation drawings or site plan held by UPA or Cabonne Council; request only with the user's explicit permission for any outreach.
- Find current photographs of every building elevation and covered connector.
- Establish which structure is Hazelholme, the former nursing home, the named Netherwood wing and the Acacia/MAC spaces.
- Confirm 2026 Netherwood status, current room mix, total places and community-health entry.
- Obtain measured building footprints from legitimate published survey/plan sources, not inferred cadastral boundaries.
- Review exact NCC Class 9c, accessibility, fire, infection control and WHS applicability with primary regulatory texts and qualified practitioners before claiming compliance.
- Cross-reference the prior repository's NSW Spatial Services parcel geometry, which is **land geometry, not a roof plan**.

## Source register

1. UPA current Yeoval page: https://www.upa.org.au/locations/dubbo/yeoval-aged-care/
2. UPA 2019 regional newsletter: https://www.upa.org.au/wp-content/uploads/2019/04/Western-Region-Mail-April-May-2019.pdf
3. UPA 2012 annual report: https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2012.pdf
4. UPA 2016 annual report: https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2016.pdf
5. Yeoval care-manager account: https://www.qpsbenchmarking.com/news/upa-yeoval-gaining-a-competitive-advantage-by-increasing-resident-satisfaction/
6. Yeoval regulator historic audit: https://www.agedcarequality.gov.au/sites/default/files/legacy-files/aacqa/files/11/mnt/www-aacqa/publications/reports/YeovalCommunityNursingHome5.pdf
7. Yeoval regulator service page: https://www.agedcarequality.gov.au/services/yeoval-community-nursing-home
8. National design principles: https://www.health.gov.au/sites/default/files/2024-08/national-aged-care-design-principles-and-guidelines_0.pdf
9. Design principles program: https://www.health.gov.au/our-work/improving-accommodation-in-residential-aged-care
10. Strengthened standards: https://www.agedcarequality.gov.au/providers/quality-standards

**Limitations:** This research synthesises public sources and existing repository findings. It does not establish surveyed door locations, precise room adjacency, current clinical workflows, code certification or full UPA portfolio architectural patterns. No outreach or emails were sent.
