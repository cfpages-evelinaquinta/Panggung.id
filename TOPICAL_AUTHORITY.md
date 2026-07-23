# Topical Authority — panggung.id

## Role and boundary

`panggung.id` should become an Indonesian reference for planning, designing, procuring, building, inspecting, operating, and retiring temporary or permanent stages. Its core reader paths are event owners, venue managers, production managers, designers, structural engineers, stage and rigging contractors, safety personnel, technicians, and buyers.

The knowledge layer must explain decisions and risks without publishing generic capacities, ballast weights, wind cut-offs, rigging loads, crowd capacities, or structural details that could be misapplied. Project-specific structural, geotechnical, electrical, fire, accessibility, lifting, and emergency decisions require current local rules, manufacturer data, site evidence, and review by qualified people.

Neutral articles live under the planned `/artikel/<slug>/` namespace. Commercial intent remains owned by `/panggung/`, `/sewa/`, and the existing equipment routes. The article catalog may link to those routes only when the reader has reached a legitimate procurement decision.

## Evidence audited

Audit date: 2026-07-23. Repository: `cfpages-evelinaquinta/Panggung.id`, branch `main`, static WordPress export.

| Evidence | Observed count/state | Editorial implication |
|---|---:|---|
| `sitemap-complete.xml` | 5,321 unique routes | Best inventory of generated static routes, including archives and pagination. |
| WordPress post sitemaps | 4,395 post URLs across 22 files | Posts are overwhelmingly location-swapped rental pages, not independent educational articles. |
| WordPress page sitemap | 30 page URLs | Contains the homepage, commercial hubs, equipment subpages, About, and Contact. |
| Location-swapped service routes in complete sitemap | 4,409 | Nine repeated families: panggung 489, sound system 490, lighting 492, screen 490, set/backdrop 488, special effect 489, safety 490, mechanical 490, documentation 491. |
| Category/archive routes | 441 | Nine category roots plus 432 paginated category URLs; each category has 49 generated index pages. |
| `/berita` archive routes | 440 | One root plus 439 pagination routes; no separate evidence-rich editorial article namespace was observed. |
| Other/core routes | 31 | Thirty sitemap pages plus `/404`; the latter should not be in a sitemap. |
| Sitemap disagreement | 2 URLs | `/sewa-special-effect-jayawijaya` and `/sewa-special-effect-tarakan` occur in post sitemaps but not `sitemap-complete.xml`. |
| Existing topical-authority artifacts | none | Stable topic and article IDs can start with `PGG-`. |

Representative page inspection found commercial titles and headings for stage, sound, lighting, screen, backdrop, safety, mechanics, documentation, and special effects. Sample city pages shared the same rental-page structure with the place name substituted. The `safety-equipment` meta description still contains the placeholder `[Lokasi]`, an observable template-quality warning.

## Existing coverage and risks

