# PM Knowledge Bank

A practical knowledge base for Platform Product Managers. Frameworks, templates, metrics, and principles drawn from real platform engineering work across startup, scale-up, and public sector environments.

---

## Career Context

Platform PM experience across:
- **Energy tech startup**: API platforms, revenue growth, founder-level strategy; navigated company acquisition
- **Regulated scale-up (fintech)**: Data/AI/ML platforms at enterprise scale across 14 product teams
- **Government / public sector**: Data Science Platform in slow-moving, highly regulated environment; built adoption without authority
- **Current**: Platform PM role; AI platform strategy; building with Claude (Agent SDK)

---

## Key STAR Stories + Metrics

| Story | Outcome |
|-------|---------|
| **API Platform (startup)** | £1.1M ARR; 0 → £20k/month per account potential; customer onboarding 3 months → <1 day; 5,000+ consumers in first 4 weeks |
| **ML Deployment Template** | Deploy time 4 weeks → 2.5 days (~90% reduction); app vs. infra split 30/70 → 80/20; OSAT 2.5 → 4.0; 80+ models in prod |
| **Central API Platform** | Reduced £28M technical debt exposure; centralized integration infrastructure at scale |
| **GenAI Platform** | Standardized AI tooling across 1,000+ person org; 80% customer contact deflection target; risk-tiering governance enabling rapid experimentation in regulated fintech |
| **API Platform (healthtech)** | £0.5M ARR; unlocked new revenue from organizations that couldn't integrate previously |
| **Data Science Platform (public sector)** | 68% analyst adoption in resistant, slow-moving environment; influence without authority |
| **Staff Engineer Coaching** | Engineer promoted to Staff after coaching on communication, impact framing, stakeholder management |
| **Developer Productivity Measurement** | Rolled out measurement across engineering community by partnering with engineering leadership and Agile Coaches |

**Total direct API revenue created**: ~£1.6M ARR across two roles

---

## Core Frameworks

### Problem Structuring (for ambiguous platform problems)
1. Clarify the "why" — what business/user problem are we solving?
2. Map stakeholders — who uses this, who builds on it, who maintains it?
3. Identify constraints — technical, org, timeline, risk tolerance
4. Define success — what does "good" look like in 3 months vs. 1 year?

### Phased Thinking
- Phase 0: cheapest way to validate this matters
- Phase 1: MVP for early adopters; manual processes OK
- Phase 2: scale to more teams; automate pain points
- Phase 3: platform-grade reliability, self-service

### Risk Tiering Framework (GenAI Governance)
- Tier 1 (Low): internal, low-stakes → self-service, lightweight review
- Tier 2 (Medium): internal sensitive data or low-stakes customer-facing → automated checks + async review
- Tier 3 (High): customer-facing, decision-influencing, PII → full review, human-in-the-loop, monitoring
- Key principle: shift compliance left — build guardrails into platform, not the review process

### Adoption Ladder
- L1 Aware → L2 Experimenting → L3 Shipped → L4 Scaled
- Track progression through levels, not binary "using/not using"

### Tiered Support Model
- Lighthouse (3-5 teams): embedded engineer, co-development → validate features, generate case studies
- Supported (10-15 teams): office hours, async Slack, training
- Self-serve (everyone else): docs, templates, community

### Translating Business Outcomes to Product Outcomes
- Start from business targets → define north star metrics → identify product outcomes team can move → link back to business metrics
- Example: business goal (reduce cost-to-serve) → platform goals (clean data, faster ML/AI shipping) → track adoption AND downstream customer metrics (contact rate, CSAT)

### API Product Principles
- Developer experience (DX): clear docs, sandbox, time-to-first-successful-call < 10 minutes
- Consistency: predictable naming, error handling, response formats
- Versioning: don't break existing integrations
- Observability: logs, status, rate limits visible to developers
- Self-serve: minimize support dependency to get started

### Integration Strategy (2-sided platform)
- Outbound: connecting to tools customers already use (Slack, HRIS, ERP)
- Inbound: letting customers/partners build on your API
- Moat: owning the data on both ends, not the integration itself

### GenAI Application Areas (3-bucket model)
1. Agentic workflows: AI monitors and fixes issues automatically
2. Natural language configuration: describe intent; AI handles implementation
3. Anomaly detection: AI flags unusual patterns

### Disagreement with Engineers
1. Understand their constraints first
2. Bring clarity on problem and priority
3. Give room for solution proposals
4. "What would change your mind?"
5. Ship small and learn rather than win argument and ship nothing

---

## Key Principles & Phrases

- "Stay close to customer problems, not internal politics"
- "Data challenged my intuition" — solve the pain data shows, not what people complain loudest about
- "Diagnose before you prescribe"
- "Phase the work: quick wins → structural investment"
- "Give room for the 'how' once 'why' is clear"
- "Make the right thing the easy thing" (platform/self-serve)
- "Platform is a force multiplier, not direct output"
- "Risk tiering, not one-size-fits-all"
- "Small learnings over big bets"
- Evaluation-driven development (define eval criteria before building — like TDD for AI)

