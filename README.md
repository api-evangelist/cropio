# Cropio (cropio)

Cropio was an independent Eastern European farm management and precision agriculture platform (fields, satellite/NDVI imagery, weather, scouting, machinery telematics, and yield) founded in 2013. Syngenta acquired Cropio in September 2019 and folded it into its Cropwise digital agriculture portfolio; the product now operates as **Cropwise Operations**, and `cropio.com` redirects to `operations.cropwise.com`.

## Operating status

- **Company:** Absorbed. Cropio no longer exists as an independent company or brand - it is now Cropwise Operations, part of Syngenta.
- **Product:** Live and active. `https://cropio.com` returns a 302 redirect to `https://operations.cropwise.com/`, which is a working, actively marketed "all-in-one digital farming solution."
- **API:** Live and unchanged in kind. The original **Cropio API v3** was not shut down - it continues to run as the documented **Cropwise Operations Platform API v3**, at `https://operations.cropwise.com/api/v3`. The legacy `https://cropio.com/api/v3` host has redirected to the new host since April 1, 2022, per Cropio's own migration notice in the docs.
- **Access model:** This is a per-account HTTP JSON REST API, not a self-serve developer marketplace. A Cropwise Operations login is required to obtain a `USER_API_TOKEN` (via `POST /sign_in` or from account settings); there is no public API-key signup form and no published, API-specific price list.
- **Separate, newer program:** In 2025 Syngenta announced a broader "Cropwise Open Platform" (`open-platform.cropwise.com`) for third-party developer co-innovation across its wider Cropwise portfolio. That is a distinct, newer initiative from the Cropio-lineage Operations API documented here and is out of scope for this entry.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/cropio/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/cropio/refs/heads/main/apis.yml)

## Tags

- Agriculture
- AgTech
- Precision Agriculture
- Farm Management
- Satellite Imagery
- NDVI
- Weather
- Telematics
- Syngenta
- Cropwise

## Timestamps

- **Created:** 2026-07-03
- **Modified:** 2026-07-03

## APIs

### Cropio Fields API

Create, list, get, update, and delete fields, field groups, field shapes (boundaries in multiple geo formats), and land parcels. Fields carry calculated/legal/tillable area, administrative location, and relations to crops, scouting reports, satellite images, and machine tasks.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)
- [SDK - cropio-ruby](https://github.com/cropio/cropio-ruby)

### Cropio Crops API

Manage crops (name, season type, base crop, color scheme), seasons (year, start/end date), production cycles, and growth stage / growth scale tracking used to plan and record what is planted on a field across a season.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)

### Cropio Satellite Imagery API

Read-only access to per-field and per-field-group satellite images - capture date, source satellite, cloud/cirrus/data coverage, and min/max/mean NDVI values - plus NDVI grid data for zoning and vegetation-health analysis.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)

### Cropio Weather API

Read-only weather station data (real and virtual stations) keyed by geoposition, including a rolling 24-hour hourly `current_weather` array (precipitation, air temperature, and related measurements) and historical weather items.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)

### Cropio Scouting & Tasks API

Create and manage scouting tasks and manual tasks assigned to a field and a responsible user, plus the field scout reports, scout report points, and plant threat findings recorded against them, and agri-work plans used to schedule field operations.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)

### Cropio Machinery & Telematics API

Manage machines, implements, and machine tasks (driver, work type, field, start/end time), plus GPS logger data - raw and hourly-aggregated positions, speed, and distance per machine - polled over HTTP with a required date/time filter. Marked "testing stage" by Cropio in the source docs.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)
- [SDK - cropio-powerbi](https://github.com/cropio/cropio-powerbi)

### Cropio Yield & Harvest API

Read and write yield maps (per-field moisture/yield/applied property maps tied to a field work result), harvest weighings and transportations, and productivity/yield estimates and their history, used to close the loop from field work back to harvest results.

- **Human URL:** [https://cropwiseoperations.docs.apiary.io/](https://cropwiseoperations.docs.apiary.io/)
- **Base URL:** `https://operations.cropwise.com/api/v3`

#### Properties

- [API Reference](https://cropwiseoperations.docs.apiary.io/)

## Common Properties

- [GitHub Organization](https://github.com/cropio)
- [LinkedIn](https://www.linkedin.com/company/cropio)
- [Website](https://operations.cropwise.com)
- [Documentation](https://cropwiseoperations.docs.apiary.io/)
- [Plans](plans/cropio-plans-pricing.yml)
- [Rate Limits](rate-limits/cropio-rate-limits.yml)
- [Fin Ops](finops/cropio-finops.yml)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
