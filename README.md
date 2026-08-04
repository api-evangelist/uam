# Autonomous University of Madrid (uam)

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

The Autonomous University of Madrid (Universidad Autónoma de Madrid, UAM) is a public research university in Madrid, Spain, founded in 1968 and ranked #198 in the QS World University Rankings 2025. This repository catalogs UAM's public, machine-readable API footprint in APIs.json format. UAM's confirmed API surface is delivered through Biblos-e Archivo, its DSpace 7.6.5 institutional repository, which exposes a HAL-based REST API and an OAI-PMH 2.0 metadata-harvesting endpoint.

- APIs.json: https://raw.githubusercontent.com/api-evangelist/uam/refs/heads/main/apis.yml
- Run with Naftiko: https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=uam-api-evangelist&utm_content=repo

## Type

- Index / Consumer / 3rd-Party

## Tags

Education, Higher Education, University, Spain, Open Access, Institutional Repository, DSpace, OAI-PMH, Research

## APIs

- **Biblos-e Archivo REST API (DSpace 7)** — HAL-based REST API for the UAM institutional repository (DSpace 7.6.5). Base URL: `https://repositorio.uam.es/server/api`. Docs: https://repositorio.uam.es/server/api and https://biblioguias.uam.es/repositorio
- **Biblos-e Archivo OAI-PMH Endpoint** — OAI-PMH 2.0 metadata-harvesting endpoint. Base URL: `https://repositorio.uam.es/server/oai/request`. Docs: https://repositorio.uam.es/server/oai/request?verb=Identify

## Plans / Rate Limits / FinOps

- Plans: [plans/uam-plans-pricing.yml](plans/uam-plans-pricing.yml)
- Rate Limits: [rate-limits/uam-rate-limits.yml](rate-limits/uam-rate-limits.yml)
- FinOps: [finops/uam-finops.yml](finops/uam-finops.yml)

## Timestamps

- Created: 2026-06-03
- Modified: 2026-06-03

## Common Properties

- Website: https://www.uam.es/
- LinkedIn: https://es.linkedin.com/school/universidad-autonoma-de-madrid/
- Authentication (ID-UAM, gated SSO): https://id.uam.es/
- Plans: plans/uam-plans-pricing.yml
- Rate Limits: rate-limits/uam-rate-limits.yml
- FinOps: finops/uam-finops.yml
- Review: review.yml

## Notes

- Verification caveat: the Biblos-e Archivo REST API and OAI-PMH endpoints were confirmed live via content fetch (DSpace 7.6.5; OAI-PMH 2.0). Direct `curl` probes returned HTTP 403 due to bot/WAF filtering, but the endpoints resolve and return valid payloads.
- UAM has no centralized developer portal. Identity is handled by the gated ID-UAM federated service (not a documented public API).
- No official institutional GitHub organization was found (only research-group and student-club accounts), so no GitHub common property is listed.
- No endpoints were fabricated; only confirmed surfaces are cataloged.

## Maintainers

- Kin Lane — kin@apievangelist.com
