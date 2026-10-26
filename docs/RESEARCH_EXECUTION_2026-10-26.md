# Field research execution log — 26 October 2026

**Current status:** PARTIALLY COMPLETE. This is an evidence-backed log of actual operations, not 68 claimed completions.

## Confirmed primary breakthrough: two cadastral parcels

Using the **live NSW Spatial Services Land Parcel Property Theme FeatureServer, layer 8 (Lot)**, we:
- Queried by a tight geographic envelope around historical aged-care provider geocodes and by the third-party suggested `6/12/DP759140` lot.
- Queried **point-in-parcel polygon intersection** for the 2017 Hazelholme geocode `(148.6498586, -32.75030022)`. Result: **Lot 2 DP613049**, NSW `cadid=102274229`.
- Queried **point-in-parcel polygon intersection** for the 2017 Yeoval Community Nursing Home geocode `(148.6504726, -32.75028137)`. Result: **Lot 6 Section 12 DP759140**, NSW `cadid=102274021`. This independently validates that the third-party lot reference really is at that provider geocode, though it does **not** establish legal ownership.
- Downloaded **original multi-vertex cadastral boundaries** from the official API into [GeoJSON](../data/yeoval_nswsds_2026_cadastral_candidates.geojson). Coordinates are EPSG:4326. The two candidate parcels share a boundary segment.

### Measured from cadastral vector geometry (not from aerial roofs)

| Candidate parcel | Calculated geodesic area, m² | Perimeter, m | Boundary segments, m (in polygon winding order) |
|---|---:|---:|---|
| 2//DP613049 | **4,342.94** | **274.22** | 91.19; 50.29; 21.13; 6.38; 54.02; 51.20 |
| 6/12/DP759140 | **1,630.32** | **167.75** | 33.62; 51.20; 31.22; 51.71 |
| **These two parcels combined** | **5,973.26** | *not combined perimeter* | *not building dimensions* |

**Calculation:** WGS84/GRS80 ellipsoidal distance and polygon area using Python `pyproj.Geod(ellps='GRS80')`, retaining values rounded to 0.01 metre/metre². This level of numeric precision is a *calculation display*, **not** a survey accuracy claim. NSW data is an authoritative digital cadastral polygon, but authoritative **deposited plan measurements and current site ownership have NOT been retrieved**. The actual residential complex could include more land; buildings may not match lot borders. **Never insert the 91 m boundary segment as a building length.**

