[README.md](https://github.com/user-attachments/files/35121041/README.md)
# Construction Timelapse (prototype)

Browser-based 4D/5D construction timelapse prototype: planned sequencing playback, as-built progress status, and earned-value financials for a linear viaduct. Three.js, single HTML file, **demo data only**.

**Live:** https://fletchercon.github.io/construction-timelapse/ (add `#progress` to open the Current progress view)

## Views
- **Planned sequencing (4D):** play or scrub the programme; elements appear on their scheduled start.
- **Current progress (4D):** status colours at a chosen status date, scheduled vs effective progress, overdue items.
- **Financials (5D):** BAC, PV, EV, AC, CPI/SPI, EAC, risk cards and a copyable payment claim schedule.

## Data
Geometry, programme and costs are generated in the page. The **⇅ Data** button exports the element register as CSV and imports a CSV keyed by `id` with any of `plan_start`, `plan_finish`, `budget_nzd`, `actual_start`, `actual_finish`, `cost_to_date_nzd` (YYYY-MM-DD). Nothing leaves the browser.

## Production path
Revit / Civil 3D → IFC → (web-ifc + Three.js, Cesium 3D Tiles, or ArcGIS I3S); P6 activities linked to element IDs; actuals from site records and the cost report.

Prototype by Fletcher Construction – Engineering Services. Not connected to live project data.