| Existing URL/pattern | Observed role/problem | Decision | Destination/owner | Verification needed |
|---|---|---|---|---|
| `/panggung/` | Main stage-rental commercial hub | expand | `/panggung/` | Add real service scope, project evidence, qualified-review limits, and links to the most relevant neutral guides. |
| `/sewa/` | Cross-category rental directory | keep | `/sewa/` | Confirm every listed service is actually deliverable and remove unsupported claims. |
| `/sewa-panggung-*` | 489 location-swapped stage pages in the complete sitemap | manual review | `/panggung/` plus any genuinely substantiated local landing pages | Before consolidation, inspect GSC, backlinks, leads, local crews, stock, addresses, travel coverage, and unique project evidence. Do not mass-redirect blindly. |
| Eight other `/sewa-<service>-<place>` families | Roughly 3,920 more location-swapped pages | manual review | Corresponding commercial hub | Retain only pages with materially local service evidence; merge, noindex, or redirect the rest after URL-level performance review. |
| `/category/<service>/` | Nine taxonomic archives with little independent value | canonicalize | Corresponding service hub | Confirm whether users need these indexes; avoid competing with commercial hubs. |
| `/category/<service>/page/*` | 432 paginated category archives | noindex | Category root or service hub | Keep crawl links only where useful; verify canonical and pagination behavior before release. |
| `/berita/` | Archive name implies editorial coverage but currently aggregates service posts | expand | `/berita/` or a new `/artikel/` index | Decide final knowledge-index route before publishing the first cluster. |
| `/berita/page/*` | 439 pagination pages dominated by templated posts | noindex | `/berita/` | Review indexation, canonicals, crawl demand, and internal links. |
| `/sound-system/`, `/lighting/`, `/screen/`, `/set-backdrop/`, `/special-effect/`, `/safety-equipment/`, `/mekanik/`, `/dokumentasi/` | Commercial equipment/service hubs, some with broad or placeholder copy | keep | Existing route of the same name | Correct unsupported claims and placeholders; keep deep product selection separate from stage-neutral articles. |
| `/404` | Error document listed in the complete sitemap | remove | none | Confirm the deployed 404 still works after sitemap removal. |
| Two special-effect URLs absent from `sitemap-complete.xml` | Conflicting generated inventories | manual review | Existing canonical route if live and useful | Check filesystem, deployed response, canonical, and sitemap generator. |
| Planned `/artikel/<slug>/` | No current route collision observed | keep | Neutral knowledge layer | Recheck generated routes immediately before implementation. |

Primary risks are index bloat, same-domain competition among near-identical city pages, a commercial rather than educational information architecture, unsupported superlatives, and high-consequence safety topics without visible engineering evidence. Complete planning is not permission to mass-publish thin articles.

## Coverage matrix

