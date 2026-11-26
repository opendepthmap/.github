# Security Policy

## Reporting a Vulnerability

OpenDepthMap is currently in **Early Alpha** (`v0.1.0-alpha`), and responsible vulnerability disclosures help protect contributors, their private tracks, and open datasets.

Please **do not** report security vulnerabilities through public GitHub Issues or Discussions.

Instead, submit a private report via GitHub Security Advisories on our public tracker:

- **Report Privately:** https://github.com/opendepthmap/docs/security/advisories/new

Please include:
1. Affected area (web portal feature, API endpoint, OGC/export endpoint, file parser, or hardware firmware).
2. Clear reproduction steps or a minimal proof of concept.
3. Expected vs. observed impact (for example, unauthorized access to private vault data or raw unredacted soundings).

We aim to acknowledge reports within **72 hours** and keep you updated as a fix is verified and released.

## Scope & Security Design

In-scope targets include:
- Hosted web portal UI and browser session workflows
- Public & authenticated HTTP API endpoints and OGC API - Features feeds
- Ingestion file parsers (`GPX`, `CSV`, `GeoJSON`, `NMEA 0183`, `IHO B-12 CSB / WIBL`)
- Public schemas, validators, and hardware firmware in `opendepthmap/protocols` and `opendepthmap/hardware`

Key architectural protections:
- **Private vs. Public Isolation:** Raw sonar uploads land in private storage and require explicit review, redaction/trimming, and `CC0-1.0` confirmation before public projection.
- **Key Separation:** Personal API keys (`odm_usr_*`) are strictly separated from write-only field-logger device keys (`odm_dev_*`), which cannot read your private vault.
- **No Unredacted Leaks on Deleted or Trimmed Tracks:** Deleting tracks or drawing private exclusion polygons invalidates derived public tiles and re-scrubs published geometry.

## Navigational Safety Disclaimer

OpenDepthMap charts and depths are supplemental bathymetric references only. They are not certified for primary marine navigation; always consult official NOAA or IHO nautical charts.
