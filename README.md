# UPA Yeoval Aged Care — evidence-based architectural research

**Research date:** 26 October 2026  
**Site:** 3–7 Lord Street, Yeoval NSW 2868, Australia  
**Operator:** United Protestant Association of NSW Ltd (UPA)  
**Goal:** Establish the *real* building footprint, layout, dimensions and external appearance before creating a geographically accurate virtual reconstruction.

> **Status: research in progress; exact plan NOT located.** Do not mistake this repository for an as-built survey. There is currently **no verified, dimensioned whole-building floor plan, CAD file, building footprint polygon, roof survey or room-by-room measured plan** in these findings.

## Outstanding research checklist (68 tasks)

The complete, prioritised checklist of **methods and tools not yet fully attempted**, including official planning records, NSW aerial imagery, geospatial measurement, archives, permission pathways and reproducible modelling, is in **[UNTRIED_RESEARCH_METHODS_TODO.md](docs/UNTRIED_RESEARCH_METHODS_TODO.md)**. It explicitly separates unattempted work from the failed/blocked Cabonne browser task. All items are open as of 26 October 2026; none should be marked complete without actual evidence.

## Latest primary-source breakthrough — building work completed by 2014

[UPA's 2014 annual report (printed p. 46)](https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2014.pdf.pdf) explicitly states the original two buildings already had a **permanent connection by 2014**, and **old interior walls were removed** to make the facility more open. A [first-hand account of the renovations](https://www.qpsbenchmarking.com/news/upa-yeoval-gaining-a-competitive-advantage-by-increasing-resident-satisfaction/) says **some rooms were demolished and replaced, and the dining room was rebuilt**. This is stronger than the later 2016 annual report's covered-walkway description. **Do not model an unchanged pre-2014 interior.** Whether the 2016 walkway mention describes the same connection or an additional improvement is unresolved.

The [2019 Yeoval manager's report (p. 6)](https://www.upa.org.au/wp-content/uploads/2019/04/Western-Region-Mail-April-May-2019.pdf) additionally confirms an **Acacia Room**, GP practice rooms and a turfed back garden. None gives exact room coordinates or sizes.

For the still-missing survey and drawings, see [ready-to-send requests to UPA and Cabonne Council](docs/REQUEST_FOR_ORIGINAL_PLANS.md).

## Important discoveries

1. **Two originally separate buildings / wings.** UPA's **2012 annual report, printed p. 42 (PDF p. 44)** says a site plan of the existing buildings had been made to guide refurbishment and that connecting *two buildings* was a primary aim. This establishes that a historical plan existed, **not** that it is freely downloadable. [UPA 2012 annual report](https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2012.pdf).
2. **The connecting walkway was built.** UPA's **2016 annual report, printed p. 41 (PDF p. 43)** says new building work *joined two wings by a covered walkway*. Important for any 2016-or-later external geometry. [UPA 2016 annual report](https://www.upa.org.au/wp-content/uploads/2016/12/Annual-Report-2016.pdf).
3. **Named western/Netherwood wing.** UPA's **2018 annual report, printed p. 21 (PDF p. 23)** documents roof gutter maintenance and repainting inside and out, and a **proposed** reopening of six beds in the Netherwood Wing. Its Western Region section also reports transferring **two bed places** from Yeoval Community Nursing Home to Bracken House. [UPA 2018 annual report](https://www.upa.org.au/wp-content/uploads/2018/10/UPA_AR2018_v_WEB.pdf).
4. **2019 renovation proposal.** UPA's April–May 2019 Western Region Mail says a proposed western-wing renovation and dining room expansion would create six additional beds and a kitchen/lounge space. These are proposals, **not proof of completed construction**. [Western Region Mail](https://www.upa.org.au/wp-content/uploads/2019/04/Western-Region-Mail-April-May-2019.pdf).
5. **2021–22 refurbishment status.** UPA's **2022 annual report, PDF p. 34** still describes the Netherwood Wing as being *considered for reopening* for lower-care respite residents; hence don't mark the proposed 2018–19 renovation as definitely completed. [UPA 2022 annual report](https://www.upa.org.au/wp-content/uploads/2022/10/Annual-Report-2022.pdf).
6. **Site organisation and beds.** The Australian Government's 2017 aged-care service list records separate entries at **3–5 Lord Street: Hazelholme Hostel, 17 residential places** and **1 Lord Street: Yeoval Community Nursing Home, 10 residential places** (total **27**). After the reported 2018 transfer of two places, a contemporary UPA brochure and directory describe **25 residents/places**. Distinguish *licensed places* from physical room counts. [2017 government data](https://www.gen-agedcaredata.gov.au/getmedia/62731781-470e-48ef-886c-b4a379ee8f8b/Australia_Service_List_2017.pdf), [UPA brochure](https://www.myagedcare.gov.au/sites/default/files/attachments/25/2-1X3TIX25.pdf).
7. **Verified room *area*, not plan dimensions.** My Aged Care advertises **26 m²** for shared room accommodation categories. This **does not establish the width, length, wall geometry, or area of single rooms**. [My Aged Care](https://www.myagedcare.gov.au/find-a-provider/search/ybsy5850hc-united-protestant-association-of-nsw-limited/aged-care-homes/yeoval-community-nursing-home-m0q0hm8h).
8. **Documented onsite spaces.** UPA's brochure lists lounges and activity rooms, kitchen, dining, library, hair salon, BBQ, landscaped gardens and single ensuite accommodation. The current UPA website also mentions shared (double) ensuite rooms, home care and a co-located community health centre. Note the brochure and UPA site describe room types slightly differently. [UPA brochure](https://www.myagedcare.gov.au/sites/default/files/attachments/25/2-1X3TIX25.pdf), [UPA official site](https://www.upa.org.au/locations/dubbo/yeoval-aged-care/).
9. **Street-facing appearance.** A publicly displayed photo shows reddish brick walls, a projecting gabled portico with light-coloured triangular lattice, UPA emblem, light columns, glazed entrance doors and brick paving. This is reliable **for the photographed entrance only**, not every elevation. [Caring Co photo / facility page](https://www.caringco.com.au/providers/yeoval-community-nursing-home).
10. **A possible cadastral lead, not verified site-wide title.** [Allhomes, 1 Lord Street](https://www.allhomes.com.au/1-lord-street-yeoval-nsw-2868) identifies *Lot 6, Section 12, DP 759140* for that address. This is **not proof that all 3–7 Lord Street facilities occupy only that lot**. Confirm all lots at NSW Land Registry Services / Cadastre.
11. **Two distinct historic government geocodes, not corner coordinates.** In 2017 federal provider data, Hazelholme is geocoded **(-32.75030022, 148.6498586)** and nursing home **(-32.75028137, 148.6504726)**. The points are **address/provider location markers**, *not* surveyed corners, parcel vertices or building centres. Do not derive precise roof or wall lengths from their separation. [2017 service list](https://www.gen-agedcaredata.gov.au/getmedia/62731781-470e-48ef-886c-b4a379ee8f8b/Australia_Service_List_2017.pdf).
12. **Community medical use.** A community health centre is listed at 3 Lord Street and Molong HealthOne GP services are listed at 3–7 Lord Street. Public service descriptions alone do not establish which rooms they currently occupy. [WayAhead](https://directory.wayahead.org.au/service/1599/), [NSW Health listing](https://playsafe.health.nsw.gov.au/healthcareservice/yeoval-general-practice/).

## What has *not* been verified

| Missing architectural datum | Finding |
|---|---|
| Whole-site dimensioned master plan | **Not located** |
| Main building exterior length × width × height | **Not established** |
| Parcel area and every Lot/DP for full site | **Not established** |
| Individual wing polygons, roof angles, footprint square metres | **Not established** |
| Number and exact placement of entry/exit doors, internal hallways, rooms | **Not established** |
| Ceiling heights, corridor widths, stair/threshold dimensions | **Not established** |
| Architect and contractor of Yeoval extensions | **Not established** |
| Completed status of Netherwood six-bed reopening | **Unconfirmed** |
| Google Maps / Street View measured drawing | **Not captured** |
| NSW Council DA plan sheets, sections or elevations | **Not obtained** |

**Please don't assign invented millimetre measurements or label schematic placements “as built”.**

## Next authoritative retrieval steps

1. [Cabonne Council DA Tracker](https://cabonne.greenlightopm.com/search-register?deptName=Development): search **1 Lord**, **3 Lord**, **3–5 Lord**, **3–7 Lord**, **Yeoval aged care**, **Hazelholme**, **Netherwood**, and retrospective applications 2007–2022. The publicly linked tracker uses JavaScript, and this research did not obtain a DA drawing.
2. Ask **Cabonne Council, (02) 6392 3200 / council@cabonne.nsw.gov.au**, for accessible approved **site plans, architectural floor plans/elevations, survey plans, alteration DAs and construction certificates** at the address, particularly the **2012 measured site plan**, the **2015–16 covered walkway approval**, and the **2018–19 Netherwood alterations**. Request documents suitable for public release, excluding confidential resident/security plans.
3. Use [NSW Planning Portal map](https://www.planningportal.nsw.gov.au/map), [NSW Spatial Viewer](https://www.planningportal.nsw.gov.au/spatialviewer/), [NSW LRS](https://online.nswlrs.com.au/), and [NSW cadastre](https://portal.spatial.nsw.gov.au/portal/home/item.html?id=6a96afdba8d6407d8bde5a3bbacb0f02) to check **all** cadastral lots, survey areas, boundaries, and DP plans.
4. Inspect high-resolution, **dated** satellite orthophotos (and available Street View) and record **per-wing exterior corner coordinates plus reference scale**, uncertainty, and whether imagery predates 2016 covered-walkway works. Do not measure from simple directory geocodes.
5. Ask UPA property/facilities team whether they can share a **public-use / redacted architectural plan** or exterior massing/elevations that does not expose private care-home security information.

## Data quality conventions

- **Verified:** explicit named primary source, with a URL and date/page.
- **Estimated:** derived from a dated georeferenced image, with methodology + error margin.
- **Unverified:** plausible feature, descriptive website claim without plans, or pending alteration.
- **Unknown:** no defensible measurements found. Leave fields null, not 0.

See [the detailed evidence register](docs/YEOVAL_ARCHITECTURE_EVIDENCE.md) and [machine-readable geometry status](data/yeoval_geometry_status.json). This is a source repository, **not** a claim of exact reconstruction.