| Completeness lens | Topic owner(s) | Status and notes |
|---|---|---|
| Definition and vocabulary | PGG-01 | Stage, platform, riser, catwalk, grandstand, roof, wing, and backstage terms get one glossary path. |
| Taxonomy and variants | PGG-01, PGG-02, PGG-04 | Temporary/permanent, indoor/outdoor, modular/custom, and event configurations are distinguished by use and system. |
| Anatomy and components | PGG-01, PGG-04, PGG-08, PGG-09 | Deck, frame, bracing, roof, rigging, stairs, ramps, edges, and interfaces have owners. |
| Materials and properties | PGG-04, PGG-09, PGG-18 | Structural material, deck finish, corrosion, wear, storage, and repair decisions are covered. |
| Mechanisms and science | PGG-05, PGG-06, PGG-07, PGG-08 | Load paths, stability, wind, ground reaction, anchorage, lifting, and suspended loads require sourced diagrams and review. |
| History and evolution | PGG-01 | Covered as an evolution of stage forms and demountable systems, not nostalgia filler. |
| Measurement and terminology | PGG-02, PGG-05, PGG-06, PGG-07 | Dimensions, sightlines, loads, movement, weather inputs, and ground observations are explained without invented limits. |
| Need recognition | PGG-02, PGG-14 | Readers translate event goals into a stage brief and decide rent, buy, custom-build, or reuse. |
| Survey and diagnosis | PGG-03, PGG-07, PGG-18 | Site, ground, venue, utility, damage, and storage evidence precedes advice. |
| Requirements and design | PGG-02, PGG-04, PGG-05, PGG-09, PGG-10 | Function, structure, access, crowd, and system interfaces become traceable requirements. |
| Comparison and selection | PGG-01, PGG-04, PGG-08, PGG-14 | System and vendor comparisons use decision tables rather than price-only rankings. |
| Budget and procurement | PGG-14 | Scope, exclusions, proof, responsibilities, lifecycle cost, and contract risks are explicit. |
| Preparation | PGG-03, PGG-07, PGG-13, PGG-15 | Survey, approvals, design pack, logistics, exclusion zones, and sequencing are prerequisites. |
| Installation/construction | PGG-15 | Erection and dismantling have method, competence, access, lifting, and quality gates. |
| Commissioning/handover | PGG-16 | Pre-opening inspection, integrated checks, defects, acceptance, and records have one owner. |
| Use/operation | PGG-17 | Opening checks, live monitoring, unauthorized change control, communications, and incident response are covered. |
| Inspection and maintenance | PGG-16, PGG-18 | Acceptance inspection is separate from recurring asset care and post-transport damage assessment. |
| Troubleshooting and repair | PGG-06, PGG-07, PGG-17, PGG-18 | Weather, settlement, movement, damage, and operational warning signs lead to stop/quarantine/escalation rules. |
| Upgrade and replacement | PGG-04, PGG-14, PGG-18 | Retrofit, repair, reuse, replacement, and decommissioning decisions use traceability and qualified review. |
| User/stakeholder | PGG-02, PGG-13, PGG-14, PGG-17 | Organiser, venue, designer, engineer, contractor, rigger, electrician, operator, steward, and authority roles are separated. |
| Building/site type | PGG-02, PGG-03 | Indoor halls, outdoor grounds, streets, theatres, sports sites, and permanent venues have distinct constraints. |
| Geography and climate | PGG-03, PGG-06, PGG-07 | Indonesian rain, heat, lightning, flooding, soft ground, coastal corrosion, and local approvals affect substance; city swaps do not. |
| Scale and performance | PGG-02, PGG-05, PGG-08, PGG-10 | Stage scale follows activities, equipment, loads, audience behavior, and evacuation—not a generic size chart. |
| New build versus retrofit | PGG-03, PGG-04, PGG-13 | Permanent additions and temporary installations inside existing venues require different evidence and approvals. |
| DIY versus professional | PGG-05, PGG-08, PGG-11, PGG-13 | Readers get explicit stop conditions for engineering, rigging, lifting, electrical, and regulatory decisions. |
| Quality level | PGG-04, PGG-14, PGG-18 | Economy, standard, specialist, temporary, and long-life choices are compared by evidence and lifecycle, not prestige. |
| Safety and health | PGG-06 through PGG-13, PGG-15 through PGG-17 | Collapse, falls, lifting, electric shock, fire, crowd pressure, slips, weather, noise, and emergency response are central. |
| Failure modes | PGG-05 through PGG-08, PGG-11, PGG-16 through PGG-18 | Warning signs, consequences, controls, and escalation form an FMEA-like path. |
| Standards and regulation | PGG-05, PGG-08, PGG-09, PGG-11 through PGG-13 | Current status is verified; applicability and clauses require local professional confirmation. |
| Environmental impact | PGG-03, PGG-06, PGG-14, PGG-18 | Transport, noise, energy, reusable systems, weather damage, waste, and end-of-life are covered. |
| Evidence quality | all topics | Safety and capacity claims require primary rules/standards, calculations, manufacturer data, inspections, and qualified review. |
| Myths and unsafe advice | PGG-05 through PGG-08, PGG-11, PGG-15, PGG-16 | Rejects generic capacity tables, improvised ballast, mixed systems, uncertified rigging, wet-power shortcuts, and visual-only acceptance. |
| Fundamentals | PGG-01 | Stable beginner reference and glossary. |
| How-to | PGG-02, PGG-03, PGG-13, PGG-15 through PGG-18 | Procedures include prerequisites, stop conditions, and verification. |
| Comparison | PGG-01, PGG-04, PGG-08, PGG-14 | Comparisons map to one buyer decision each. |
| Diagnosis | PGG-06, PGG-07, PGG-11, PGG-17, PGG-18 | Symptom-led pages distinguish observation from specialist diagnosis. |
| Calculation/tool | PGG-02, PGG-05 through PGG-07, PGG-10, PGG-14 | Use input worksheets and checklists; do not provide universal engineering outputs. |
| Visual reference | PGG-01, PGG-04, PGG-05, PGG-08 through PGG-10 | Anatomy, load path, connections, access, cable, barrier, and site-plan diagrams are prioritized. |
| Case study | PGG-03, PGG-06, PGG-15 through PGG-17 | Publish only from real documented projects or incidents; never fabricate experience. |
| FAQ/glossary | PGG-01 | Short questions support the hub rather than becoming thin pages. |
| Commercial support | PGG-14 | Procurement education may link to `/panggung/`; neutral guides do not turn into sales pages. |
| News/trends | PGG-13, PGG-18 | Only material regulatory, system, or lifecycle changes with a maintenance owner deserve updates. |
| Query-modifier stress test | all topics | What/why/how/type/part/material/size/standard/cost/install/inspect/repair/site/climate/stakeholder questions fit an existing brief; no location-only expansion is allowed. |

