# Thoughtly (thoughtly)

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
