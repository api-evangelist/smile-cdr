# Smile Digital Health (smile-cdr)

Smile Digital Health (formerly Smile CDR) is a Toronto-based health interoperability software company and the commercial steward of the open source **HAPI FHIR** project — the world's most widely deployed Java implementation of the HL7 FHIR standard. Its flagship platform, **Smile CDR** (marketed under the **Smile Omni** portfolio as the **OmniVera Health Data Platform**), is a FHIR-native clinical data repository and integration engine that ingests HL7 v2.x, CDA, CSV, JSON, XML, and FHIR payloads, normalizes them to FHIR (R4, R5, STU3, DSTU2), and exposes them through a hardened FHIR REST API, SMART on FHIR / OAuth2 / OIDC, Bulk Data, Subscriptions, MDM, Terminology Services, CQL-based Quality Measures, and a JSON Admin API.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/smile-cdr/refs/heads/main/apis.yml)

## Tags

- Healthcare, FHIR, HL7, Clinical Data Repository, Interoperability, HAPI FHIR, SMART on FHIR, Terminology Services, MDM, Bulk Data, Subscriptions, CMS Interoperability, Prior Authorization, Digital Quality Measures, CQL, Payer, Provider

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## Smile Omni Product Families

| Family | Purpose | Key Modules |
|---|---|---|
| **OmniVera** | FHIR-native data platform (Smile CDR) | Health Data Platform, Data Quality+, Data Access+ |
| **OmniCompli** | Regulatory compliance for US payers | CMS Suite, CMS Suite+, CMS Concierge |
| **OmniQ** | Digital quality measurement | dQM (HEDIS + custom), Intelligence Hub |
| **OmniConcierge** | Implementation and operations | Managed Services, Professional Services, Knowledge |

## APIs

### Smile CDR FHIR Endpoint
Core FHIR REST API — full FHIR REST interaction set (read, vread, update, patch, delete, history, search, transaction, batch, conditional CRUD) across FHIR R4, R5, STU3, DSTU2. OpenAPI / Swagger UI auto-generated at `{baseUrl}/swagger-ui/`.