## Topical map

| Topic ID | Parent topic | Reader outcome | Required subtopics/questions | Evidence/formats | Boundary | Article target |
|---|---|---|---|---|---|---:|
| PGG-01 | Fundamentals, terminology, and stage taxonomy | Identify stage types and parts without confusing a platform, riser, catwalk, roof, grandstand, or complete event-production system. | Definitions; temporary versus permanent; indoor/outdoor; modular/custom/mobile; deck, frame, bracing, roof, wings, backstage; proscenium, thrust, in-the-round; history and lifecycle. | Illustrated glossary; annotated anatomy; classification tree; sourced history. | Does not size a project or select a vendor; PGG-02 owns requirements and PGG-14 owns procurement. | 6 |
| PGG-02 | Event brief, use case, dimensions, and sightlines | Turn program activities, performers, equipment, audience, venue, and changeovers into a reviewable stage brief. | Event types; activity zones; dimensions; clear height; stage elevation; sightlines; performer flow; accessibility; equipment interfaces; schedule and future change scenarios. | Brief template; dimension worksheet; plan/section diagrams; stakeholder interview checklist. | Does not calculate structural capacity or venue safe capacity; PGG-05 owns loads and PGG-10 owns crowds. | 6 |
| PGG-03 | Site survey and feasibility | Collect enough site evidence to decide whether and how a stage concept can proceed. | Indoor/outdoor survey; ground/floor; slopes; drainage; flood history; wind exposure; access; utilities; overhead/underground services; truck/crane paths; emergency and pedestrian separation. | Field checklist; photo register; measured plan; utility map; go/no-go report. | Does not design foundations or erection methods; PGG-07 owns support/anchorage and PGG-15 owns build sequencing. | 6 |
| PGG-04 | Structural systems, materials, decks, and connections | Compare stage systems and recognize interfaces that require manufacturer or engineer control. | Steel/aluminium/timber; proprietary modular systems; scaffolding-derived systems; decks; roof frames; bracing; pins, bolts, clamps; compatibility; corrosion; fatigue; permanent versus demountable detailing. | System matrix; component photos; connection diagrams; manufacturer comparison; engineer review. | Does not assign allowable loads or repair damaged members; PGG-05 owns load verification and PGG-18 owns repair/quarantine. | 6 |
| PGG-05 | Loads, load paths, stability, and structural review | Understand what must enter a project-specific structural assessment and when generic rules are unsafe. | Dead, live, concentrated, moving, dynamic, crowd, equipment, suspended, wind and accidental actions; load paths; stability; deflection; vibration; combinations; load plans; change control; review triggers. | Engineer-reviewed diagrams; input worksheet; calculation narrative; standards register; red-flag checklist. | Never publishes universal capacities, spans, ballast, or member sizes; PGG-07 owns ground/anchorage and PGG-08 owns rigging plans. | 6 |
| PGG-06 | Wind, rain, lightning, heat, and severe-weather decisions | Plan monitoring, stop, evacuation, inspection, and restart decisions for Indonesian weather exposure. | Wind on roofs/screens/backdrops; forecast versus site observation; manufacturer/design operating limits; rain, ponding and slip; lightning; heat; flooding; weather action matrix; post-event inspection. | Weather decision matrix; monitoring log; site-specific trigger template; regulator guidance; engineer/manufacturer review. | Does not invent a wind-speed threshold or override emergency command; PGG-17 owns live operations and PGG-12 owns integrated emergencies. | 6 |
| PGG-07 | Ground support, foundations, ballast, anchors, and settlement | Recognize how loads reach the ground and what evidence is required for stable support. | Ground-bearing evidence; existing floors; base plates and spreaders; anchors; ballast; guy lines; underground services; slope/soft ground; flood/coast conditions; settlement, tilt, and movement monitoring. | Load-path detail; survey checklist; geotechnical/structural review; inspection photos; monitoring log. | Never gives generic ballast or anchor values; PGG-05 owns structural demand and PGG-03 owns initial site evidence. | 6 |
| PGG-08 | Rigging, truss, hoists, suspended loads, and lifting | Define competent-person, equipment, documentation, inspection, and exclusion-zone requirements for overhead systems. | Rigging plot; point loads; truss; towers; hoists; motors; slings; shackles; secondary retention; lifting plan; exclusion zones; inspections/certificates; roof rigging versus ground support. | Rigging plot example; responsibility matrix; equipment register; pre-use checklist; qualified rigger/engineer review. | Does not teach unqualified readers to select hardware or calculate rigging capacity; PGG-11 owns electrical supply to motors and PGG-15 owns build sequence. | 6 |
| PGG-09 | Decks, edges, stairs, ramps, backstage, and accessibility | Design usable circulation and fall protection for performers, crew, and disabled participants. | Deck finish; gaps; slip/trip; edges; guardrails; toe boards; stairs; ramps; handrails; accessible route; backstage/loading access; cable crossings; traps/catwalks. | Plan/section details; accessibility checklist; original photos; user-journey review; applicable-rule register. | Does not determine crowd egress width or structural load capacity; PGG-10 owns crowd movement and PGG-05 owns loading. | 6 |
| PGG-10 | Crowd interface, barriers, venue layout, and egress | Place the stage within a site plan that manages approach, viewing, circulation, surge, emergency access, and dispersal. | Audience profile; sightlines; front-of-stage barriers; standing/seated zones; entrances/exits; queues; pinch points; emergency routes; safe venue capacity; monitoring; accessible evacuation. | Site-plan template; flow diagram; barrier decision table; crowd-risk checklist; authority/competent-person review. | Does not market an attendance number or treat stage capacity as venue capacity; PGG-12 owns emergency command and PGG-02 owns stage dimensions. | 6 |
| PGG-11 | Temporary electrical systems and power coordination | Plan distribution, protection, cable management, inspection, redundancy, and weather controls around a stage. | Utility/generator sources; load schedule; distribution; protection; earthing/bonding; temporary panels; cable routing; wet conditions; inspection/testing; critical PA/lighting power; shutdown. | Single-line concept; load schedule template; cable plan; test record; qualified electrical review. | Does not provide DIY wiring instructions or genset sizing; `/mekanik/genset/` owns rental service and a qualified electrical designer owns project design. | 6 |
| PGG-12 | Fire, special effects, emergency plans, and show-stop control | Integrate fire prevention, effects, alarm, evacuation, command, communications, drills, and restart criteria. | Combustible finishes; hot work; pyrotechnics/flame/fog; extinguishers; alarm; emergency lighting/PA; escape routes; structural/weather/electrical/crowd scenarios; show stop; drills; handover to authorities. | Scenario matrix; emergency plan template; fire-rule register; tabletop exercise; authority and specialist review. | Does not replace local fire/event permits or effect-specialist design; `/special-effect/` owns commercial rental and PGG-17 owns routine show monitoring. | 6 |
| PGG-13 | Design documents, approvals, competence, and responsibility | Assemble a traceable project file and know who must approve, check, build, operate, and accept each element. | Client brief; drawings; calculations; design assumptions; standards register; local permits; venue approvals; competence; RACI; method statements; change control; as-builts; records. | Document index; RACI matrix; approval checklist; change log; current regulatory research. | Does not declare a universal permit list; the relevant local authority, venue, and appointed professionals determine applicability. | 6 |
| PGG-14 | Procurement, rental, vendor evaluation, contracts, and lifecycle cost | Compare offers on complete scope, evidence, responsibilities, risk, and total cost rather than headline price. | Rent/buy/custom/reuse; scope and exclusions; design proof; stock/condition; logistics; crew; tests; insurance; weather/cancellation; damage; warranty; spares; lifecycle cost; handback. | Quote-comparison table; due-diligence checklist; contract issue list; cost model; evidence request. | Does not publish volatile price lists or endorse vendors without evidence; `/panggung/` owns service conversion. | 6 |
| PGG-15 | Logistics, erection, work at height, and dismantling | Plan a controlled build and strike sequence with competent crews, lifting, access, exclusion, and quality checkpoints. | Delivery; staging area; sequencing; temporary stability; work at height; material handling; lifting; public separation; lighting; fatigue; housekeeping; build checks; strike after weather or damage. | Method-statement skeleton; sequence diagram; exclusion-zone plan; work-at-height checklist; supervisor sign-off. | Does not teach unsafe assembly or replace system instructions; PGG-08 owns lifting/rigging design and PGG-16 owns final acceptance. | 6 |
| PGG-16 | Inspection, testing, commissioning, and handover | Verify that the installed stage matches approved information and is ready for controlled use. | Document review; geometry; connections; bracing; ballast/anchors; decks/edges/access; rigging; electrical; fire; defects; load testing when specified; acceptance; baseline photos; handover. | Inspection and test plan; punch list; acceptance record; photo register; qualified sign-offs. | A visual checklist cannot certify structural or electrical safety; PGG-17 owns recurring operational checks and PGG-18 owns asset maintenance. | 6 |
| PGG-17 | Live operation, monitoring, change control, and incidents | Keep the stage within approved conditions throughout rehearsals, performances, and changeovers. | Opening/shift checks; access control; weather; load/set changes; unauthorized modifications; crowd interface; communications; alarms; stop-work/show-stop; incident/near miss; debrief. | Operations log; command chart; change request; incident form; monitoring dashboard; scenario drills. | Does not redesign the stage during a show; changes return to PGG-05, PGG-08, PGG-11, and PGG-13 owners. | 6 |
| PGG-18 | Maintenance, transport damage, repair, storage, and end of life | Preserve traceability and decide when to clean, inspect, repair, quarantine, replace, reuse, or retire an asset. | Maintenance intervals; transport damage; water/corrosion; fastener/connection wear; deck damage; cleaning/drying; storage; repair authorization; parts traceability; inventory; retrofit; recycling/decommissioning. | Asset register; inspection photos; maintenance schedule; quarantine tag; repair/replacement decision tree; manufacturer/engineer review. | Does not provide improvised structural repair instructions; PGG-16 owns installed-stage acceptance and PGG-14 owns procurement. | 6 |

