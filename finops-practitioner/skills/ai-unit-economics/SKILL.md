---
name: ai-unit-economics
description: AI unit-economics discipline — auto-activates when evaluating whether AI spend is worth it, pushing from tokens and requests to cost-per-successful-outcome
---

You hold the unit-economics discipline for AI spend conversations. When the user is evaluating AI cost or value, apply these rules automatically.

## The core move

Tokens, requests, and monthly bills are inputs. The decision-grade number is **cost per successful task** — total workflow cost divided by outcomes that actually met the quality bar. Whenever a conversation stalls on "is this expensive?", reframe to "what does one good outcome cost, and what did it cost before AI?"

## Numerator discipline

The full cost of a successful task includes:
- The model calls that produced it — AND the retries and failed attempts along the way
- Guardrail, evaluation, and monitoring calls riding on the workflow
- The amortized slice of any subscription, credit pool, or reserved capacity it consumes
- Human review time where it's a structural part of the loop (note it even if unpriced)

## Denominator discipline

- Only outcomes that met the stated quality bar count as successes
- Outputs that needed substantial human rework are partial successes at best — pick a convention and keep it consistent
- If nobody has defined "successful," that's the first finding — propose a definition before optimizing anything

## Interpretation rules

- A missing retry/failure rate means the computed number is a FLOOR — always label it
- Cost-per-success comparisons across models are only valid at the same quality bar; a cheaper model that fails more is often more expensive per success
- Watch the denominator when costs "improve" — falling cost per task with falling task quality is a regression wearing a trend line
- Unit economics justify scale decisions; run-rate totals justify budget decisions — keep the two arguments separate

## The counterfactual

The strongest version of the analysis includes what the task cost before AI (labor minutes × loaded rate, vendor fee, or queue time). Without a counterfactual, cost-per-success describes the spend; with one, it justifies or kills it.
