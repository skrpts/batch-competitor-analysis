---
type: skill
id: competitor-profiling
title: Competitor Profiling
description: "Produces a structured competitive profile for a single competitor against consistent evaluation criteria"
tags: [Production, Competitive, Research]
connections:
  - target: llm-service
    type: runs_on
---

## Capability

Analyses a single competitor and produces a structured profile covering positioning, strengths, weaknesses, target market, pricing, and threat assessment. Designed to run inside a for_each loop so every competitor in a list receives the same depth of analysis.

## When to Use

- As the body step in a for_each loop iterating over competitors
- When you need consistent, comparable profiles across a set of competitors
- When each analysis should be independent (no cross-contamination between competitors)

## Evaluation Framework

1. **Identity** — company name, founding year, headquarters, team size, funding stage
2. **Positioning** — primary value proposition, tagline, market segment
3. **Product** — core features, key differentiators, platform/technology
4. **Target market** — company size, industry, buyer persona
5. **Pricing** — model (freemium/subscription/usage), starting price, enterprise tier
6. **Strengths** — what they do well, where they lead
7. **Weaknesses** — gaps, complaints, areas they underserve
8. **Threat level** — low/medium/high relative to your product, with reasoning

## Inputs

- Competitor name (from `{{loop.item}}`)
- Your product description (for relative positioning)
- Analysis focus areas (optional)

## Outputs

A structured markdown profile following the evaluation framework above. Consistent format across all competitors for easy comparison.
