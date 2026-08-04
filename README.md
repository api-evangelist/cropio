# Cropio (cropio)

<!-- API-EVANGELIST-PROVENANCE:BEGIN -->
> ### About this repository
>
> **This is not our API.** This repository is an independent, third-party profile of a company's
> **publicly available** API surface, maintained by [API Evangelist](https://apievangelist.com).
> API Evangelist does not operate, host, resell, or support this company's APIs, and is not
> affiliated with or endorsed by the company unless stated on the profile.
>
> **Where the information came from.** Everything here is assembled from material a member of the
> public can reach with a browser and no credentials — the company's own website, developer portal
> and documentation, the specifications it publishes for public use (OpenAPI, AsyncAPI, JSON Schema,
> `apis.json`, `llms.txt` and similar), its public repositories, and its public status, pricing and
> changelog pages. **Nothing here is obtained by breaching a system, defeating an access control, or
> using credentials of any kind.**
>
> **The rating is an independent assessment.** The Kin Score and Agent Readiness rating are
> independently calculated scores of a company's *public* API artifacts, produced by API Evangelist
> against a published rubric. They are not certifications, endorsements, security assessments, or
> audits, and they score published artifacts — not the quality, safety, or security of the software.
>
> **Corrections, re-scores, and removal are free.** No partnership, contract, or purchase is
> required, and you do not need to justify the request.
>
> - **Something wrong?** Open an issue on this repository, or email
>   [info@apievangelist.com](mailto:info@apievangelist.com).
> - **Published something new?** Ask for a re-score and we will re-run the rating.
> - **Want the listing taken down?** Say so and we will honor it. The profile is reduced to your
>   company name, a factual description, and a link to your own site, and the company is recorded as
>   **unrated** — never scored zero for having asked.
>
> **Response times.** Acknowledgement within **one business day**; removal or restriction within
> **two business days**; corrections and re-scores within **five business days**.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

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
