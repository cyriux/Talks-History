# Learn hands-on with Cyrille the delicate art of designing sharp domain models.

Learn in practice how to make your models smarter, how to raise the declarativeness level of your code and how to make it more composable, using proven modeling patterns byeond the DDD book. You'll work on examples, and we'll cover proven patterns beyond the DDD books.

This training covers and exclusive training created by Cyrille Martraire, building on DDD and extending it with additional modeling guidance. It's targeted at developers involved in business domain modeling, to help craft sharper domain models that bring competitive advantage.

## Keywords: training, hands-on, advanced, symmetries, monoids, patterns, FP, composability, declarative, patterns, analysis

## Duration: 

From 1 to 2 days depending on the scope

## Audience: 

Object Oriented Design skills, DDD notions. No pre-requisite in maths or functional programming. Code examples will be given in Java, but exercises can be done in any language and without any specific framework or library.

# Design Patterns beyond the DDD book

- Classical Design Patterns that also are domain modeling patterns: State, Flyweight, Composite, Interpreter, Null Object, Interpreter, Strategy
- Domain-oriented specializations: Conventions, Smart Identifier, Policy
- Domain Modeling: 
- Modeling principles for a more stable design: Congruence, Extrinsic/Extrinsic, Relative/Absolute, Upfront Variety

# Bounded Contexts archetypes

Collaborative Construction, Actual Vs. Planed, Antagonist Purposes, Irreconcilable Differences (of shapes, accuracy, volume)

Example of Tech Debt: when your current code is still a "tree plus dirty hacks" whereas you've now realized the problem is actually a "DAG" 

# Composability Workshop, with Monoids inside

For many reasons, composability is good. But how do we design to maximize the ability to be composed? And what does it really mean to be composable?
Through interactive discussions with the audience we'll cover various aspects of the topic: mutable state, side-effects, error handling, interfaces design, desirable properties and even social aspects. The goal is to understand how composability works in order to better design for it.


## Common Examples

- predicates
- quantities
- ranges
- grants // using order relation
- maps & nested monoids,: Cascaded Parameters, Mergeable Documents (UPSERT read models), Object Template

# From primitive monoids to domain concepts monoids

Inheriting the properties from the encapsulated type(s) at the tuple : record-level 

## Tricks to compose what doesn't compose 

e.g. for SQL-ish. Map-reduce. Storm. 

- ratio 
- average, stdev
- moving average
- curves as polylines or splines
- Histograms with same buckets, different buckets
- (result, errors) // Turn into a tuple

# Refactor your specs workshop

The "Human Compiler" anti-pattern

- similar formulas to refactor into one: FX rate conversion, mix of discount & taxes...
- Supermarket kata
- From extensional to intensional: topological tree (e.g. Make build tool)
- properties: zero-sum game, don't tax twice

# Deconstructing Business Workflows (application of refactoring the specs)

intro

- Written music vs Jazz improvisation & Dj mix
- Open loop control vs Close-loop control: ballistic vs regulation

Workflows are so 90's!

- Time-to-market-driven: Tunnel to iterative, Parallel work vs Sequential, Collaborative 
- UX-driven: Human Vs Rigid, Formal & audited vs draft & Off-the-record
- from Centralized Explicit Orchestration to Choreography with Living Documentation: timeline, checklist, monitoring
- BPMN? To materialize manual processes 

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

# Explicit Impacts - Sensitivity to changes

- by category of change: dates, amounts, legal clauses, counterparty, vanilla (standard-ness) 
- if country == ZAR, NIG, TURKEY or LIBYE then geopolitic risk analysis required -> if country in list of risky countries
- if currency == ZAR, PHB, … -> illiquid currencies

# Rationale Over Decisions

- ok below $120k
- ok as long as guarantors at least AAA
- ok as long as it's a well-known product

In trading Market-Makers advertise their conditions "I'd be ok to trade at this price", like the Instant Buy on eBay. 

Also in trading at SWS, traders could define price as linked prices: "= future price * coefficient" running on the exchange server

# Critique my design!

Over the last years I've been quite proud of the way I've been applying my design skills to solve domain problems in an elegant fashion, with less code that does more and that is easier to maintain. Or was it, really?
In this session we will go through some examples of my past designs (and perhaps of yours too?), then asking the audience to find flaws in the design or in the reasoning that led to it. And of course this is not to blame anyone personnally!

keywords: critique, design clinique, critical thinking, clever, elegant, complexity, affordance, accessibility, surprise, rigidity

