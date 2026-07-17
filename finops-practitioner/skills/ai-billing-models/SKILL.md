---
name: ai-billing-models
description: AI vendor billing-model fluency — auto-activates when normalizing, comparing, or forecasting AI spend across seats, usage, credits, and reserved capacity
---

You have deep fluency in how AI products bill. When the user is working on AI spend tasks, apply this knowledge automatically.

## The billing shapes

- **Per-seat subscription** — flat monthly/annual per user (chat assistants, copilots, embedded AI tiers). The waste mode is inactive seats; the control is seat-to-active-user reconciliation on a cadence
- **Usage-based API** — metered per token, request, image, or minute, usually with different input/output rates and per-model pricing. The waste modes are retries, oversized prompts/contexts, and defaulting to a bigger model than the task needs
- **Prepaid credits** — money in, credits out, often with expiry and sometimes with bonus tiers. The waste modes are expiry (breakage) and the false comfort of "already paid" masking a rising run rate
- **Reserved / provisioned capacity** — committed throughput (e.g., provisioned units) billed whether used or not. The waste mode is committing to peak instead of base load; the control is utilization tracking against the commitment
- **Hybrid** — seat + usage overage, platform fee + credits, or an enterprise minimum with drawdown. Read the invoice's fixed and variable parts separately or the normalization will be wrong
- **Embedded AI** — AI features priced inside a non-AI product (CRM tiers, office suites, support desks). Frequently invisible in an "AI spend" search because the line item doesn't say AI

## Normalization rules

- Amortize annual prepay to monthly (÷12) and SAY it's amortized — cash timing and run rate are different questions
- Convert credit purchases to run rate from actual burn (credits used per month × price per credit), not from the purchase amount
- Count reserved capacity at commitment, with a utilization percentage alongside — 40% utilization of a committed pool is the finding, not a lower cost
- Keep one currency and one period; label estimates as estimates every time

## Contract mechanics worth flagging

- Auto-renewal windows and notice periods (the negotiation clock starts at notice-minus-30, not at renewal)
- True-up clauses on seat growth; whether unused seats true DOWN
- Credit rollover and expiry terms
- Rate-lock or price-protection language, and what happens to grandfathered pricing at renewal

Always distinguish run-rate math (FinOps working numbers) from accounting treatment (the controller's domain) — never present the former as the latter.
