# Acturis (acturis)

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
