---
type: skill
id: strategic-recommendation
title: Strategic Recommendation
description: "Produces actionable competitive strategy recommendations based on the comparative analysis"
tags: [Production, Competitive, Strategy]
connections:
  - target: llm-service
    type: runs_on
---

## Capability

Reads a comparative competitive analysis and produces prioritised strategic recommendations. Focuses on three action categories: where to differentiate, where to defend, and where to invest.

## When to Use

- As the final step after competitive consolidation
- When analysis needs to translate into concrete decisions
- When stakeholders need a clear "so what?" from competitive research

## Recommendation Framework

1. **Differentiate** — areas where your product can establish a unique position that no competitor occupies. These are your biggest opportunities.
2. **Defend** — areas where competitors are strong and you risk losing ground. These need attention to maintain your current position.
3. **Invest** — capabilities or markets where no competitor is strong yet. These are bets on future positioning.

Each recommendation includes: the specific action, the competitive rationale, the expected impact (high/medium/low), and the timeframe (immediate/quarter/year).

## Inputs

- Comparative analysis matrix
- Your product description and current positioning

## Outputs

A prioritised list of strategic recommendations, grouped by action category, with rationale and impact assessment for each.
