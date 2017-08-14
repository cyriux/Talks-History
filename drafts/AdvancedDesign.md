# Learn hands-on with Cyrille the delicate art of designing sharp domain models.

Learn in practice how to make your models smarter, how to raise the declarativeness level of your code and how to make it more composable, using proven modeling patterns byeond the DDD book. You'll work on examples, and we'll cover proven patterns beyond the DDD books.

This training covers and exclusive training created by Cyrille Martraire, building on DDD and extending it with additional modeling guidance. It's targeted at developers involved in business domain modeling, to help craft sharper domain models that bring competitive advantage.

## Keywords: training, hands-on, advanced, symmetries, monoids, patterns, FP, composability, declarative, patterns, analysis

## Duration: 

From 1 to 2 days depending on the scope

## Audience: 

Object Oriented Design skills, DDD notions. No pre-requisite in maths or functional programming. Code examples will be given in Java, but exercises can be done in any language and without any specific framework or library.

# Business case: an online insurance brokerage

SEO, catalogue of insurance packages (combining several different basic insurances into something more valuable for customers), application, credit approval(analysis, antifraud, pricing, limit), transaction closing, billing, claim management, aggregation for reinsurance with a big name, reporting, commissioning


# Modeling toolbelt

## Design Patterns beyond the DDD book

- Classical Design Patterns that also are domain modeling patterns: State, Flyweight, Composite, Interpreter, Null Object, Interpreter, Strategy
- Domain-oriented specializations: Conventions, Smart Identifier, Policy
- Domain Modeling: Top-down defaulting, bottom up consolidation (derived values), Balanced Business Transaction (A quantity of 
something, e.g. a product or service, exchanged against a quantity of something else, usually cash; can be bipolar, or polarized on one particular side)
- Modeling principles for a more stable design: Congruence, Extrinsic/Extrinsic, Relative/Absolute, Upfront Variety, Cost/benefit now, vs Progressivity / Plasticity, Benchmark against another business domain

## Bounded Contexts archetypes

Collaborative Construction, Actual Vs. Planed, Antagonist Purposes, Irreconcilable Differences (of shapes, accuracy, volume), the E-Commerce backbone

Example of Tech Debt: when your current code is still a "tree plus dirty hacks" whereas you've now realized the problem is actually a "DAG" 

> I once had the best ever domain expert, he was the CEO. We would sit on the table and discuss until we felt we got into the essence of the problem, or the underlying maths.

# Composability Workshop, with Monoids inside

For many reasons, composability is good. But how do we design to maximize the ability to be composed? And what does it really mean to be composable?
Through interactive discussions with the audience we'll cover various aspects of the topic: mutable state, side-effects, error handling, interfaces design, desirable properties and even social aspects. The goal is to understand how composability works in order to better design for it.

## Common Examples

- Predicates
- Quantities
- Ranges
- Grants // using order relation
- Maps & nested monoids: Cascaded Parameters, Mergeable Documents (UPSERT read models), Object Template

## From primitive monoids to domain concepts monoids

Inheriting the properties from the encapsulated type(s) at the tuple : record-level 

## Tricks to compose what doesn't compose 

e.g. for SQL-ish. Map-reduce. Storm. 

- Ratio 
- Average, stdev
- Moving average
- Curves as polylines or splines
- Histograms with same buckets, different buckets
- Tuple Everything: turn it into a tuple (result, errors) to make it a closed type // railway-oriented programming


# Refactor your specs workshop

Premature Specification = lost opportunities
  
The "Human Compiler" anti-pattern

- similar formulas to refactor into one: FX rate conversion, mix of discount & taxes... Books are useful, but copying closed formulas verbatim is not how we build great products
- Supermarket kata
- From extensional to intensional: topological tree (e.g. Make build tool)
- properties: zero-sum game, don't tax twice

And of course: recognize and apply all the patterns from your toolbelt

Start with concrete examples of all kinds (text, excel, visual...), sketching (cash flows diagrams, wiring boxes, workflows), exploratory code, model as code, metaphors (modular synth)

Chase analogies, similarities 
look for symmetries and invariants in domain: in sentences, visually, use your brain as a pattern finder, or in the code if not found before
TDD: no duplication (Within a BC: cash management != legal), as expressive as possible

Common part or structure of scenarios suggests refactoring. It may be subtle duplication hidden behind a different face.

Generalize: a developer job! 
Automated scenarios: make sure progression never regresses

