# Requests for exact survey and approved plans

**Purpose:** obtain architecturally accurate, permission-to-use drawings of the Yeoval aged-care campus at **3–7 Lord Street, Yeoval NSW 2868** (historic government records also refer to **1 Lord Street** and **3–5 Lord Street**). This is the one important gap preventing a truly precise floorplan/3D model.

These are **ready-to-copy drafts**. They have **not been sent** to anyone.

## 1. Cabonne Council — development, construction and surveying records

**To:** council@cabonne.nsw.gov.au  
**Subject:** Public plans request — UPA Yeoval / Hazelholme / Yeoval Community Nursing Home, Lord Street

Hello Cabonne Planning team,

I'm undertaking a historical architectural research project about UPA Yeoval Aged Care, also recorded as Yeoval Community Nursing Home and Hazelholme Hostel. I'm trying to establish the real building footprint, wing locations, dimensions and external elevations at 3–7 Lord Street, Yeoval NSW 2868 (including historical address references to 1 Lord Street and 3–5 Lord Street).

Could you please identify the relevant DA / CDC / construction certificate references and advise how I can obtain publicly releasable records, especially:

- approved **dimensioned site surveys and site plans**, including boundary dimensions and all site Lot/DP identifiers;
- approved **architectural floor plans, elevations, sections and roof plans**, including drawing numbers, revision dates and scale;
- the building work that **connected two existing wings via a covered walkway**, completed around 2015–2016;
- any 2018–2022 development or refurbishment applications for the **western Netherwood Wing**, six additional beds, kitchen/lounge and dining expansion;
- older surveys or alterations associated with the **2012 plan of existing buildings** mentioned in UPA's annual report.

I am not asking for private resident information, security-system layouts or personal details. Redacted public-release documents covering **external massing and the general building envelope** would be very useful if more detailed internal plans are restricted.

Please let me know application numbers, document titles, access methods, fees and the contact person for a historical records request.

Kind regards,

## 2. UPA NSW — original commissioned plans

**Recipient:** UPA Property / Facilities team via official contact website [upa.org.au](https://www.upa.org.au/contact-us/) or the Yeoval service at [official Yeoval page](https://www.upa.org.au/locations/dubbo/yeoval-aged-care/). Check for the appropriate staff inbox before sending.

**Subject:** Yeoval Aged Care historical site plan (2012), walkway drawings (2016) and Netherwood Wing plans

Hello UPA team,

I am researching the architectural history of UPA Yeoval Aged Care for an educational 3D recreation.

Your **2012 annual report (printed p. 42)** mentions that a site plan of the existing buildings had been completed, with the intention of connecting two buildings. Your **2016 annual report** confirms a covered walkway joined the wings. Your **April–May 2019 Western Region Mail (p. 6)** describes proposed Western/Netherwood Wing alterations, six beds and a kitchen/lounge and dining expansion.

Would your property records contain any of the original **2012 site survey**, approved **2015–2016 walkway/site plans**, external **elevations or building dimensions**, or **Netherwood proposal plans**?

Even a **public-use, redacted external site plan or roof plan** with a scale and permission for research reference would help greatly. I don't need individual resident, care, or security information, and won't publish restricted drawings without permission.

Could you also confirm whether the six-bed Netherwood renovation was completed, and if so, approximately when?

Kind regards,

## 3. NSW Land Registry Services — cadastral geometry

Before assuming site area, verify **each parcel** comprising 1, 3, 5 and 7 Lord Street via the [NSW LRS online portal](https://online.nswlrs.com.au/) and [NSW Planning Spatial Viewer](https://www.planningportal.nsw.gov.au/spatialviewer/).

- **Unconfirmed lead only:** 1 Lord Street appears as **Lot 6, Section 12, DP 759140** on third-party [Allhomes](https://www.allhomes.com.au/1-lord-street-yeoval-nsw-2868). Other parcels might belong to the complex.
- Get **DP title/plan numbers, bounding distances, deposited survey plan, orientation, parcel boundaries**, and (if released) plan-of-subdivision contours.
- A cadastral survey shows *land boundaries*, not necessarily the walls, roof or floorplan.

## 4. How to turn a genuine plan into precise Repo Town geometry

1. Confirm plan date, drawing number, revision, orientation and scale/bar.
2. Confirm *all* occupied parcel boundaries and cadastral conversion to metres, and inspect imagery dates against the walkway.
3. Georeference a **roof/site plan** against at least three independently known coordinates, ideally surveyed plan points; record reprojection residual and drawing scale uncertainty.
4. Digitise separately: building polygons, wing outlines, roofs, entrance portico, covered walkway, landscaped beds, hardstanding/driveways; assign metres only when the image has a validated scale.
5. Record for every feature: source URI, document date, whether construction was complete, confidence and accuracy ±m.
6. Indoor spaces: only publish general public/authorised plans; use approximated generic rooms where publicly releasable originals are unavailable.
7. Test all model doors/circulation against publicly verifiable geometry, and avoid describing inferred coordinates as **100% true**.

## Record status

- Council DA search site: [Cabonne Development Application Tracker](https://cabonne.greenlightopm.com/search-register?deptName=Development).
- No numbered DA drawing, as-built survey, accurate measured 3D footprint or complete floor plan was retrieved as of **26 October 2026**.
- All unverified geometry dimensions are stored as `null` in [data/yeoval_geometry_status.json](../data/yeoval_geometry_status.json).
