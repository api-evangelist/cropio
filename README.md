# Cropio

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
> **Not from the company, and here with a question?** You are welcome here — we would rather be the
> front line and point you the right way than have a good report go nowhere. What this repository
> can answer is narrow, though, so it is worth knowing who you are actually looking for:
>
> - **A question about how the API works, an account, billing, or a bug in the service** — that is
>   the company's own support, not us. We profile this API; we do not operate it and cannot see
>   your account.
> - **A bug in an open-source project we only catalog** — file it on that project's own repository.
>   This has happened with a real and correct bug report that reached us instead of the people who
>   could fix it, which helped nobody.
> - **Anything about this listing itself** — the description, the tags, the rating, a missing or
>   wrong artifact — is ours. Open an issue here.
> - **Not sure, or something general about API Evangelist or APIs.io** — open an issue on the
>   [APIs.io Inbox](https://github.com/api-search/inbox) and we will route it.
>
> **This repository contains no software, and we will never ask you to download anything.** There is
> no build, release, installer, or binary here — only text and machine-readable API descriptions, so
> there is nothing here that can be "corrupt" or need "repairing". Any issue, comment, or email
> claiming otherwise and offering a download link is not from us and is hostile. Do not follow the
> link; it is a lure. Report it to GitHub and, if you like, tell us at
> [info@apievangelist.com](mailto:info@apievangelist.com) so we can take it down.
>
> **On a security or compliance team?** Email
> [info@apievangelist.com](mailto:info@apievangelist.com) with *security* in the subject line and
> you will get a person, not a form. We will tell you exactly which public URLs this profile was
> built from so your team can see the same surface we did, and we will take the listing down on
> request while you work through it.
>
> Full detail: **[Where this data comes from](https://apievangelist.com/about/where-our-data-comes-from)**
<!-- API-EVANGELIST-PROVENANCE:END -->

> **Acquired or rebranded.** This company was acquired, merged or renamed. Its API, if it still exists, is offered under another name. This profile is kept as a historical record and is not maintained or rated.

Cropio was an independent Eastern European farm management and precision agriculture platform (fields, satellite/NDVI imagery, weather, scouting, machinery telematics, and yield) founded in 2013. Syngenta acquired Cropio in September 2019 and folded it into its Cropwise digital agriculture portfolio; the product now operates as Cropwise Operations, and cropio.com redirects to operations.cropwise.com. The original Cropio API v3 was not shut down - it continues to run as the documented Cropwise Operations Platform API v3, reachable at operations.cropwise.com/api/v3 (the legacy cropio.com/api/v3 host has redirected there since April 1, 2022). It is a per-account HTTP JSON REST API (not a self-serve developer marketplace) - a Cropwise Operations login is required to obtain a USER_API_TOKEN, and there is no published self-signup API key flow or API-specific price list. Syngenta separately launched a broader "Cropwise Open Platform" for partners in 2025, which is a distinct, newer developer program outside the scope of this entry.

**Areas:** Agriculture · AgTech · Precision Agriculture · Farm Management · Satellite Imagery · NDVI · Weather · Telematics · Syngenta · Cropwise

## Cropio on APIs.io (historical record)

Everything profiled for Cropio is published on APIs.io rather than in this repository. Start at the provider page — **[apis.io/providers/cropio/](https://apis.io/providers/cropio/)** — or go straight to one of the APIs or properties below.

### APIs (7)

- [Cropio Fields API](https://apis.io/apis/cropio/cropio-fields-api/) — Create, list, get, update, and delete fields, field groups, field shapes (boundaries in multiple geo formats), and land parcels. Fields carry…
- [Cropio Crops API](https://apis.io/apis/cropio/cropio-crops-api/) — Manage crops (name, season type, base crop, color scheme), seasons (year, start/end date), production cycles, and growth stage / growth scale tracking used…
- [Cropio Satellite Imagery API](https://apis.io/apis/cropio/cropio-satellite-imagery-api/) — Read-only access to per-field and per-field-group satellite images - capture date, source satellite, cloud/cirrus/data coverage, and min/max/mean NDVI…
- [Cropio Weather API](https://apis.io/apis/cropio/cropio-weather-api/) — Read-only weather station data (real and virtual stations) keyed by geoposition, including a rolling 24-hour hourly current_weather array (precipitation,…
- [Cropio Scouting & Tasks API](https://apis.io/apis/cropio/cropio-scouting-and-tasks-api/) — Create and manage scouting tasks and manual tasks assigned to a field and a responsible user, plus the field scout reports, scout report points, and plant…
- [Cropio Machinery & Telematics API](https://apis.io/apis/cropio/cropio-machinery-telematics-api/) — Manage machines, implements, and machine tasks (driver, work type, field, start/end time), plus GPS logger data - raw and hourly-aggregated positions,…
- [Cropio Yield & Harvest API](https://apis.io/apis/cropio/cropio-yield-and-harvest-api/) — Read and write yield maps (per-field moisture/yield/applied property maps tied to a field work result), harvest weighings and transportations, and…

### Published properties

Each property below is a page on APIs.io carrying the machine-readable artifact and what it says.

#### Security (1)

Authentication, trust centre, and vulnerability disclosure.

- [Cropio Domain Security](https://apis.io/security/cropio/cropio-domain-security/)

#### Plans and pricing (1)

Published plans, tiers and prices.

- [Cropio Plans Pricing](https://apis.io/plans/cropio/cropio-plans-pricing/)

#### Rate limits (1)

Published request limits.

- [Cropio Rate Limits](https://apis.io/rate-limits/cropio/cropio-rate-limits/)

#### FinOps (1)

What the API costs to run, by operation.

- [Cropio Finops](https://apis.io/finops/cropio/cropio-finops/)

## Where to find this API

Links to the company's own pages. This repository publishes no copy of their specifications — the canonical document is theirs and lives at the URLs below.

- [Website](https://operations.cropwise.com)
- [Documentation](https://cropwiseoperations.docs.apiary.io/)
- [GitHub](https://github.com/cropio)

## API Evangelist rating

**Not rated** — this company is recorded as acquired or rebranded, so no score is published. If it is in fact operating, say so on this repository and it will be re-profiled.

## How this profile is made

API Evangelist profiles a company's public API surface the way a developer would find it: the website, developer portal and documentation, the specifications it publishes, its public repositories, and its pricing, status and changelog pages. From that it derives the properties above — contracts split per API, workflows, schemas, collections, governance rules, plans and rate limits — and scores them against the published [Kin Score rubric](https://github.com/api-evangelist/kin-score).

The artifacts are published on [APIs.io](https://apis.io), not in this repository. This repository is the public record for Cropio: the place to say something is wrong, missing or out of date, and to ask for a re-score or a removal.

## Open an issue

- **Something about this listing** — a wrong description, a missing API, a stale artifact or a question about the rating: [open an issue on this repository](https://github.com/api-evangelist/cropio/issues/new).
- **A new API, or one that is not in the catalog yet** — [submit it on APIs.io](https://apis.io/add/).
- **Anything else** — [the APIs.io inbox](https://github.com/api-search/inbox/issues/new) or [info@apievangelist.com](mailto:info@apievangelist.com).