**Reference query:** [Official NSW polygon feature query](https://portal.spatial.nsw.gov.au/server/rest/services/NSW_Land_Parcel_Property_Theme/FeatureServer/8/query?where=cadid%20IN%20%28102274229%2C102274021%29%26outFields=lotidstring%2Clotnumber%2Csectionnumber%2Cplanlabel%2Ccadid%26returnGeometry=true%26outSR=4326%26f=pjson) (query arguments should be regenerated through [ArcGIS REST service](https://portal.spatial.nsw.gov.au/server/rest/services/NSW_Land_Parcel_Property_Theme/FeatureServer/8) if URL encoding changes).

**Primary provider-location source:** [Australian Government residential service list 2017](https://www.gen-agedcaredata.gov.au/getmedia/62731781-470e-48ef-886c-b4a379ee8f8b/Australia_Service_List_2017.pdf). These are provider geocodes and can be offset from actual entrance/building positions.

## Confirmed primary breakthrough: 2013 high-resolution imagery metadata

Queried **NSW Spatial Services [NSW_Imagery_Theme/MapServer/0](https://portal.spatial.nsw.gov.au/server/rest/services/NSW_Imagery_Theme/MapServer/0)** at a coordinate inside the candidate complex.

Returned record:

```json
{
  "BlockName": "YEOVAL",
  "BlockType": "ADS40Towns",
  "BlockStartDate": 1376352000000,
  "BlockStartDate_UTC": "2013-08-13T00:00:00Z",
  "Resolution_cm": 10,
  "HighPS": 2,
  "LowPS": 0
}
```

**Interpretation:** Official imagery catalogue **reports** a Yeoval mosaic block starting **13 August 2013** at nominal **10 cm** resolution. It is a credible lead for pre/around-2014 renovation roof outlines. It **does not** show that current 2026 basemap tiles at this point are actually rendered from this particular block, nor that image extraction succeeded. An aerial crop and roof digitisation were **not obtained**. NSW's [Basemap metadata](https://portal.spatial.nsw.gov.au/client/services?id=c04ce33be7a04a7884f786f5beb20b19) warns date and resolution can depend on zoom level, and advises checking per-image date using **Explorer Identify**.

## Newly corroborated 2020 capacity

A [NSW Parliament-published Commonwealth 2020 aged care list](https://www.parliament.nsw.gov.au/lcdocs/other/15601/Attachment%202%20-%20Mr%20Paul%20Versteege%20-%20NSW%20service%20list%20Australia-at-30-June-2020.pdf) records **Yeoval Community Nursing Home at 1 Lord St as 8 allocated places**, consistent with a 2018 transfer of **two places** from its 2017 count of 10. Combined with the historic **17-place Hazelholme** service, this supports **25 places in 2020**. These are regulatory places, not 25 known single bedrooms. The 2020 source also shows a changed location point longitude compared with the 2017 service list: **do not treat either as a surveyed corner**.

## Planning register / dataset access tests

- [Cabonne DA Tracker](https://cabonne.greenlightopm.com/search-register?deptName=Development): prior TinyFish GUI automation prevented from starting due to negative wallet; this run did **not** recover actual DA attachments through text indexing. **No negative DA finding is justified.**
- [NSW Online DA Data API](https://www.planningportal.nsw.gov.au/opendata/dataset/online-da-data-api) located; dataset page provides **data broker contact and data dictionary**, not an immediately downloaded site-specific result set. The [NSW APIs portal](https://www.planningportal.nsw.gov.au/API) says the integration APIs require subscription keys. Specific application numbers **remain unknown**, and the API may omit pre-July 2021 lodgements.
- Targeted public-index searches for Yeoval Lord Street development applications (Cabonne domain, Planning Portal, commercial DA aggregators) did **not surface an unequivocal matching application** in the checked public results. This cannot establish that no applications exist.
- [Cabonne Informal GIPA policy](https://www.cabonne.nsw.gov.au/Council/Information-Access/Public-Access-to-Information-GIPA) confirmed. Free informal access first; a paid formal application requires a **$30 application fee plus possible $30/hour processing**, user approval and an Australian postal address.
- **Actual email requests SENT** from the user's connected personal Gmail on **26 October 2026**:
  - Council `council@cabonne.nsw.gov.au` — Gmail Sent message ID `1a177faede6be585`. Asked for plans, DA file numbers, cadastral boundaries and archives.
  - UPA `info@upa.org.au` — Gmail Sent message ID `1a177faf8c348180`. Asked for 2012 plan, 2014 plans, Netherwood status and public-release licensing.
  - These IDs are provided only for follow-up tracking and should not expose private email bodies or contact metadata in public-facing exports beyond this minimally necessary log.
- This is **not a formal paid GIPA submission** and responses have not been received/verified.

## Building-footprint database attempts

1. Queried [NSW Environment's 'Building' polygon layer](https://mapprod.environment.nsw.gov.au/arcgis/rest/services/Basemap/Basemap_DIO_GCS_GDA2020/MapServer/390) within a tight Lord Street bounding box. **0 features returned** in this layer. This means *that particular layer* doesn't provide site roofs in that query; it does not prove no buildings exist.
2. Found [Microsoft open Australian footprint dataset](https://github.com/microsoft/AustraliaBuildingFootprints), ~11.3 million model-generated polygons, but its country-wide bulk file is large and was **not extracted**.
3. Found [Microsoft Global ML Building Footprints](https://github.com/microsoft/GlobalMLBuildingFootprints) and [Overture Maps building data](https://docs.overturemaps.org/getting-data/) with location/bounding-box extraction options. **Candidate data has not yet been downloaded or intersected.** Footprints from these sources are model-derived and need aerial confirmation.

## Attempts that failed to produce data

- **Direct OpenStreetMap API and Overpass** query URLs returned "not accessible" in available web retrieval; an empty footprint result **cannot** be inferred.
- **Direct Python HTTPS requests** to public websites failed with DNS/name-resolution errors in the local sandbox; this is an environment limitation, not source absence.
- **NSW imagery tile export** was not retrieved from available web/container tools; therefore **no building roof geometry** has been measured, notwithstanding the excellent 2013 10 cm metadata.
- **Dynamic NSW address prototype FeatureServer** search for Yeoval yielded zero matches in the tested partial/prototype layer; the authoritative parcel geometry service *did* work by spatial query. A zero response from this specific prototype does not disprove the addresses.

## To do immediately next

1. Access the **2013 10 cm NSW YEOVAL imagery** and inspect image date/coverage at each wing, digitise roofs with error.
2. Retrieve **Overture/Microsoft per-region building footprints**, spatially intersect with the two parcel GeoJSON polygons and validate by independent aerial.
3. Obtain Council's historical **DA/BA numbers and 2012 UPA survey** through already sent correspondence, without paid steps unless authorised.
4. Verify both **Lot/DP ownership/parcel inclusion** via NSW LRS/deposited plan, noting possible additional campus parcels.
5. Update the [68-item checklist](UNTRIED_RESEARCH_METHODS_TODO.md) with **statuses per task** instead of marking everything done.

**No claim is made that the entire 68-task list is complete; physical surveys, paid sources, confidential plans, and permission-dependent tasks remain gated.**
