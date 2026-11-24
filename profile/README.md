# OpenDepthMap

An open-source bathymetric mapping ecosystem and subsea situational awareness platform.

![OpenDepthMap - DIY Open Bathymetry & Scuba Navigation System Overview](https://raw.githubusercontent.com/opendepthmap/.github/main/profile/assets/opendepthmap-overview.jpg)

## Why This Project Exists

- **Lowering Financial & Navigational Barriers:** Commercial hydrographic survey gear and USBL underwater positioning systems cost tens of thousands of dollars, out of reach for individual divers, citizen scientists, and search-and-recovery clubs. Underwater, analog magnetic compasses are also disrupted by cross-currents, wrecks, reinforced concrete, steel cylinders, and low visibility. OpenDepthMap brings surface-tethered positioning and bathymetric logging within standard DIY maker budgets.
- **Closing the Nearshore "White Ribbon" Gap:** National survey vessels typically draw too much draft to safely map shallow rocky coastlines, intertidal reefs, and kelp beds (under 10-15 meters), while satellite-derived bathymetry fails in dark or turbid coastal waters. Surface micro-buoys and diver-towed sensors naturally fill this gap.
- **Tracking Storm & Dredging Change Over Time:** Shifting sandbars, mobile river mouths, dynamic shoals, and active channels change rapidly. Frequent community resurveys enable localized bathymetric differencing to track erosion, sediment deposition, and post-storm shifts.
- **Rescuing Sonar Data from Proprietary Silos:** Recreational boaters and anglers capture high-resolution sonar data every day that stays trapped inside closed manufacturer formats. OpenDepthMap brings vendor-neutral ingestion into open, standard geospatial formats with privacy-by-default controls.
- **Mapping Uncharted Inland Waters:** Millions of small lakes, quarries, and reservoirs remain completely unmapped by official agencies. Crowd-sourced open bathymetry gives local dive teams, water managers, and limnologists accessible depth charts.
- **Subsea Ecological Ground-Truthing & Hazard Mapping:** Depth soundings alone miss critical underwater context. Pairing depth data with diver-verified substrate types (sand, silt, bedrock, boulder), ecological tags (reefs, kelp holdfasts, invasive species), and geo-referenced underwater photos builds a richer subsea GIS layer.

## Built For

- **Recreational Scuba Divers & Foragers:** Offline dark-water depth charts, gloved magnetic-button hardware controls, locked return bearings, and privacy-by-default protection for sensitive reefs and shoreline entries.
- **Coastal Boaters, Anglers & Small-Craft Operators:** Explicit vertical datum labeling (never mixing unreduced raw transducer depth with tide-reduced chart datums), shoal hazard visibility, and open sonar log importing.
- **DIY Hardware Makers & Tinkerers:** Open-source surface survey buoy and diver receiver designs, accessible bills of materials, waterproofing guidance, and local browser-based device setup.
- **GIS Engineers & Marine Scientists:** Reproducible geospatial standards, quality-control flags, uncertainty grading, standardized marine taxonomy metadata, and open exports (OGC API - Features, IHO B-12 CSB, GeoParquet, CF-NetCDF, COG, and PMTiles).

## Roadmap Overview

| Phase | Focus | Status |
| :--- | :--- | :--- |
| **Phase 1** | Core Web Portal, Open Schemas & Cloud Processing Platform | In Design |
| **Phase 2** | Open-Source Autonomous Surface Survey Buoy (CAD & Firmware) | Planned |
| **Phase 3** | Tethered Spool Puck & Diver Hand/Wrist Receiver | Planned |

## Public Repositories

- **[opendepthmap/protocols](https://github.com/opendepthmap/protocols):** Public data schemas, wire protocols, external API specifications, and sanitized sample fixtures (CC0-1.0 / MIT).
- **[opendepthmap/hardware](https://github.com/opendepthmap/hardware):** Open-source hardware designs, CAD/STL files, bills of materials, and embedded firmware for Phase 2 and Phase 3 units (CERN-OHL-P v2 / MIT).

## Current Status

OpenDepthMap is currently in its **early architecture and specification phase**. Public schemas, reference fixtures, and hardware baselines will be published incrementally as each milestone is finalized.

## Attribution & Non-Navigational Disclaimer

Base map land and shoreline data derived from OpenStreetMap is used under ODbL 1.0 ([Map data © OpenStreetMap contributors](https://www.openstreetmap.org/copyright)).

> **Important:** Supplemental bathymetric reference only. Not certified for primary marine navigation; always consult official NOAA/IHO nautical charts. Hardware receivers are supplemental situational awareness tools and never replace a primary dive computer, analog backup compass, or physical reel guideline.