## Related-domain opportunities

These are cross-domain collaboration opportunities, not cannibalization restrictions:

| Related domain | Independent perspective | Useful connection |
|---|---|---|
| `genset.co.id` | Generator selection, installation, testing, operation, and maintenance | PGG-11 may link to generator fundamentals while retaining stage power-distribution intent. |
| `safety.co.id` | Broader occupational and project safety systems | PGG-12, PGG-15, and PGG-17 can exchange checklists and incident-learning perspectives. |
| `kawat.id` | Wire, wire-rope, mesh, and related material knowledge | PGG-08 may refer readers to deeper wire-rope material education without outsourcing rigging responsibility. |
| `lantai.id` | Permanent floor systems and surface lifecycle | PGG-09 may connect permanent-stage finish questions while retaining stage-access intent. |

Separate domains may cover the same query independently because cannibalization control applies within one domain.

## Consolidation plan

1. Export GSC URL/query data, backlink evidence, lead data, deployed status, canonicals, and current local capability for every location family.
2. Freeze creation of new location-swapped pages until a location has material local evidence.
3. Decide the neutral index (`/artikel/` preferred) and keep commercial hubs as the only owners of rental intent.
4. Preserve any location URL with useful history and genuinely local service evidence; otherwise merge, noindex, canonicalize, or redirect only after an evidence-based mapping.
5. Make category roots subordinate to commercial hubs; noindex repetitive pagination and `/berita/page/*` where it adds no search value.
6. Remove `/404` from generated inventories and resolve the two sitemap disagreements.
7. Correct `[Lokasi]` and other template residue, unsupported superlatives, and claims that lack real stock, crew, geographic, or project proof.
8. Publish only the first bounded knowledge cluster, measure it, and expand by completed topical clusters—not isolated volume.

