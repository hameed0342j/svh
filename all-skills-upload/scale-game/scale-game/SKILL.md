---
name: scale-game
description: Test ideas and architectures at extreme scales (1000x bigger/smaller, instant/year-long) to expose fundamental truths hidden at normal scales. This skill should be used when uncertain about scalability, when edge cases are unclear, or when validating architecture for production volumes.
---

# Scale Game

Test your approach at extreme scales to find what breaks and what surprisingly survives.

**Core principle:** Extremes expose fundamental truths hidden at normal scales.

## When to Use This Skill

- When uncertain about scalability of a solution
- When edge cases are unclear
- When validating architecture for production volumes
- When preparing a hackathon pitch that needs a scalability story
- When a judge might ask "but will this work at scale?"

## Quick Reference

| Scale Dimension | Test At Extremes | What It Reveals |
|-----------------|------------------|-----------------|
| Volume | 1 item vs 1B items | Algorithmic complexity limits |
| Speed | Instant vs 1 year | Async requirements, caching needs |
| Users | 1 user vs 1B users | Concurrency issues, resource limits |
| Duration | Milliseconds vs years | Memory leaks, state growth |
| Failure rate | Never fails vs always fails | Error handling adequacy |
| Geography | 1 city vs 195 countries | Regulatory, latency, localization |
| Data sources | 1 API vs 1000 APIs | Integration architecture |

## Process

1. **Pick dimension** — What could vary extremely?
2. **Test minimum** — What if this was 1000x smaller/faster/fewer?
3. **Test maximum** — What if this was 1000x bigger/slower/more?
4. **Note what breaks** — Where do limits appear?
5. **Note what survives** — What's fundamentally sound?

## Instructions

When a user asks to stress-test an idea at scale:

1. **Identify the idea's core dimensions** — What variables could change?
2. **Create a scale table:**

```markdown
| Scale | At 1x | At 1000x | What Breaks | Design Response |
|-------|-------|----------|-------------|-----------------|
| [Dim] | [Normal] | [Extreme] | [Failure] | [Architecture fix] |
```

3. **Test both directions** — Bigger AND smaller
4. **Extract design implications** — Each "what breaks" becomes a design decision
5. **Summarize architectural requirements** revealed by the scale test

## Examples

### Logistics Scale Test
| Scale | Normal | At 1B Scale | Design Implication |
|-------|--------|-------------|-------------------|
| Packages/day | 1,000 | 1,000,000,000 | Distributed routing, edge computing |
| Delivery zones | 1 city | Global | Federated logistics network |
| Vehicle types | Trucks | Drones, robots, ships | Abstract transport interface |
| Data sources | GPS only | GPS + weather + traffic + social | Event-driven data pipeline |

### Fintech Scale Test
| Scale | Normal | At 1B Scale | Design Implication |
|-------|--------|-------------|-------------------|
| Transactions/sec | 100 | 100,000,000 | Event-driven, CQRS pattern |
| Currencies | 1 (INR) | 180 currencies | Multi-currency ledger from day 1 |
| Regulators | 1 (RBI) | 50+ global | Pluggable compliance engine |

## Red Flags You Need This

- "It works in dev" (but will it work in production?)
- No idea where limits are
- "Should scale fine" (without testing)
- Surprised by production behavior

## Remember

- Extremes reveal fundamentals
- What works at one scale fails at another
- Test both directions (bigger AND smaller)
- Use insights to validate architecture early
- Judges LOVE scalability stories — "we tested at 1B and our architecture holds"
