---
name: simplification-cascades
description: Find one insight that eliminates multiple components at once. This skill should be used when complexity is spiraling, when implementing the same concept multiple ways, or when accumulating special cases. It reveals "everything is a special case of..." moments that collapse complexity dramatically.
---

# Simplification Cascades

Sometimes one insight eliminates 10 things. Look for the unifying principle that makes multiple components unnecessary.

**Core principle:** "Everything is a special case of..." collapses complexity dramatically.

## When to Use This Skill

- When implementing the same concept multiple ways
- When accumulating special cases and if/else chains
- When complexity is spiraling during hackathon development
- When you need to cut scope without losing value
- When building an MVP and need to find the elegant core

## Quick Reference

| Symptom | Likely Cascade |
|---------|----------------|
| Same thing implemented 5+ ways | Abstract the common pattern |
| Growing special case list | Find the general case |
| Complex rules with exceptions | Find the rule with no exceptions |
| Excessive config options | Find defaults that work for 95% |

## Process

1. **List the variations** — What's implemented multiple ways?
2. **Find the essence** — What's the same underneath?
3. **Extract abstraction** — What's the domain-independent pattern?
4. **Test it** — Do all cases fit cleanly?
5. **Measure cascade** — How many things become unnecessary?

## Instructions

When a user is dealing with growing complexity:

1. **Identify the variations** — Ask: "What are you building multiple versions of?"
2. **Look for the common pattern:**

```markdown
**Before:**
- System A: [handles case 1]
- System B: [handles case 2]
- System C: [handles case 3]
- System D: [handles case 4]

**Insight:** "All are just [common abstraction] with [variation point]"

**After:** One [abstraction] engine with 4 [types]

**Eliminated:** [N] separate implementations → 1 unified system
```

3. **Validate** — Does every case fit the abstraction cleanly? If not, the cascade is forced.
4. **Measure** — Count what you can delete. Real cascades eliminate 3+ things.

## Examples

### Logistics Cascade
- **Before:** Separate tracking for packages, vehicles, warehouses, drivers
- **Insight:** "All are just entities with location, status, and events"
- **After:** One `TrackableEntity` system with entity types
- **Eliminated:** 4 tracking implementations → 1 universal tracker

### Fintech Cascade
- **Before:** Separate modules for loans, insurance, investments, payments
- **Insight:** "All are just financial contracts with terms, parties, and triggers"
- **After:** One `FinancialContract` engine with 4 contract types
- **Eliminated:** 4 codebases → 1 unified engine

### Healthcare Cascade
- **Before:** Separate flows for appointments, prescriptions, lab orders, referrals
- **Insight:** "All are just clinical requests with a requester, provider, and outcome"
- **After:** One `ClinicalRequest` pipeline
- **Eliminated:** 4 workflow engines → 1 unified pipeline

## Red Flags You're Missing a Cascade

- "We just need to add one more case..." (repeating forever)
- "These are all similar but different" (maybe they're the same?)
- Refactoring feels like whack-a-mole
- Growing configuration file
- "Don't touch that, it's complicated"

## Remember

- Simplification cascades = 10x wins, not 10% improvements
- One powerful abstraction > ten clever hacks
- Hackathon judges love elegant simplicity over feature bloat
- Measure in "how many things can we delete?"
- The pattern is usually already there — just needs recognition