---

## Interview Themes → Stories

- **Delivering impact at speed / ambiguity**: ML template (data challenged intuition), startup acquisition (kept shipping), API MVP in 2 weeks
- **Complex problem solving**: ML template 90% reduction (mapped end-to-end, diagnosed bottleneck), public sector 68% adoption (influence without authority)
- **Technical collaboration**: ML deployment transformation (deep partnership with MLOps, clarity on "why", room for "how")
- **Conflict / disagreement**: Build vs. buy debate (wrote technical paper with data, presented options not blockers); staff engineer coaching
- **Failure / learning**: Startup pivot (all-or-nothing → modular), tooling license oversight, API developer experience (would invest earlier in docs/sandbox)
- **Drive / ambition**: Lead with £28M debt reduction, £1.6M ARR, 80+ models in prod, 90% deployment reduction

---

## Platform Product Strategy

### Mission Pattern
Enable Developer Experience by building high performance, secure, scalable infrastructure through automation and promotion best practices — enabling the business to move faster safely, reducing developers' cognitive load.

### Vision Pattern
Engineers can simply and autonomously build, run and deploy software.

### Common Platform Problems to Address
1. Fractured SDLC → impacts engineering efficiency, team performance, DX, customer feedback loops
2. Lack of consistency in standards → fragmented developer workflow, slow cycle time
3. Security not a first-class citizen
4. Insufficient observability

### Strategy Goals (template)
1. X% improvement in Engineering Speed via Developer Enablement
2. Standardize infrastructure, environments, tech stack, CI/CD via IaC and automation
3. Security embedded in SDLC; minimum compliance % maintained against mandated standards
4. Improve Observability (monitoring, logging, incident management) cost-efficiently

### Metrics Framework

| Area | Metric | Notes |
|------|--------|-------|
| Engineering Speed | Lead Cycle Time | Baseline → Target (e.g. 6 days → 3 days) |
| Engineering Speed | Self-Reported Productivity | % of engineers rating themselves productive |
| Developer Happiness | Quarterly satisfaction survey | Correlated with speed |
| Compliance | % across mandated standards | Set minimum threshold (e.g. >70%) |
| Environment Adoption | % of demos/tests in non-prod | Baseline 0 → Target 100% |

### Prioritization Scoring (1=Low, 2=Medium, 3=High)

| Dimension | Description |
|-----------|-------------|
| Business Value | Direct impact on company objectives; saves £ or £ enabler |
| Developer Impact | Improves DX or reduces dev time |
| Effort | Implementation effort |
| Risk/Contagion | How quickly an unsolved problem spreads |

### Roadmap Initiative Categories
- **OKR**: Objectives and Key Results — strategic bets
- **Continuous Improvement**: incremental, ongoing
- **Support Requests (SR)**: reactive, team-driven
- **Product Requests (PR)**: feature requests from internal customers

---

## Developer Discovery Interview Template

Used to understand actual SDLC workflows — not to brainstorm solutions.

**Format**: 30-min Q&A with Engineering Managers and Tech Leads
**Principle**: "Be curious, not judgemental" — learn what they actually do today and *why*, not what they wish they had.

**Goal**: Build a holistic view of the software development lifecycle to identify both short-term wins and longer-term areas of impact. Primary customers are individual contributors on product engineering teams.

### Interview Structure

**Intro (5 min)**
> "Our aim is to get insights into the way you and your team currently work. I have questions covering the major phases of the software development lifecycle. Please focus on what you do today, and flag anything that feels wonky, confusing, or tedious."

**Questions (20 min)**

*Warm-up*
- How long have you been at the company? What is your team responsible for?

*SDLC — New Applications*
- Tell me about the last time you created a new application. What were the steps?
- How long did it take to get it up and running?
- How do you measure performance of a new application?

*SDLC — Existing Applications*
- What current applications are you working on?
- How do you measure performance? What alerts do you have set up?

*SDLC — Planning*
- When you start a new project, what's the first step? What do you do after?
- How do you identify requirements?

*SDLC — Debugging*
- What was a recent difficult bug? How did you go about debugging it?
- How do you debug production issues?
- How do you know if your services are healthy?

*SDLC — Security*
- How do you guard against security vulnerabilities in your code?
- Does your service handle PII? How?
- If you were a hacker for a moment — how would you attack your services?

*SDLC — Testing*
- How do you test or validate your work locally?
- How do you test changes in combination with other dev changes?
- How do you know a change is ready for production?

*SDLC — Product/Customer Sign-off*
- How do you share work in progress with your PM?
- How do you present work for sign-off?

**Wrap-up (5 min)**
Thank the participant, confirm any follow-up items.

### Post-Interview
- Link recording and transcript to the schedule/tracker
- Mine for trends across interviews before drawing conclusions
