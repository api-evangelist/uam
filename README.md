# Autonomous University of Madrid (uam)

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