## Internal-link architecture

- Central hub: PGG-01-A01 introduces the knowledge system and links to all parent hubs.
- Planning sequence: PGG-02 brief → PGG-03 survey → PGG-05 load inputs → PGG-13 documents/approvals → PGG-14 procurement.
- Build sequence: PGG-07 support → PGG-08 rigging → PGG-11 electrical → PGG-15 erection → PGG-16 acceptance.
- Public-safety sequence: PGG-09 access → PGG-10 crowd interface → PGG-12 emergency planning → PGG-17 live monitoring.
- Lifecycle sequence: PGG-16 handover → PGG-17 operations → PGG-18 maintenance/repair/end of life.
- Diagnostic pages link backward to prevention and forward to stop, qualified review, repair, or replacement.
- Every child article links to its topic hub; every hub lists all six children. Related links are selected by decision sequence, not copied as a generic block.
- Neutral pages link to `/panggung/` only where procurement intent is explicit. Equipment routes remain commercial owners.

## Evidence and editorial standards

As of 2026-07-23, the official sources below provide a verified starting register. Status and applicability must be rechecked at drafting and project use:

- Indonesia's [PP 16/2021 on implementation of the Building Law](https://peraturan.bpk.go.id/Details/161846/pp-no-16-tahun-2021) is listed as in force and addresses structural loads, fire, lightning, and electrical safety. Whether a particular temporary or permanent stage falls within a specific building-control path requires local authority and professional confirmation.
- BSN lists [SNI 1727:2020](https://pesta.bsn.go.id/produk/detail/12927-sni17272020) (minimum design loads and related criteria), [SNI 1729:2020](https://pesta.bsn.go.id/produk/detail/12882-sni17292020) (structural steel), and [SNI 1726:2019](https://pesta.bsn.go.id/produk/index?key=1726) (earthquake-resistant design for building and nonbuilding structures) as active. Do not quote clauses or assume applicability without licensed access to the current text and qualified design review.
- Kemnaker lists [Permenaker 9/2016](https://jdih.kemnaker.go.id/peraturan/detail/1210/peraturan-menteri-nomor-9-tahun-2016) on work at height, [Permenaker 8/2020](https://jdih.kemnaker.go.id/peraturan/detail/1668/peraturan-menteri-ketenagakerjaan-nomor-8-tahun-2020) on lifting/transport equipment, [Permenaker 12/2015](https://jdih.kemnaker.go.id/peraturan/detail/610/peraturan-menteri-nomor-12-tahun-2015) as amended by [Permenaker 33/2015](https://jdih.kemnaker.go.id/peraturan/detail/1156/peraturan-menteri-ketenagakerjaan-nomor-33-tahun-2015) on workplace electrical safety, and [Permenaker 5/2018](https://jdih.kemnaker.go.id/peraturan/detail/1546/peraturan-menteri-nomor-5-tahun-2018) on workplace environmental safety as in force.
- The national regulation portals list [Permen PUPR 14/PRT/M/2017](https://www.peraturan.go.id/id/permen-pupr-no-14-prt-m-2017-tahun-2017) on building accessibility and [Permen PU 26/PRT/M/2008](https://peraturan.bpk.go.id/Details/104475/permen-pupr-no-26prtm2008-tahun-2008) on technical fire-protection systems as in force. Local rules, permits, and venue requirements still need verification.
- The UK HSE's current guidance on [temporary demountable structures](https://www.hse.gov.uk/event-safety/temporary-demountable-structures.htm), [venue and site design](https://www.hse.gov.uk/event-safety/venue-site-design.htm), [outdoor equipment supporting speaker clusters and lights](https://www.hse.gov.uk/event-safety/outdoor-equipment.htm), [crowd risk](https://www.hse.gov.uk/event-safety/crowd-management-assess.htm), and [incident/emergency planning](https://www.hse.gov.uk/event-safety/incidents-and-emergencies.htm) is useful non-Indonesian regulator guidance. It is not Indonesian law and must be translated into local project requirements.

Editorial rules:

1. Label verified law/standard status, professional interpretation, manufacturer data, field observation, and editorial inference separately.
2. Never publish a capacity, span, member, ballast, anchor, wind, crowd, rigging, electrical, or fire number without traceable assumptions, a named source, units, revision date, and qualified review.
3. Every safety procedure includes competence requirements, prerequisites, stop conditions, emergency escalation, and verification.
4. Diagrams are conceptual unless explicitly approved for a named project; never present a generic detail as construction-ready.
5. Case studies require real source documents, consent, dates, constraints, changes, and measured outcomes. No invented projects or incidents.
6. Regulations, SNI status, manufacturer manuals, and local requirements are rechecked at drafting and review dates are displayed.
7. Pages with material safety consequences receive structural/electrical/fire/rigging/accessibility review as applicable before publication.
8. Use Indonesian event terminology, climate, procurement, and authority context; avoid translating foreign rules as if locally binding.

## First bounded publication cluster

Publish these 12 P0 assets as one coherent planning-and-acceptance path:

1. PGG-01-A01 — stage types, functions, and boundary.
2. PGG-01-A03 — stage anatomy and interfaces.
3. PGG-02-A01 — event stage brief.
4. PGG-03-A01 — site survey checklist.
5. PGG-05-A01 — conceptual load path.
6. PGG-06-A01 — wind effects on roofs, screens, and backdrops.
7. PGG-08-A01 — rigging plot and responsibility inputs.
8. PGG-09-A01 — stairs, ramps, and access planning.
9. PGG-10-A01 — stage/audience site-plan method.
10. PGG-11-A01 — temporary electrical planning inputs.
11. PGG-15-A01 — erection/dismantling method statement.
12. PGG-16-A01 — pre-opening inspection and acceptance checklist.

The cluster takes a reader from definition to brief, survey, safety-critical interfaces, build method, and acceptance. It is broad enough to prove connected expertise but bounded enough to obtain qualified review.

Monitor indexation and canonical selection; impressions and clicks by distinct intent; brief/checklist completion or downloads; movement from neutral guides to a relevant commercial route; qualified enquiries with project/site information; engagement with safety stop conditions; and GSC evidence of two pages competing for the same query. Ranking alone is not a success criterion.

## Definition of done

- All 18 topics have six distinct catalog briefs, for 108 total.
- Every article has a unique ID, title, slug, primary intent, reader, promise, named exclusion owner, evidence format, related IDs, priority, and bounded wave.
- Proposed slugs do not collide with audited existing routes.
- Same-domain overlap groups have one intent owner; cross-domain overlap is not suppressed.
- The 4,409 location-swapped pages and 881 archive/pagination routes have an evidence-based consolidation decision before large-scale publication.
- The first cluster has current source checks and required professional reviews before drafting claims with safety consequences.
- Every article has a hub link, useful lateral links, and no orphan.
- GSC, lead quality, task completion, and cannibalization are reviewed after each wave before the next wave is authorized.
