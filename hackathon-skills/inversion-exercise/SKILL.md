---
name: inversion-exercise
description: Flip core assumptions to reveal hidden constraints and alternative approaches. This skill should be used when stuck on unquestioned assumptions, when feeling forced into "the only way" to do something, or when needing novel hackathon angles by asking "what if the opposite were true?"
---

# Inversion Exercise

Flip every assumption and see what still works. Sometimes the opposite reveals the truth.

**Core principle:** Inversion exposes hidden assumptions and alternative approaches.

## When to Use This Skill

- When stuck on unquestioned assumptions
- When feeling forced into "the only way" to do something
- When brainstorming contrarian hackathon ideas
- When every solution feels incremental, not breakthrough
- When judges have seen all the "obvious" approaches

## Quick Reference

| Normal Assumption | Inverted | What It Reveals |
|-------------------|----------|-----------------|
| Cache to reduce latency | Add latency to enable caching | Debouncing patterns |
| Pull data when needed | Push data before needed | Prefetching, eager loading |
| Handle errors when occur | Make errors impossible | Type systems, contracts |
| Build features users want | Remove features users don't need | Simplicity >> addition |
| Optimize for common case | Optimize for worst case | Resilience patterns |
| Users need bank accounts | No bank account required | Crypto wallets, prepaid instruments |
| Deliveries go to addresses | No fixed addresses needed | What3Words, dynamic pickup points |
| Patients visit hospitals | Hospitals visit patients | Telehealth, mobile clinics, IoT |
| Faster delivery is better | Strategic slowness saves money | Eco-delivery, carbon credits |
| Returns are a cost center | Returns are revenue | Mid-transit interception |

## Process

1. **List core assumptions** — What "must" be true in your domain?
2. **Invert each systematically** — "What if opposite were true?"
3. **Explore implications** — What would we do differently?
4. **Find valid inversions** — Which actually work somewhere?

## Instructions

When a user asks to invert assumptions:

1. **Extract domain assumptions** — Ask: "What are the 5 things everyone assumes must be true in [domain]?"
2. **Invert each one** — Create a table:

```markdown
| Assumption | Inverted | Implications | Valid? |
|-----------|----------|-------------|--------|
| [standard belief] | [opposite] | [what changes] | [yes/no + why] |
```

3. **Develop valid inversions** into full idea concepts
4. **Test boundaries** — Where does the inversion break?
5. **Extract the insight** — State what the inversion taught you

## Example

**Problem:** Users complain app is slow

**Normal approach:** Make everything faster (caching, optimization, CDN)

**Inverted:** Make things intentionally slower in some places
- Debounce search (add latency → enable better results)
- Rate limit requests (add friction → prevent abuse)
- Lazy load content (delay → reduce initial load)

**Insight:** Strategic slowness can improve UX

## Red Flags You Need This

- "There's only one way to do this"
- Forcing solution that feels wrong
- Can't articulate why approach is necessary
- "This is just how it's done"

## Remember

- Not all inversions work — test boundaries
- Valid inversions reveal context-dependence
- Sometimes the opposite IS the answer
- Question every "must be" statement
- The best hackathon ideas come from flipping what judges expect to hear
