# Thoughtly (thoughtly)

Thoughtly is an AI voice and chat agent platform that helps revenue and support teams contact every lead across every channel — voice, SMS, email, WhatsApp, and iMessage. The product combines a no-code agent designer (decision-tree builder, Vibes AI assistant, Genius knowledge base), a managed telephony layer (purchased numbers, branded calling, BYOC, voice cloning), and a public REST API for programmatically creating contacts, triggering outbound calls, and subscribing to call-completion webhooks.

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/thoughtly/refs/heads/main/apis.yml)

**Run:** [Capabilities Using Naftiko](https://github.com/naftiko/fleet?utm_source=api-evangelist&utm_medium=readme&utm_campaign=company-api-evangelist&utm_content=repo)

## Tags

- Voice AI, Chat AI, Conversational AI, AI Agents, Outbound Calling, Inbound Calling, Lead Conversion, SMS, WhatsApp, CRM, Telephony

## Timestamps

- **Created:** 2026-05-24
- **Modified:** 2026-05-24

## APIs

### Thoughtly API

Public REST API for the Thoughtly platform. Manage Agents (called "interviews" in the API), create and update Contacts, trigger outbound calls, search call responses, subscribe to webhook events (`NEW_RESPONSE`, `PHONE_TRANSFER`, etc.), and trigger Webhook-driven Automations. Authentication uses two headers: `x-api-token` and `team_id`, both available from [Developer Settings](https://app.thoughtly.com/settings/developer).

**Base URL:** `https://api.thoughtly.com`

**Human URL:** [https://docs.thoughtly.com/developers](https://docs.thoughtly.com/developers)

- [Documentation — Developers](https://docs.thoughtly.com/developers)
- [Documentation — API Reference](https://docs.thoughtly.com/api-reference)
- [OpenAPI (upstream)](https://docs.thoughtly.com/api-reference/openapi.json)
- [OpenAPI (this repo)](openapi/thoughtly-api-openapi.yml)
- [Spectral Rules](rules/thoughtly-rules.yml)
- [JSON Schema — Contact](json-schema/thoughtly-contact-schema.json)
- [JSON Schema — Agent](json-schema/thoughtly-agent-schema.json)
- [JSON Schema — Call](json-schema/thoughtly-call-schema.json)
- [JSON Schema — Webhook](json-schema/thoughtly-webhook-schema.json)
- [JSON Structure — Contact](json-structure/thoughtly-contact-structure.json)
- [JSON Structure — Call](json-structure/thoughtly-call-structure.json)
- [JSON-LD Context](json-ld/thoughtly-context.jsonld)
- [Example — Create Contact](examples/thoughtly-create-contact-example.json)
- [Example — Call A Contact](examples/thoughtly-call-contact-example.json)
- [Example — Subscribe Webhook](examples/thoughtly-subscribe-webhook-example.json)
- [Example — NEW_RESPONSE Webhook Payload](examples/thoughtly-new-response-webhook-example.json)
- [Naftiko Capability — Agents](capabilities/agents.yaml)
- [Naftiko Capability — Contacts](capabilities/contacts.yaml)
- [Naftiko Capability — Webhooks](capabilities/webhooks.yaml)

## Endpoints

| Method | Path | Operation |
|---|---|---|
| GET | `/interview` | Get Agents |
| GET | `/interview/{interview_id}/responses` | Search Calls |
| GET | `/contact` | Get Contacts |
| POST | `/contact/create` | Create Contact |
| GET | `/contact/{id}` | Get Contact |
| DELETE | `/contact/{id}` | Delete Contact |
| POST | `/contact/call` | Call A Contact |
| GET | `/user` | Get User Details |
| GET | `/webhooks` | Get Currently Active Webhooks |
| POST | `/webhooks/subscribe` | Subscribe To Webhook |
| DELETE | `/webhooks/unsubscribe` | Unsubscribe From Webhook |
| POST | `/webhook/automation/{automation_id}` | Trigger Automation With Webhook |

## Authentication

Every authenticated request requires two headers:

| Header | Purpose |
|---|---|
| `x-api-token` | API token from Developer Settings. |
| `team_id` | Team identifier scoping requests to a workspace. |

The single exception is `POST /webhook/automation/{automation_id}`, which is intentionally unauthenticated so external systems can trigger Webhook-driven Automations.

## Rate Limits

- **100 requests per minute** per API key across all endpoints.
- A `429 Too Many Requests` response indicates throttling — apply exponential backoff.
- Thoughtly does **not** auto-retry failed outgoing webhook deliveries; a 429 from a subscriber URL is retried once respecting `Retry-After`.

See [`rate-limits/thoughtly-rate-limits.yml`](rate-limits/thoughtly-rate-limits.yml).

## Webhook Events

| Event | Description |
|---|---|
| `NEW_RESPONSE` | A call has completed; payload includes call metadata, agent info, structured transcript, and custom fields. |
| `PHONE_TRANSFER` | A call has been transferred (warm or cold) to another number. |
| `FOLDER_NEW_RESPONSE` | New response within a specific folder. |
| `FOLDER_PHONE_TRANSFER` | Phone transfer within a specific folder. |
| `ACTION_FAILED` | An in-call action failed. |

## Plans and Pricing

| Plan | Price | Included | Notes |
|---|---|---|---|
| Free | $0 | 10 minutes/month, unlimited seats | 14-day full-feature trial. |
| Starter | ~$30/month | 300 minutes | Overage approx $0.09/minute voice. |
| Enterprise | Custom | Custom | SSO, audit log, BYOC, BYOK, branded calling. |
| AppSumo Lifetime | One-time | Credit-based | 10 credits/min voice, 8 credits/SMS, 500 credits/phone-number/month, 1 credit/automation-step, 3 credits/chat-test, 200 credits per $1 carrier fees. |

See [`plans/thoughtly-plans-pricing.yml`](plans/thoughtly-plans-pricing.yml) and [`finops/thoughtly-finops.yml`](finops/thoughtly-finops.yml).

## Native Integrations

**CRM:** Salesforce, HubSpot, Zoho CRM, GoHighLevel, Pipedrive, Attio, Keap, Fence Flow
**Scheduling:** Calendly, Acuity Scheduling, Cal.com, Mindbody, Zoho Bookings
**Communication:** Gmail, Slack, WhatsApp Business, iMessage/Lync
**Ticketing:** Zendesk
**E-commerce:** Shopify
**Productivity:** Google Sheets, Airtable, Typeform, Trello, Smartsheet, Zoom
**Automation Platforms:** Zapier, Make

Full integration index: [docs.thoughtly.com/integrations/getting-started](https://docs.thoughtly.com/integrations/getting-started).

## Resources

- **Pricing:** [docs.thoughtly.com/platform/billing](https://docs.thoughtly.com/platform/billing)
- **Changelog:** [docs.thoughtly.com/support/changelog](https://docs.thoughtly.com/support/changelog)
- **Support:** [docs.thoughtly.com/support/getting-help](https://docs.thoughtly.com/support/getting-help)
- **FAQ:** [docs.thoughtly.com/resources/faq](https://docs.thoughtly.com/resources/faq)
- **Glossary:** [docs.thoughtly.com/resources/glossary/overview](https://docs.thoughtly.com/resources/glossary/overview)
- **Promptbooks:** [docs.thoughtly.com/promptbooks/browse](https://docs.thoughtly.com/promptbooks/browse)
- **Whitepapers:** [docs.thoughtly.com/resources/whitepapers/overview](https://docs.thoughtly.com/resources/whitepapers/overview)
- **LinkedIn:** [linkedin.com/company/thoughtly-ai](https://www.linkedin.com/company/thoughtly-ai/)

## Maintainers

- Kin Lane — [apievangelist.com](https://apievangelist.com) — kin@apievangelist.com
