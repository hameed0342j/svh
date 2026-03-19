# 🧠 Comprehensive Hackathon Skills — Fintech / Logistics / Healthcare

> **Purpose:** A unified skills reference for generating **scalable, feasible, novel solutions** for hackathons across Fintech, Logistics, and Healthcare domains. Curated from `superpowers-skills` and `awesome-claude-skills` repositories.

> [!TIP]
> **How to Use:** Load this file at the start of any ideation session. Apply skills sequentially: **Brainstorm → Analyze → Research → Architect → Plan.** Each skill includes domain-specific examples.

---

## Table of Contents

1. [Section 1: Ideation & Brainstorming](#section-1-ideation--brainstorming)
2. [Section 2: Problem Analysis & Scalability](#section-2-problem-analysis--scalability)
3. [Section 3: Research & Domain Knowledge](#section-3-research--domain-knowledge)
4. [Section 4: Architecture & Design](#section-4-architecture--design)
5. [Section 5: Hackathon Domain Framework](#section-5-hackathon-domain-framework)

---

# Section 1: Ideation & Brainstorming

---

## Skill 1: brainstorming-ideas-into-designs

```yaml
name: brainstorming-ideas-into-designs
description: Interactive idea refinement using Socratic method to develop fully-formed designs from rough concepts
when_to_use: When you have a rough hackathon idea and need to transform it into a structured, validated design before building
```

### Overview
Transform rough ideas into fully-formed designs through structured questioning and alternative exploration.

**Core principle:** Ask questions to understand, explore alternatives, present design incrementally for validation.

### The Process

#### Phase 1: Understanding
- Clarify the problem statement within the chosen domain
- Ask ONE question at a time: Purpose, constraints, success criteria
- Identify target users and pain points

#### Phase 2: Exploration
- Propose 2-3 different approaches
- For each: Core architecture, trade-offs, complexity assessment
- Evaluate which approach resonates with hackathon constraints (time, team size, demo-ability)

#### Phase 3: Design Presentation
- Present in 200-300 word sections
- Cover: Architecture, components, data flow, error handling
- Validate after each section: "Does this look right so far?"

#### Phase 4: Planning Handoff
- Create implementation plan with bite-sized tasks
- Assign tasks based on team strengths

### Hackathon Application

| Domain | Example Prompt | Expected Output |
|--------|---------------|-----------------|
| **Fintech** | "I want to build a micro-lending platform for gig workers" | 3 architectural approaches with trade-offs for demo feasibility |
| **Logistics** | "Real-time fleet optimization using crowd-sourced data" | User flow, data pipeline design, MVP scope definition |
| **Healthcare** | "AI triage system for rural clinics with low connectivity" | Offline-first architecture, data sync strategy, privacy design |

### Remember
- One question per message during understanding
- Apply YAGNI ruthlessly — hackathon = MVP, not full product
- Explore 2-3 alternatives before settling
- Present incrementally, validate as you go
- Go backward when needed — flexibility > rigid progression

---

## Skill 2: collision-zone-thinking

```yaml
name: collision-zone-thinking
description: Force unrelated concepts together to discover emergent properties — "What if we treated X like Y?"
when_to_use: When conventional approaches feel inadequate and you need breakthrough innovation by forcing unrelated concepts together
```

### Overview
Revolutionary insights come from forcing unrelated concepts to collide. Treat X like Y and see what emerges.

**Core principle:** Deliberate metaphor-mixing generates novel solutions.

### Quick Reference

| Stuck On | Try Treating As | Might Discover |
|----------|-----------------|----------------|
| Payment processing | Immune system | Fraud detection as antibodies, adaptive learning |
| Supply chain tracking | Nervous system | Real-time signals, reflex responses to disruption |
| Patient data | Water flow | Streaming health data, data lakes for population health |
| Credit scoring | DNA sequencing | Behavioral genome, mutation-based risk patterns |
| Last-mile delivery | Ant colony | Swarm optimization, pheromone-trail routing |

### Process
1. **Pick two unrelated concepts** from different domains
2. **Force combination**: "What if we treated [A] like [B]?"
3. **Explore emergent properties**: What new capabilities appear?
4. **Test boundaries**: Where does the metaphor break?
5. **Extract insight**: What did we learn?

### Hackathon Collision Examples

#### Fintech × Biology
**Collision:** "What if we treated financial transactions like a circulatory system?"
- **Emergent:** Blood cells = micro-transactions flowing through arteries = payment rails
- **Insight:** Detect "financial clots" (fraud clusters) using cardiovascular diagnostics
- **Novel Solution:** Real-time transaction health monitoring dashboard

#### Logistics × Game Theory
**Collision:** "What if we treated warehouse allocation like a multiplayer strategy game?"
- **Emergent:** Warehouses compete for optimal inventory, AI referee balances supply
- **Insight:** Nash equilibrium for multi-warehouse optimization
- **Novel Solution:** Gamified logistics optimization engine

#### Healthcare × Blockchain
**Collision:** "What if we treated patient consent like a smart contract?"
- **Emergent:** Self-executing consent with automatic data access/revocation
- **Insight:** Patients control data granularly, audit trail is immutable
- **Novel Solution:** Decentralized consent management platform

### Remember
- Wild combinations often yield best insights
- Test metaphor boundaries rigorously
- Best source domains: physics, biology, economics, psychology, game theory
- Document even failed collisions — they teach

---

## Skill 3: inversion-exercise

```yaml
name: inversion-exercise
description: Flip core assumptions to reveal hidden constraints and alternative approaches — "what if the opposite were true?"
when_to_use: When stuck on unquestioned assumptions or feeling forced into "the only way" to do something
```

### Overview
Flip every assumption and see what still works. Sometimes the opposite reveals the truth.

**Core principle:** Inversion exposes hidden assumptions and alternative approaches.

### Quick Reference

| Normal Assumption | Inverted | What It Reveals |
|-------------------|----------|-----------------|
| Users need a bank account | What if no bank account is required? | Crypto wallets, prepaid instruments |
| Deliveries must go to addresses | What if there were no fixed addresses? | What3Words, dynamic pickup points |
| Patients visit hospitals | What if hospitals visit patients? | Tele-health, mobile clinics, IoT monitoring |
| Credit needs history | What if we ignore history? | Real-time behavioral scoring |
| Inventory must be pre-stocked | What if inventory arrives on-demand? | Just-in-time micro-fulfillment |

### Process
1. **List core assumptions** — What "must" be true in your domain?
2. **Invert each systematically** — "What if opposite were true?"
3. **Explore implications** — What would we do differently?
4. **Find valid inversions** — Which actually work somewhere?

### Hackathon Inversion Examples

#### Fintech
- **Assumption:** "Users should save money" → **Inverted:** "What if spending IS saving?"
- **Solution:** Round-up micro-investment app that treats every purchase as an investment trigger

#### Logistics
- **Assumption:** "Faster delivery is always better" → **Inverted:** "What if slower delivery saves money and the planet?"
- **Solution:** Eco-delivery option with carbon credits and discounts for patient customers

#### Healthcare
- **Assumption:** "Diagnosis requires a doctor" → **Inverted:** "What if the patient self-diagnoses accurately?"
- **Solution:** AI-guided symptom checker with medical-grade accuracy and escalation protocols

### Remember
- Not all inversions work — test boundaries
- Valid inversions reveal context-dependence
- Sometimes the opposite IS the answer
- Question every "must be" statement

---

# Section 2: Problem Analysis & Scalability

---

## Skill 4: scale-game

```yaml
name: scale-game
description: Test at extremes (1000x bigger/smaller, instant/year-long) to expose fundamental truths hidden at normal scales
when_to_use: When uncertain about scalability, edge cases unclear, or validating architecture for production volumes
```

### Overview
Test your approach at extreme scales to find what breaks and what surprisingly survives.

**Core principle:** Extremes expose fundamental truths hidden at normal scales.

### Quick Reference

| Scale Dimension | Test At Extremes | What It Reveals |
|-----------------|------------------|-----------------|
| Volume | 1 transaction vs 1B transactions | Database bottlenecks, queue overflow |
| Speed | Instant settlement vs 1-year settlement | Async requirements, caching needs |
| Users | 1 user vs 1B users | Concurrency, resource limits |
| Geography | 1 city vs 195 countries | Regulatory compliance, latency |
| Failure rate | Never fails vs always fails | Error handling, resilience |

### Process
1. **Pick dimension** — What could vary extremely in your hackathon demo?
2. **Test minimum** — What if this was 1000x smaller/faster/fewer?
3. **Test maximum** — What if this was 1000x bigger/slower/more?
4. **Note what breaks** — Where do limits appear?
5. **Note what survives** — What's fundamentally sound?

### Hackathon Scale Tests

#### Fintech
| Scale | Normal | At 1B Scale | Design Implication |
|-------|--------|-------------|-------------------|
| Transactions/sec | 100 | 100,000,000 | Event-driven architecture, CQRS |
| Currencies | 1 (INR) | 180 currencies | Multi-currency ledger from day 1 |
| Regulatory bodies | 1 (RBI) | 50+ global regulators | Pluggable compliance engine |

#### Logistics
| Scale | Normal | At 1B Scale | Design Implication |
|-------|--------|-------------|-------------------|
| Packages/day | 1,000 | 1,000,000,000 | Distributed routing, edge computing |
| Delivery zones | 1 city | Global | Federated logistics network |
| Vehicle types | Trucks | Drones, robots, ships | Abstract transport interface |

#### Healthcare
| Scale | Normal | At 1B Scale | Design Implication |
|-------|--------|-------------|-------------------|
| Patient records | 10,000 | 10,000,000,000 | Sharded health data, FHIR compliance |
| Concurrent diagnoses | 10 | 10,000,000 | Async AI inference, edge processing |
| Data sources | Hospital EMR | Wearables + IoT + genomics | Universal health data adapter |

### Remember
- Extremes reveal fundamentals
- What works at one scale fails at another
- Test both directions (bigger AND smaller)
- Use insights to validate architecture early — judges LOVE scalability stories

---

## Skill 5: simplification-cascades

```yaml
name: simplification-cascades
description: Find one insight that eliminates multiple components — "if this is true, we don't need X, Y, or Z"
when_to_use: When implementing the same concept multiple ways, accumulating special cases, or complexity is spiraling
```

### Overview
Sometimes one insight eliminates 10 things. Look for the unifying principle that makes multiple components unnecessary.

**Core principle:** "Everything is a special case of..." collapses complexity dramatically.

### Quick Reference

| Symptom | Likely Cascade |
|---------|----------------|
| Same thing implemented 5+ ways | Abstract the common pattern |
| Growing special case list | Find the general case |
| Complex rules with exceptions | Find the rule that has no exceptions |
| Excessive config options | Find defaults that work for 95% |

### Hackathon Simplification Examples

#### Fintech
- **Before:** Separate modules for loans, insurance, investments, payments
- **Insight:** "All are just financial contracts with terms, parties, and triggers"
- **After:** One `FinancialContract` engine with 4 contract types
- **Eliminated:** 4 separate codebases → 1 unified engine

#### Logistics
- **Before:** Separate tracking for packages, vehicles, warehouses, drivers
- **Insight:** "All are just entities with location, status, and events"
- **After:** One `TrackableEntity` system with entity types
- **Eliminated:** 4 tracking implementations → 1 universal tracker

#### Healthcare
- **Before:** Separate flows for appointments, prescriptions, lab orders, referrals
- **Insight:** "All are just clinical requests with a requester, provider, and outcome"
- **After:** One `ClinicalRequest` pipeline
- **Eliminated:** 4 workflow engines → 1 unified pipeline

### Process
1. **List the variations** — What's implemented multiple ways?
2. **Find the essence** — What's the same underneath?
3. **Extract abstraction** — What's the domain-independent pattern?
4. **Test it** — Do all cases fit cleanly?
5. **Measure cascade** — How many things become unnecessary?

### Remember
- Simplification cascades = 10x wins, not 10% improvements
- One powerful abstraction > ten clever hacks
- Hackathon judges love elegant simplicity over feature bloat
- Measure in "how many things can we delete?"

---

## Skill 6: meta-pattern-recognition

```yaml
name: meta-pattern-recognition
description: Spot patterns appearing in 3+ domains to find universal principles that can be applied to your hackathon domain
when_to_use: When noticing the same pattern across 3+ different domains or experiencing déjà vu in problem-solving
```

### Overview
When the same pattern appears in 3+ domains, it's probably a universal principle worth extracting.

**Core principle:** Find patterns in how patterns emerge.

### Cross-Domain Pattern Table

| Pattern | In Fintech | In Logistics | In Healthcare | Abstract Form |
|---------|-----------|-------------|--------------|---------------|
| **Scoring** | Credit score | Delivery reliability score | Patient risk score | Entity reputation engine |
| **Matching** | Lender-borrower match | Driver-package match | Doctor-patient match | Two-sided marketplace |
| **Streaming** | Transaction stream | Location stream | Vital signs stream | Real-time event pipeline |
| **Pooling** | Investment pools | Vehicle pools | Organ donor pools | Resource pooling with fairness |
| **Queuing** | Payment queue | Delivery queue | Appointment queue | Priority queue with SLAs |

### Process
1. **Spot repetition** — See same shape in 3+ places
2. **Extract abstract form** — Describe independent of any domain
3. **Identify variations** — How does it adapt per domain?
4. **Check applicability** — Where else might this help?

### Hackathon Power Move
**Build the abstract pattern, then demo it in your chosen domain.** Tell judges: "This same engine works across Fintech, Logistics, and Healthcare — we built the universal version."

### Remember
- 3+ domains = likely universal principle
- Abstract form reveals new applications
- Universal patterns are battle-tested
- Judges love cross-domain applicability

---

## Skill 7: when-stuck-problem-solving-dispatch

```yaml
name: when-stuck-problem-solving-dispatch
description: Dispatch to the right problem-solving technique based on how you're stuck
when_to_use: When stuck during hackathon and unsure which technique to apply
```

### Quick Dispatch

| How You're Stuck | Use This Skill |
|------------------|----------------|
| **Complexity spiraling** — Same thing 5+ ways | → simplification-cascades |
| **Need innovation** — Conventional solutions inadequate | → collision-zone-thinking |
| **Recurring patterns** — Same issue different places | → meta-pattern-recognition |
| **Forced by assumptions** — "Must be done this way" | → inversion-exercise |
| **Scale uncertainty** — Will it work in production? | → scale-game |
| **Multiple valid approaches** — Can't decide | → preserving-productive-tensions |

### Combining Techniques
- **Simplification + Meta-pattern**: Find pattern, then simplify all instances
- **Collision + Inversion**: Force metaphor, then invert its assumptions
- **Scale + Simplification**: Extremes reveal what to eliminate

---

# Section 3: Research & Domain Knowledge

---

## Skill 8: tracing-knowledge-lineages

```yaml
name: tracing-knowledge-lineages
description: Understand how ideas evolved over time to find old solutions for new problems and avoid repeating past failures
when_to_use: When evaluating existing solutions in Fintech/Logistics/Healthcare, or when "new" ideas might be revivals
```

### Overview
Ideas have history. Understanding why we arrived at current approaches prevents repeating failures and rediscovers abandoned solutions.

**Core principle:** Before judging current approaches or proposing "new" ones, trace their lineage.

### Hackathon Application

#### Trace Before Proposing
When pitching a "novel" solution, check:
1. **Has this been tried before?** (Failed startups, abandoned features)
2. **Why did it fail then?** (Technology limits? Regulation? Timing?)
3. **What's different NOW?** (AI advancement? New APIs? Changed regulations?)

#### Domain Lineage Examples

| "New" Idea | Historical Precedent | Why It Died | What Changed |
|-----------|---------------------|-------------|-------------|
| AI credit scoring | Expert systems (1990s) | Too rigid, no data | ML + massive data + cloud compute |
| Drone delivery | Pneumatic tubes (1900s) | Infrastructure cost | Autonomous tech + GPS + lightweight drones |
| Telemedicine | Phone consultations (1960s) | No visual, no data sharing | Video calls + IoT vitals + EHR integration |
| Blockchain payments | DigiCash (1990s) | No smartphone, no internet mass adoption | Mobile-first, crypto infrastructure |
| Crowd-sourced logistics | Hitchhiking culture | Safety, trust | Rating systems, real-time tracking, insurance |

### Document Your Lineage for Judges
```markdown
## Why NOW — Our Solution's Timing Advantage

**Previous attempts:** [What was tried before]
**Why they failed:** [Root cause, not symptoms]
**What changed:** [Technology/regulation/behavior shift]
**Our insight:** [What we do differently because we learned from history]
```

### Remember
- Current approaches exist for reasons — trace those reasons
- Past failures might work now — context changes
- "New" approaches might be revivals — check precedents
- Judges respect founders who know the history of their space

---

## Skill 9: content-research-writer

```yaml
name: content-research-writer
description: Assists in conducting research, structuring content, adding citations, and creating polished presentations and documentation
when_to_use: When preparing hackathon presentations, writing project documentation, or researching domain-specific problems
```

### Overview
Your research and writing partner for hackathon deliverables — presentations, documentation, and pitch decks.

### Hackathon Workflow

1. **Research the problem space**
   - Find current market data and statistics for your domain
   - Identify existing solutions and their gaps
   - Gather evidence for your "why now" argument

2. **Structure the presentation**
   ```
   Hook → Problem → Solution → Demo → Business Model → Team → Ask
   ```

3. **Add citations and data**
   - Market size numbers with sources
   - Pain point statistics
   - Competitor landscape data

4. **Polish the pitch**
   - Strong hook (data-driven, story, or question)
   - Clear value proposition
   - Compelling demo narrative

### Domain Research Targets

| Domain | Research Areas | Key Data Sources |
|--------|--------------|-----------------|
| **Fintech** | Unbanked population, digital payment growth, regulatory landscape | RBI reports, World Bank, PwC surveys |
| **Logistics** | Last-mile cost, delivery failure rates, carbon footprint | McKinsey logistics reports, industry whitepapers |
| **Healthcare** | Doctor-patient ratio, rural healthcare gaps, digital health adoption | WHO data, NITI Aayog, health ministry reports |

---

## Skill 10: lead-research-assistant

```yaml
name: lead-research-assistant
description: Identifies target users, market opportunities, and competitive landscape for your hackathon solution
when_to_use: When validating market need, identifying target users, or analyzing competitive landscape for your hackathon idea
```

### Overview
Validates your hackathon idea against real market signals — who needs this, how big is the opportunity, and who are the competitors.

### Hackathon Market Validation Framework

1. **Define your target user**
   - Who has this pain point?
   - How severe is it (nice-to-have vs. hair-on-fire)?
   - How many people have this problem?

2. **Identify market signals**
   - Job postings mentioning this problem
   - Existing workarounds people use
   - Related search trends

3. **Map the competitive landscape**
   - Direct competitors and their gaps
   - Adjacent solutions that partially solve this
   - Why your approach is different

### Domain-Specific User Profiles

| Domain | Target User | Pain Point | Market Size Signal |
|--------|------------|------------|-------------------|
| **Fintech** | Gig workers without credit history | Can't access loans or insurance | 300M+ gig workers globally |
| **Logistics** | Small e-commerce sellers | Can't afford enterprise logistics | 12M+ SME sellers in India |
| **Healthcare** | Rural patients 50km+ from hospital | No access to specialists | 65% of India is rural |

---

# Section 4: Architecture & Design

---

## Skill 11: preserving-productive-tensions

```yaml
name: preserving-productive-tensions
description: Recognize when disagreements reveal valuable context, preserve multiple valid approaches instead of forcing premature resolution
when_to_use: When oscillating between equally valid approaches that optimize for different legitimate priorities during hackathon design
```

### Overview
Some tensions aren't problems to solve — they're valuable information to preserve.

**Core principle:** Preserve tensions that reveal context-dependence. Force resolution only when necessary.

### Hackathon Design Tensions

| Tension | Option A | Option B | Hackathon Strategy |
|---------|----------|----------|-------------------|
| **Security vs UX** | Maximum encryption, multi-factor auth | One-click access, minimal friction | Make it configurable — demo with smooth UX, pitch enterprise security |
| **Real-time vs Batch** | Live processing, instant results | Batch processing, cheaper | Build real-time for demo impact, mention batch as cost optimization |
| **Privacy vs Insight** | Fully anonymized data | Rich personal data for AI | Federated learning — pitch "best of both worlds" |
| **Build vs Buy** | Custom ML model | Pre-trained API (GPT, etc.) | Use APIs for hackathon speed, pitch custom model for production |

### When to Force a Decision (Hackathon Context)
- **Time pressure** → Pick the simpler option
- **Demo impact** → Pick the visually impressive option
- **Judge appeal** → Pick the more innovative option
- **Feasibility** → Pick what your team can actually build in time

---

## Skill 12: writing-implementation-plans

```yaml
name: writing-implementation-plans
description: Create detailed implementation plans with bite-sized tasks for team members
when_to_use: When design is complete and you need to split work among hackathon team members
```

### Overview
Write comprehensive plans with tasks small enough that any team member can pick up and execute (2-5 minutes per task).

### Hackathon Plan Template

```markdown
# [Project Name] — Hackathon Implementation Plan

**Goal:** [One sentence]
**Domain:** [Fintech / Logistics / Healthcare]
**Team:** [Names and roles]
**Duration:** [Hours available]

## Architecture (2-3 sentences)
[High-level approach]

## Task Breakdown

### Track 1: Backend (Person A)
- [ ] Task 1.1: Set up project scaffold (15 min)
- [ ] Task 1.2: Create data models (20 min)
- [ ] Task 1.3: Build core API endpoints (30 min)
- [ ] Task 1.4: Integrate AI/ML service (30 min)

### Track 2: Frontend (Person B)
- [ ] Task 2.1: Set up React/Next.js app (10 min)
- [ ] Task 2.2: Build main dashboard UI (40 min)
- [ ] Task 2.3: Connect to backend APIs (20 min)
- [ ] Task 2.4: Add animations and polish (30 min)

### Track 3: Data & Demo (Person C)
- [ ] Task 3.1: Prepare sample dataset (15 min)
- [ ] Task 3.2: Create demo script/flow (20 min)
- [ ] Task 3.3: Build presentation slides (30 min)
- [ ] Task 3.4: Record video walkthrough (20 min)

## Integration Checkpoints
- [ ] Hour 2: Backend + Frontend connected
- [ ] Hour 4: Core feature working end-to-end
- [ ] Hour 6: Demo-ready with polish
```

---

# Section 5: Hackathon Domain Framework

---

## Skill 13: hackathon-domain-evaluator

```yaml
name: hackathon-domain-evaluator
description: Evaluate and score hackathon ideas across feasibility, scalability, novelty, and domain alignment
when_to_use: When comparing multiple hackathon ideas or validating your chosen approach
```

### Idea Evaluation Rubric

Score each dimension 1-10:

| Dimension | 1-3 (Weak) | 4-6 (Average) | 7-10 (Strong) |
|-----------|-----------|----------------|----------------|
| **Novelty** | Existing solution clone | Incremental improvement | Genuinely new approach |
| **Feasibility** | Can't build in time | Possible with compromises | Clearly achievable MVP |
| **Scalability** | Works for demo only | Works for 1000s of users | Architecture handles millions |
| **Impact** | Nice-to-have | Solves real problem | Transforms lives/industry |
| **Demo-ability** | Hard to show | Requires explanation | Wow factor in 3 minutes |
| **Domain Fit** | Tangential to domain | Related to domain | Core domain problem |

**Target:** Total score ≥ 45/60 before proceeding.

### Domain Problem Templates

#### 🏦 Fintech Problem Template
```
Problem:  [Financial pain point for underserved population]
Users:    [Specific user segment with numbers]
Why Now:  [Technology/regulatory enabler that didn't exist before]
Solution: [AI/ML/blockchain-powered approach]
Revenue:  [Transaction fee / subscription / freemium model]
Data:     [What data makes this work, how do you get it ethically]
Risk:     [Regulatory, security, adoption risks + mitigations]
```

**Hot Problem Areas:**
- Financial inclusion for unbanked/underbanked (1.4B globally)
- Real-time fraud detection using behavioral AI
- Embedded finance for non-financial platforms
- AI-powered personal financial advice for masses
- Cross-border payments for SMEs
- Green finance / ESG scoring automation

#### 🚛 Logistics Problem Template
```
Problem:  [Inefficiency in supply chain / delivery / tracking]
Users:    [Specific stakeholder — shipper, carrier, receiver]
Why Now:  [IoT/AI/drone/EV technology enabler]
Solution: [Data-driven optimization approach]
Revenue:  [Per-shipment fee / SaaS / cost savings share]
Data:     [GPS, weather, traffic, demand signals]
Risk:     [Reliability, regulation, adoption risks + mitigations]
```

**Hot Problem Areas:**
- Last-mile delivery optimization (30% of total shipping cost)
- Reverse logistics and returns management
- Carbon-neutral supply chain tracking
- Cold chain monitoring for pharmaceuticals/food
- Predictive demand planning for hyperlocal delivery
- Multi-modal transport optimization (road + rail + air)

#### 🏥 Healthcare Problem Template
```
Problem:  [Access / quality / cost gap in healthcare delivery]
Users:    [Patient segment / provider type / administrator]
Why Now:  [AI/IoT/telehealth/genomics enabler]
Solution: [Technology-enabled care delivery approach]
Revenue:  [Per-consultation / subscription / B2B licensing]
Data:     [Health records, wearables, imaging, genomics]
Risk:     [Privacy, accuracy, regulation risks + mitigations]
```

**Hot Problem Areas:**
- AI-assisted diagnostics for resource-poor settings
- Mental health support at scale (chatbot + human hybrid)
- Drug interaction checker using AI + patient history
- Remote patient monitoring with wearable IoT
- Clinical trial matching for patients
- Preventive health scoring from lifestyle + genetics

---

## 🎯 Quick-Start Decision Tree

```
START → Pick your domain
  │
  ├─ Fintech → Use collision-zone-thinking to combine finance + [biology/game theory/social networks]
  │            → Use inversion-exercise to flip a banking assumption
  │            → Use scale-game to stress-test at 1B transactions
  │
  ├─ Logistics → Use collision-zone-thinking to combine supply chain + [ant colonies/nervous systems/weather patterns]
  │              → Use simplification-cascades to find the one abstraction
  │              → Use scale-game to stress-test at global scale
  │
  └─ Healthcare → Use collision-zone-thinking to combine healthcare + [streaming/blockchain/gaming]
                 → Use inversion-exercise to flip a clinical assumption
                 → Use meta-pattern-recognition to find cross-domain health patterns
```

---

## 🏁 Hackathon Execution Checklist

```
□ Domain selected (Fintech / Logistics / Healthcare)
□ Problem validated using domain template
□ Idea scored ≥ 45/60 on evaluation rubric
□ Brainstorming skill applied — 3 approaches evaluated
□ Collision-zone-thinking applied — novel angle found
□ Inversion-exercise applied — assumptions challenged
□ Scale-game applied — architecture validates at 1000x
□ Simplification cascades — complexity reduced to elegant core
□ Knowledge lineage traced — "why now" argument solid
□ Market validated — target users identified with data
□ Implementation plan created — tasks split among team
□ Presentation structured — Hook → Problem → Solution → Demo
□ GitHub repo clean and documented
□ Demo script rehearsed (3-minute pitch)
□ Video presentation recorded (optional)
```

---

> **Source Repositories:**
> - `superpowers-skills` (obra/superpowers-skills) — Problem-solving, collaboration, architecture skills
> - `awesome-claude-skills` (ComposioHQ/awesome-claude-skills) — Research, content, domain skills
>
> **Skills Count:** 13 curated skills from 87+ available, selected for hackathon relevance
