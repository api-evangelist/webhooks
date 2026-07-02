# Webhooks (webhooks)
An index and topic collection covering webhook delivery, ingestion, transformation, retry, and inspection APIs. Webhooks are the dominant HTTP pattern for asynchronous, event-driven integration between SaaS platforms — providers POST events to consumer endpoints, and consumers must reliably receive, verify, persist, and process those deliveries. This collection includes purpose-built webhook gateways like Hookdeck and ngrok, webhook inspection tools like Beeceptor and Webhook.site, durable event platforms like Inngest and Trigger.dev, automation hubs that expose webhook triggers (Zapier, n8n, Make, Pipedream, IFTTT, Integrately), cloud event buses (Amazon EventBridge, SNS, SQS, Azure Event Grid), and major webhook-emitting providers (Stripe, GitHub, Shopify, Twilio, SendGrid, Slack) whose webhook surfaces define the practices the rest of the ecosystem builds on.

**URL:** [https://apievangelist.com](https://apievangelist.com)

## Tags:

 - Webhooks, Event Delivery, Webhook Gateway, Webhook Inspection, Async Events

## Timestamps

- **Created:** 2026-05-19
- **Modified:** 2026-05-19

## Common Properties

- [Portal](https://apievangelist.com)
- [GitHubOrganization](https://github.com/api-evangelist)
- [JSONSchema - Webhook Endpoint Schema](https://raw.githubusercontent.com/api-evangelist/webhooks/refs/heads/main/json-schema/webhooks-webhook-endpoint-schema.json)
- [JSONSchema - Delivery Attempt Schema](https://raw.githubusercontent.com/api-evangelist/webhooks/refs/heads/main/json-schema/webhooks-delivery-attempt-schema.json)
- [JSON-LD](https://raw.githubusercontent.com/api-evangelist/webhooks/refs/heads/main/json-ld/webhooks-context.jsonld)
- [Vocabulary](https://raw.githubusercontent.com/api-evangelist/webhooks/refs/heads/main/vocabulary/webhooks-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Webhook Delivery and Retries | Webhook platforms reliably deliver event payloads from producer APIs to consumer endpoints, with automatic retries, exponential backoff, and dead-letter queues to handle transient consumer failures. |
| Signature Verification and Security | Webhook providers sign payloads with HMAC-SHA256, Ed25519, or asymmetric keys so consumers can verify authenticity, prevent replay attacks, and reject forged requests. |
| Webhook Inspection and Debugging | Tools like Beeceptor, Webhook.site, and ngrok give developers public URLs for local endpoints and human-readable logs of inbound webhook traffic for debugging and replay. |
| Webhook Gateways and Fan-Out | Gateway platforms like Hookdeck and Convoy sit between producers and consumers to centralize signing, filtering, transformation, fan-out to multiple destinations, and observability. |
| Event Filtering and Transformation | Webhook platforms let teams filter events by type or payload content, transform JSON payloads inline, and route the result to specific consumer endpoints or queues. |
| Local Tunneling for Development | Tunneling tools like ngrok and smee.io expose localhost endpoints to public URLs so developers can receive and debug real webhook traffic during local development. |
| Durable Event Workflows | Platforms like Inngest and Trigger.dev treat webhook deliveries as the entry point to durable, retryable, multi-step workflows with built-in scheduling, queues, and step-level retries. |

## Use Cases

| Name | Description |
|------|-------------|
| Receiving Stripe Payment Events | E-commerce and SaaS applications subscribe to Stripe webhook events to keep billing state in sync and trigger fulfillment. |
| GitHub CI/CD Automation | Engineering teams use GitHub webhook events (push, pull_request, release) to trigger CI/CD pipelines, ChatOps notifications, and security scanning. |
| Shopify Order Fan-Out | Merchants use webhook gateways to fan out Shopify order events to fulfillment, accounting, marketing, and analytics consumers with per-destination retry isolation. |
| Local Webhook Development with Tunnels | Developers use ngrok or smee.io to receive production-style webhook traffic on localhost during integration development. |
| Webhook Observability and Replay | Operations teams use webhook gateways and inspection tools to monitor delivery success, alert on failures, and replay missed deliveries from history. |
| No-Code Webhook Automation | Business users use Zapier, Make, n8n, IFTTT, and Pipedream to wire webhook events from one SaaS app into actions in another without writing code. |
| Event-Driven Cloud Fan-Out | Cloud teams use Amazon EventBridge, SNS, and SQS to fan webhook deliveries out to multiple subscribers with at-least-once delivery guarantees. |

## Integrations

| Name | Description |
|------|-------------|
| Hookdeck | Webhook gateway that ingests, verifies, persists, filters, transforms, and reliably delivers webhook events with retry, replay, and observability. |
| ngrok | Secure tunneling and ingress platform widely used to expose local webhook endpoints to public URLs for development and debugging. |
| Beeceptor | Webhook inspection and mocking platform providing instant public endpoints to capture, inspect, and mock inbound HTTP and webhook traffic. |
| Inngest | Durable event-driven platform that receives webhook events and runs them through retryable, multi-step workflow functions. |
| Trigger.dev | Developer-first background jobs and workflows platform with first-class webhook triggers, retries, and long-running execution. |
| Stripe | Payments platform whose webhook event model defines best practice for the broader webhook ecosystem. |
| GitHub | Source control platform emitting webhook events for repository, issue, PR, release, and CI/CD activity. |
| Amazon EventBridge | Serverless event bus that ingests events from AWS services, SaaS partners, and custom applications and fans them out to targets including webhook endpoints. |

## Artifacts

Machine-readable artifacts describing webhook endpoints, events, deliveries, and signing — organized by format.

### JSON Schema

- [Webhook Endpoint Schema](json-schema/webhooks-webhook-endpoint-schema.json)
- [Delivery Attempt Schema](json-schema/webhooks-delivery-attempt-schema.json)

### JSON Structure

- [Webhook Endpoint Structure](json-structure/webhooks-webhook-endpoint-structure.json)
- [Delivery Attempt Structure](json-structure/webhooks-delivery-attempt-structure.json)

### JSON-LD

- [Webhooks Context](json-ld/webhooks-context.jsonld)

## Vocabulary

- [Webhooks Vocabulary](vocabulary/webhooks-vocabulary.yaml) — Unified taxonomy of webhook endpoints, events, deliveries, signing configs, workflows, and personas across gateways, inspection tools, automation hubs, and event-emitting platforms.

## Network

This index references the following webhook tooling and webhook-emitting platform repositories:

- [Amazon EventBridge](https://github.com/api-evangelist/amazon-eventbridge)
- [Amazon SNS](https://github.com/api-evangelist/amazon-sns)
- [Amazon SQS](https://github.com/api-evangelist/amazon-sqs)
- [Azure Event Grid](https://github.com/api-evangelist/azure-event-grid)
- [Beeceptor](https://github.com/api-evangelist/beeceptor)
- [Cloudflare](https://github.com/api-evangelist/cloudflare)
- [GitHub](https://github.com/api-evangelist/github)
- [Hookdeck](https://github.com/api-evangelist/hookdeck)
- [IFTTT](https://github.com/api-evangelist/ifttt)
- [Inngest](https://github.com/api-evangelist/inngest)
- [Integrately](https://github.com/api-evangelist/integrately)
- [Make](https://github.com/api-evangelist/make)
- [n8n](https://github.com/api-evangelist/n8n)
- [ngrok](https://github.com/api-evangelist/ngrok)
- [Pipedream](https://github.com/api-evangelist/pipedream)
- [Postman](https://github.com/api-evangelist/postman)
- [Relay](https://github.com/api-evangelist/relay-app)
- [SendGrid](https://github.com/api-evangelist/sendgrid)
- [Shopify](https://github.com/api-evangelist/shopify)
- [Slack](https://github.com/api-evangelist/slack)
- [Splunk](https://github.com/api-evangelist/splunk)
- [Stripe](https://github.com/api-evangelist/stripe)
- [Tray.io](https://github.com/api-evangelist/tray-io)
- [Trigger.dev](https://github.com/api-evangelist/trigger-dev)
- [Twilio](https://github.com/api-evangelist/twilio)
- [Workato](https://github.com/api-evangelist/workato)
- [Zapier](https://github.com/api-evangelist/zapier)

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
