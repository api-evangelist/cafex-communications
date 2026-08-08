# CafeX Communications

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

CafeX Communications, Inc. (founded 2013) builds a low-code platform for developing intelligent
applications and agentic systems for regulated industries — banking, insurance, healthcare and
government. The CafeX AI platform is delivered as multi-tenant SaaS at `app.cafex.com` and is
organised into App Studio (App Builder, Flow Builder, Rule Builder, Data Tables, API Lab), Data
Studio (Data AI, Data Gateway, Data Visualizer) and Agent Studio (Agent Builder, LM Insights).
CafeX began as a WebRTC and embedded-communications vendor (Fusion Client, Live Assist, CafeX
Meetings, later the Challo collaboration workspace) and has since repositioned around AI workflow
and process automation.

## Public API surface

CafeX publishes one public, callable API:

- **CafeX Audit Events API** — `POST https://app.cafex.com/audit-search-rest/search`, a tenant-scoped
  JSON search over audit event data, secured with an OAuth 2.0 client-credentials bearer token from
  `POST https://auth.cafex.com/authserver/token`. Cursor pagination (`page.continuationToken`,
  `pageSize` max 100), ISO 8601 timestamps, one-year event retention, eight-hour access tokens.
  Both endpoints were confirmed live by anonymous probe on 2026-08-08.

CafeX publishes **no** OpenAPI, AsyncAPI, GraphQL SDL, MCP server or A2A agent card, and no
`/.well-known/` discovery document on any host. The API contract exists only as prose in a help
center article. Note that `app.cafex.com` answers HTTP 200 with an SPA HTML shell for every
`/.well-known/*` path — those are not documents.

- Website: https://cafex.ai/ (cafex.com redirects here)
- Help center: https://support.cafex.com/support/solutions
- Status: https://status.cafex.ai/ · Trust center: https://trust.cafex.ai/
- GitHub: https://github.com/cafexcomms (5 legacy WebRTC repos, none updated since 2022)
- Secondary-market listing: https://forgeglobal.com/cafex-communications_stock/