- [Documentation — FHIR Standard](https://smilecdr.com/docs/fhir/standard.html)
- [Documentation — CRUD Operations](https://smilecdr.com/docs/fhir/crud_operations.html)
- [Documentation — Searching](https://smilecdr.com/docs/fhir/searching.html)
- [OpenAPI / Swagger Support](https://smilecdr.com/docs/fhir_repository/openapi_swagger.html)
- [Public Swagger UI — HAPI FHIR test server](https://hapi.fhir.org/baseR4/swagger-ui/)

### Smile CDR SMART on FHIR
SMART on FHIR / OAuth2 / OIDC authorization for FHIR endpoints — standalone launch, EHR launch, PKCE, refresh tokens, consent, `.well-known/smart-configuration`.

- [Documentation — SMART on FHIR](https://smilecdr.com/docs/smart/index.html)
- [Documentation — OpenID Connect](https://smilecdr.com/docs/security/openid_connect.html)

### Smile CDR Bulk Data
FHIR Bulk Data Access (Flat FHIR) — asynchronous system-, group-, and patient-level NDJSON export with backend-services authorization.

- [Documentation — Bulk Export](https://smilecdr.com/docs/bulk/fhir_bulk_export.html)
- [Documentation — Bulk Import](https://smilecdr.com/docs/bulk/fhir_bulk_import.html)

### Smile CDR Subscriptions
FHIR R4 Subscription and R4B/R5 Subscription / SubscriptionTopic backport — REST hook, websocket, email, and message-queue channels.

- [Documentation — Subscriptions](https://smilecdr.com/docs/fhir/subscriptions.html)

### Smile CDR Master Data Management
FHIR-native MDM for Patient and Practitioner — probabilistic matching, golden records, candidate rules, survivorship, `$mdm-*` operations, MDM Admin endpoint.

- [Documentation — MDM](https://smilecdr.com/docs/mdm/mdm.html)

### Smile CDR Terminology Services
`$expand`, `$validate-code`, `$lookup`, `$translate`, `$subsumes` over CodeSystem, ValueSet, ConceptMap. Bundled SNOMED CT, LOINC, ICD-10/11, RxNorm, CPT.

- [Documentation — Terminology](https://smilecdr.com/docs/terminology/index.html)

### Smile CDR CQL & Quality Measures
Clinical Quality Language engine and FHIR Clinical Reasoning module backing **OmniQ dQM** including HEDIS — `$evaluate-measure`, `$apply`.

- [Documentation — Measures](https://smilecdr.com/docs/measures/index.html)

### Smile CDR CDA Exchange
Bidirectional HL7 CDA / C-CDA exchange — CDA-to-FHIR ingest and FHIR-to-CDA rendering.

- [Documentation — CDA Exchange](https://smilecdr.com/docs/cda_exchange/cda_exchange.html)

### Smile CDR HL7 v2.x Interface
MLLP HL7 v2.x inbound and outbound — ADT, ORM, ORU, MDM, SIU, VXU, DFT — with v2-to-FHIR mapping.

- [Documentation — HL7 v2.x](https://smilecdr.com/docs/hl7v2x/hl7v2x_support.html)

### Smile CDR JSON Admin API
REST/JSON admin surface — Module Config, System Config, User Management, Audit Log, Transaction Log, Metrics, Runtime Status, Batch Job, Bulk Import, MDM Admin, OpenID Connect Clients / Keystores / Servers / Sessions.

- [Documentation — JSON Admin API](https://smilecdr.com/docs/json_admin_endpoints/json_admin_api.html)
- [Documentation — Module Config Endpoint](https://smilecdr.com/docs/json_admin_endpoints/module_config_endpoint.html)
- [Documentation — User Management Endpoint](https://smilecdr.com/docs/json_admin_endpoints/user_management_endpoint.html)

### Smile CDR CMS Interoperability Suite
Pre-packaged CMS-compliant FHIR APIs for US payers — Patient Access, Provider Directory, Drug Formulary, Payer-to-Payer (CMS-9115-F), Prior Authorization (CMS-0057-F / Da Vinci PAS, CRD, DTR). Built on US Core, CARIN BB, Da Vinci, PDex profiles.

- [Solution — CMS Suite](https://www.smiledigitalhealth.com/solution/cms-suite)

## Open Source — HAPI FHIR

Smile Digital Health maintains [HAPI FHIR](https://hapifhir.io), the Apache 2.0-licensed Java implementation of HL7 FHIR (>2,300 GitHub stars, 1,400+ forks). The codebase originated at University Health Network, has been developed for two decades, and is hosted at [github.com/hapifhir](https://github.com/hapifhir). Smile CDR is the commercial, hardened, enterprise-supported distribution built around HAPI FHIR.

| Repository | Purpose |
|---|---|
| [hapifhir/hapi-fhir](https://github.com/hapifhir/hapi-fhir) | Core Java FHIR library, client, and JPA server |
| [hapifhir/hapi-fhir-jpaserver-starter](https://github.com/hapifhir/hapi-fhir-jpaserver-starter) | Reference JPA server starter |
| [hapifhir/org.hl7.fhir.core](https://github.com/hapifhir/org.hl7.fhir.core) | Core FHIR standards library |
| [hapifhir/org.hl7.fhir.validator-wrapper](https://github.com/hapifhir/org.hl7.fhir.validator-wrapper) | FHIR Validator CLI, GUI, and server |
| [hapifhir/hapi-hl7v2](https://github.com/hapifhir/hapi-hl7v2) | HL7 v2 messaging library |
| [smilecdr/FHIR.ts](https://github.com/smilecdr/FHIR.ts) | TypeScript / JavaScript FHIR library (Apache 2.0) |

## Common Properties

- [Website — smiledigitalhealth.com](https://www.smiledigitalhealth.com)
- [Smile Omni](https://www.smiledigitalhealth.com/smile-omni)
- [OmniVera Health Data Platform](https://www.smiledigitalhealth.com/smilecdr)
- [OmniCompli CMS Suite](https://www.smiledigitalhealth.com/solution/cms-suite)
- [OmniQ Digital Quality Measures](https://www.smiledigitalhealth.com/solution/digital-quality-measures)
- [OmniConcierge Professional Services](https://www.smiledigitalhealth.com/solution/professional-services)
- [Documentation — Table of Contents](https://smilecdr.com/docs/welcome/table_of_contents.html)
- [Documentation — Installation](https://smilecdr.com/docs/installation/index.html)
- [Documentation — Security](https://smilecdr.com/docs/security/index.html)
- [Documentation — OpenAPI / Swagger](https://smilecdr.com/docs/fhir_repository/openapi_swagger.html)
- [Documentation — JSON Admin API](https://smilecdr.com/docs/json_admin_endpoints/json_admin_api.html)
- [HAPI FHIR — hapifhir.io](https://hapifhir.io)
- [GitHub — Smile Digital Health](https://github.com/smilecdr)
- [GitHub — HAPI FHIR](https://github.com/hapifhir)
- [Public HAPI FHIR test server](https://hapi.fhir.org)
- [LinkedIn](https://www.linkedin.com/company/smile-digital-health)
- [YouTube — @SmileCDR](https://www.youtube.com/@SmileCDR)
- [Twitter — @SmileDigiHealth](https://twitter.com/SmileDigiHealth)

## Deployment, Compliance, and Scale

- **Deployment:** On-premises, AWS, Azure, GCP, Kubernetes; supported databases include PostgreSQL, MySQL, MariaDB, Oracle, SQL Server, and MongoDB
- **Architecture:** MegaScale horizontal partitioning, 60–80 percent storage reduction via binary offloading
- **Certifications:** HITRUST v9.4, SOC 2 Type II, ISO 27001 / 27017 / 27018, ISO 13485, ONC 2015 Edition
- **Footprint:** 190+ global implementations; 30+ US payer deployments; 2B+ records transformed to FHIR; 255K+ transactions/second on reference benchmarks; 99.99 percent annual availability target
- **Pricing:** Commercial; not publicly listed — quoted per deployment and module footprint

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
