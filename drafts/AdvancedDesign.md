
This training covers and exclusive training created by Cyrille Martraire, building on DDD and extending it with additional modeling guidance. It's targeted at developers involved in business domain modeling, to help craft sharper domain models that bring competitive advantage.

## Duration: 

From 1 to 2 days depending on the scope

## Audience: 

Object Oriented Design skills, DDD notions. No pre-requisite in maths or functional programming. Code examples will be given in Java, but exercises can be done in any language and without any specific framework or library.

# Design Patterns beyond the DDD book

- Classical Design Patterns that also are domain modeling patterns: State, Flyweight, Composite, Interpreter, Null Object, Interpreter, Strategy
- Domain-oriented specializations: Conventions, Smart Identifier, Policy
- Domain Modeling: 
- Modeling principles: Congruence, Extrinsic/Extrinsic, Relative/Absolute 

# Bounded Contexts archetypes

Collaborative Construction, Actual Vs. Planed, Antagonist Purposes, Irreconcilable Differences (of shapes, accuracy, volume)

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

- similar formulas to refactor into one: FX rate conversion, mix of discount & taxes...
- arbitrary workflows to refactor into delegation + constant workflow
- arbitrary workflows to refactor into topological sort + short-circuit + senior ranking
- if country == ZAR, NIG, TURKEY or LIBYE then geopolitic risk analysis required -> if country in list of risky countries
- if currency == ZAR, PHB, … -> illiquid currencies 
- Supermarket kata

# Critique my design!

Abstract
Over the last years I've been quite proud of the way I've been applying my design skills to solve domain problems in an elegant fashion, with less code that does more and that is easier to maintain. Or was it, really?
In this session we will go through some examples of my past designs (and perhaps of yours too?), then asking the audience to find flaws in the design or in the reasoning that led to it. And of course this is not to blame anyone personnally!

keywords: critique, design clinique, critical thinking, clever, elegant, complexity, affordance, accessibility, surprise, rigidity

# Learn hands-on with Cyrille the delicate art of designing supple domain models that are elegant, tasty and that evolve well.
Learn in practice how to raise the declarativeness level of your code, and how to make it more composable.

All this takes nuance, which is why we will also go through a few pendantic words like Congruence, Salience, Extrinsic and Extensional to provide a better guidance for the designer. You'll work on examples, and we'll mention standard but lesser-known patterns along the road.

keywords: training, hands-on, advanced, symmetries, monoids, patterns, FP, composability, declarative, patterns, analysis
