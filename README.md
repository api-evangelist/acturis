# Acturis (acturis)

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

Acturis is a United Kingdom insurance software company founded in 2000 by David McDonald and Theo Duchen, operating the UK's leading multi-tenant SaaS platform for general insurance brokers, insurers and MGAs. The Acturis system covers commercial and personal lines broking, e-trade and digital distribution, policy administration, claims, document management, premium finance and accounting, and it builds and runs eight of the top ten UK insurer extranets. Acturis Group extends the platform into Germany, France and Canada (through the acquisitions of Power Broker and Brovada) and reports over 100,000 users across more than 40 countries.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/acturis/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/acturis/refs/heads/main/apis.yml)

## Tags

- Insurance
- United Kingdom
- Broker
- Agency Management
- Policy Administration
- Claims
- Property and Casualty
- Insurtech
- E-Trade
- MGA

## Timestamps

- **Created:** 2026-07-25
- **Modified:** 2026-07-25

## APIs

**None listed — and that is the finding.**

Acturis publishes no public developer portal and no downloadable API definitions. `developer.acturis.com`, `developers.acturis.com`, `docs.acturis.com` and `api.acturis.com` do not resolve; `/developers`, `/developer`, `/api` and `/integrations` all return 404. There is not even a login wall to record — there is simply no developer surface.

The word "API" appears on acturis.com only as marketing adjective — "our API-enabled platform will integrate seamlessly with any existing or future systems you use" (insurer page) and "our API capabilities and two-way integration with third parties" (commercial lines page) — with no reference documentation behind either claim.

The only concretely named API is the **Aviva claims Broker API**, announced 2024-12-13: a one-way transfer of individual claim records and updates from Aviva's claims system into a broker's Acturis system, covering personal and commercial lines motor, property and liability claims. It is free to brokers but enabled through an Aviva Claims Service Manager or an Acturis Account Manager — partner registration, not signup — and no endpoints, payloads, authentication scheme or specification are published.

Because no real specification exists, this repo has no `openapi/` directory. Nothing was reconstructed.

## Standards posture

The UK has no open-insurance obligation, so the machine-readable layer under UK broking is not a regulator's API. It is **Polaris Standards** and the **imarket** digital-trading service — code lists, question sets, data dictionaries, and messaging in EDI, XML and JSON. Acturis has traded on this since "May 2005 Acturis facilitates first insurer integration with industry portal iMarket," and Polaris lists Acturis among the integrated broker systems.

**ACORD posture:** no ACORD reference found on acturis.com. ACORD lineage reaches Acturis only through the Canadian arm — Acturis Canada earned CSIO's API Security Standards Certification on 2026-01-26 and raised its overall CSIO Standards Certification Rating to Gold, and the CSIO XML Standard is licensed to CSIO by ACORD.

## Quote / bind / issue / FNOL

| Verb | Publicly exposed | Notes |
| --- | --- | --- |
| Quote | No | Comparative quoting runs inside the Acturis UI and via imarket. |
| Bind | No | E-trade bind is a platform function behind a broker login. |
| Issue | No | Policy administration and document issue are platform functions. |
| FNOL | No (partial, inbound) | The Aviva Broker API pushes claim records *into* Acturis; it is not third-party FNOL submission and is not self-serve. |

Audience for every path above: **partner-only**.

## Links

- [Website](https://www.acturis.com/)
- [About Acturis](https://www.acturis.com/about-acturis/)
- [Product](https://www.acturis.com/product/)
- [News](https://www.acturis.com/news/)
- [Contact](https://www.acturis.com/contact/)
- [Acturis Group](https://acturisgroup.com/)
- [LinkedIn](https://www.linkedin.com/company/acturis)

## Review

See [review.yml](review.yml) for the full probe log, HTTP statuses, standards posture, auth model, and sources.
