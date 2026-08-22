# Thoughtly (thoughtly)

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

Thoughtly is an AI voice and chat agent platform that helps revenue and support
teams contact every lead across every channel — voice, SMS, email, WhatsApp,
and iMessage. The product combines a no-code agent designer (decision-tree
builder, Vibes AI assistant, Genius knowledge base), a managed telephony layer
(purchased numbers, branded calling, BYOC, voice cloning), and a public REST
API for programmatically creating contacts, triggering outbound calls, and
subscribing to call-completion webhooks. Thoughtly integrates natively with
Salesforce, HubSpot, Zoho, GoHighLevel, Keap, Pipedrive, Attio, Calendly,
Acuity, Cal.com, Mindbody, Gmail, Slack, Zendesk, Shopify, Zapier, and Make.

**APIs.json:** [https://raw.githubusercontent.com/api-evangelist/thoughtly/refs/heads/main/apis.yml](https://raw.githubusercontent.com/api-evangelist/thoughtly/refs/heads/main/apis.yml)

## Scope

- **Type:** Index
- **Position:** Provider
- **Access:** 3rd-Party

## Tags

- Voice AI
- Chat AI
- Conversational AI
- AI Agents
- Outbound Calling
- Inbound Calling
- Lead Conversion
- SMS
- WhatsApp
- CRM
- Telephony

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Thoughtly API

Public REST API for the Thoughtly platform. Manage Agents (called
"interviews" in the API), create and update Contacts, trigger outbound
calls, search call responses, subscribe to webhook events
(NEW_RESPONSE, PHONE_TRANSFER, etc.), and trigger Webhook-driven
Automations. Authentication uses two headers: x-api-token and team_id.

- **Human URL:** [https://docs.thoughtly.com/developers](https://docs.thoughtly.com/developers)
- **Base URL:** `https://api.thoughtly.com`

#### Tags

- Voice AI
- Agents
- Contacts
- Calls
- Webhooks

#### Properties

- [Documentation](https://docs.thoughtly.com/developers)
- [Documentation](https://docs.thoughtly.com/api-reference)
- [OpenAPI](https://docs.thoughtly.com/api-reference/openapi.json) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [OpenAPI](openapi/thoughtly-api-openapi.yml) — [OpenAPI Specification](https://spec.openapis.org/oas/latest.html)
- [Postman Collection](collections/thoughtly-api.postman_collection.json) — [Postman Collection 2.1](https://schema.getpostman.com/json/collection/v2.1.0/collection.json)
- [Open Collection](collections/thoughtly-api.opencollection.json) — [Open Collection 1.0](https://schema.opencollection.com/opencollection/v1.0.0.json)
- [Spectral Rules](rules/thoughtly-rules.yml)
- [JSON Schema](json-schema/thoughtly-contact-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/thoughtly-agent-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/thoughtly-call-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Schema](json-schema/thoughtly-webhook-schema.json) — [JSON Schema](https://json-schema.org/specification)
- [JSON Structure](json-structure/thoughtly-contact-structure.json)
- [JSON Structure](json-structure/thoughtly-call-structure.json)
- [JSON-LD](json-ld/thoughtly-context.jsonld) — [JSON-LD](https://www.w3.org/TR/json-ld11/)
- [Examples](examples/thoughtly-create-contact-example.json)
- [Examples](examples/thoughtly-call-contact-example.json)
- [Examples](examples/thoughtly-subscribe-webhook-example.json)
- [Examples](examples/thoughtly-new-response-webhook-example.json)
- [Webhooks](https://docs.thoughtly.com/integrations/webhooks)
- [Documentation](https://docs.thoughtly.com/automations/getting-started)
- [Authentication](https://app.thoughtly.com/settings/developer)

## Common Properties

- [Website](https://thoughtly.com)
- [Portal](https://docs.thoughtly.com)
- [Documentation](https://docs.thoughtly.com/developers)
- [Documentation](https://docs.thoughtly.com/api-reference)
- [Getting Started](https://docs.thoughtly.com/getting-started/quick-start)
- [Sign Up](https://app.thoughtly.com/signup)
- [Login](https://app.thoughtly.com/login)
- [Authentication](https://app.thoughtly.com/settings/developer)
- [Pricing](https://docs.thoughtly.com/platform/billing)
- [Plans](plans/thoughtly-plans-pricing.yml)
- [Rate Limits](rate-limits/thoughtly-rate-limits.yml)
- [Fin Ops](finops/thoughtly-finops.yml)
- [Changelog](https://docs.thoughtly.com/support/changelog)
- [Support](https://docs.thoughtly.com/support/getting-help)
- [F A Q](https://docs.thoughtly.com/resources/faq)
- [Glossary](https://docs.thoughtly.com/resources/glossary/overview)
- [Whitepapers](https://docs.thoughtly.com/resources/whitepapers/overview)
- [Video Library](https://docs.thoughtly.com/resources/video-library)
- [Integrations](https://docs.thoughtly.com/integrations/getting-started)
- [Webhooks](https://docs.thoughtly.com/integrations/webhooks)
- [Automations](https://docs.thoughtly.com/automations/getting-started)
- [Knowledge Base](https://docs.thoughtly.com/genius/getting-started)
- [Agent Builder](https://docs.thoughtly.com/build/agent-builder/overview)
- [Phone Numbers](https://docs.thoughtly.com/phone-number/getting-started)
- [Voices](https://docs.thoughtly.com/agents/voices)
- [Blog Post](https://thoughtly.com/blog)
- [LinkedIn](https://www.linkedin.com/company/thoughtly-ai/)
- [Twitter](https://twitter.com/thoughtlyai)
- [Affiliate Program](https://docs.thoughtly.com/promptbooks/joining-the-thoughtly-affiliate-program)
- [Referral Program](https://docs.thoughtly.com/support/referral-program)
- [Promptbooks](https://docs.thoughtly.com/promptbooks/browse)
- [Vocabulary](vocabulary/thoughtly-vocabulary.yml)
- [Integration](https://docs.thoughtly.com/integrations/crm/salesforce)
- [Integration](https://docs.thoughtly.com/integrations/crm/hubspot)
- [Integration](https://docs.thoughtly.com/integrations/crm/zoho)
- [Integration](https://docs.thoughtly.com/integrations/crm/highlevel)
- [Integration](https://docs.thoughtly.com/integrations/crm/pipedrive)
- [Integration](https://docs.thoughtly.com/integrations/crm/attio)
- [Integration](https://docs.thoughtly.com/integrations/crm/keap)
- [Integration](https://docs.thoughtly.com/integrations/scheduling/calendly)
- [Integration](https://docs.thoughtly.com/integrations/scheduling/acuity)
- [Integration](https://docs.thoughtly.com/integrations/scheduling/cal-com)
- [Integration](https://docs.thoughtly.com/integrations/scheduling/mindbody)
- [Integration](https://docs.thoughtly.com/integrations/communication/gmail)
- [Integration](https://docs.thoughtly.com/integrations/communication/slack)
- [Integration](https://docs.thoughtly.com/integrations/communication/whatsapp-business)
- [Integration](https://docs.thoughtly.com/integrations/ticketing/zendesk)
- [Integration](https://docs.thoughtly.com/integrations/e-commerce/shopify)
- [Integration](https://docs.thoughtly.com/integrations/productivity/google-sheets)
- [Integration](https://docs.thoughtly.com/integrations/productivity/airtable)
- [Integration](https://docs.thoughtly.com/integrations/productivity/typeform)
- [Integration](https://docs.thoughtly.com/integrations/productivity/trello)
- [Integration](https://docs.thoughtly.com/integrations/productivity/smartsheet)
- [Integration](https://docs.thoughtly.com/integrations/productivity/zoom)
- [Integration](https://docs.thoughtly.com/integrations/automations/zapier)
- [Integration](https://docs.thoughtly.com/integrations/automations/make)
- [Features](undefined)

## Maintainers

**FN:** Kin Lane
**Email:** kin@apievangelist.com
**URL:** https://apievangelist.com