Progression: just like baby steps in TDD, move from rather simple examples to more complex, without gaps. Or diversity first : swap, future, option, FX to assess their major commonalities ASAP.

## Explicit Intent Modeling / mandate / decision rationale

"I'm ok below $200k" as opposed to just "ok" for the current loan at $180K.

- ok below $120k
- ok as long as guarantors at least AAA
- ok as long as it's a well-known product

E.g. Survey form about loans: do you need filling it again after a change? It depends on the kind of change. Dimensions of change. In finance, standard risk factors are obvious candidates. Plus other concerns like exotic-ness wrt to regulator 

In trading Market-Makers advertise their conditions "I'd be ok to trade at this price", like the Instant Buy on eBay. 

Also in trading at SWS, traders could define price as linked prices: "= future price * coefficient" running on the exchange server

E.g. "Sell it all before time: 6 unit: month from: signature date"

Indexed interest rates, indexed apartment rent. Alias, e.g. "Leading Month", Spot, Overnight, Tomorrow/Next. Partially sortable.

E.g. DDDEU 2015 modeling: replicating portfolio management from one a leader investor to followers investors: not easy directly, but easier once you go through the indirection of the (more abstract) "investment intent"

# Deconstructing Business Workflows (application of refactoring the specs)

intro

- Written music vs Jazz improvisation & Dj mix
- Open loop control vs Close-loop control: ballistic vs regulation

Workflows are so 90's!

- Time-to-market-driven: Tunnel to iterative, Parallel work vs Sequential, Collaborative 
- UX-driven: Human Vs Rigid, Formal & audited vs draft & Off-the-record
- from Centralized Explicit Orchestration to Choreography with Living Documentation: timeline, checklist, monitoring
- BPMN? To materialize manual processes 

Every workflow involves some more or less implicit negotiation aspect: acknowledge it and make it explicit, or it will happen outside in the worst conditions.

## Where do workflows come from? 
- Short circuit early
- Don't disturb people
- only disturb senior people once everything's ready
- Things that depend on prerequisite have to happen after

Questioning workflows
- serial bs parallel
- draft vs. final 
- reusable decisions

Workshop

- arbitrary workflows to refactor into delegation + constant workflow
- arbitrary workflows to refactor into topological sort + short-circuit + senior ranking

## Explicit Impacts - Sensitivity to changes

- by category of change: dates, amounts, legal clauses, counterparty, vanilla (standard-ness) 
- if country == NIGERIA, TURKEY or LIBYA then geopolitic risk analysis required -> if country in list of risky countries
- if currency == ZAR, THB, … -> "illiquid" currencies

Goal: reverse-engineer the rationale behind the business rule, to code it from the first principles

## Decision Rationale Over Just Decisions

"I'm ok below $200k" as opposed to just "ok" for the current loan at $180K.

- ok below $120k
- ok as long as guarantors at least AAA
- ok as long as it's a well-known product

E.g. Survey form about loans: do you need filling it again after a change? It depends on the kind of change. Dimensions of change. In finance, standard risk factors are obvious candidates. Plus other concerns like exotic-ness wrt to regulator 

In trading Market-Makers advertise their conditions "I'd be ok to trade at this price", like the Instant Buy on eBay. 

Also in trading at SWS, traders could define price as linked prices: "= future price * coefficient" running on the exchange server

E.g. "Sell it all before time: 6 unit: month from: signature date"

Indexed interest rates, indexed apartment rent. Alias, e.g. "Leading Month", Spot, Overnight, Tomorrow/Next. Partially sortable. 

# Critique my design!

The best design may be too good to be true.

- CRUD by default: Not useful because we know so little everything's just a notebook at the moment: CRUD
- Expand the Design-Requirements Grey Zone: Design Vs Requirements (Alistair Cockburn), or the different between discovering and inventing
- Messy Domains: Identify early messy domains (subject to arbitary external or historical peculiarities) vs strictly regular domains (that you own, or that only depend on pure logic reasoning)
- Intelligence Cap: Using concepts not everybody involved can understand is irrelevant, 

Exercise:

Over the last years I've been quite proud of the way I've been applying my design skills to solve domain problems in an elegant fashion, with less code that does more and that is easier to maintain. Or was it, really?
In this session we will go through some examples of my past designs (and perhaps of yours too?), then asking the audience to find flaws in the design or in the reasoning that led to it. And of course this is not to blame anyone personnally!

keywords: critique, design clinique, critical thinking, clever, elegant, complexity, affordance, accessibility, surprise, rigidity

