# 1-Day Workshop: Domain Modelling From First Principles

First principles are the origins, main concepts or assumptions that cannot be deduced from anything else. Reasoning from first principles is best described by Elon Musk: You boil things down to the most fundamental truths and say, "What are we sure is true?" ... and then reason up from there. This contrasts with reasoning by analogy, "where we are doing this because it’s like something else that was done or it is like what other people are doing."

Reasoning from first principles takes a lot of mental energy, but it is the key to radical innovations beyond small incremental evolutions. This is particularly relevant for domain modelling in DDD, especially on a core domain that we'd like to understand deeper.

Join Cyrille Martraire for a whole day where you will learn how to deconstruct domain models until you reach their substantial first principles. We'll start from feature requests as on a real project, and we'll crunch them through code refactoring and through critical analysis, leading to insights and smarter implementation in the resulting code.

## What you will learn through practice

- How to turn hardcoded business logic into dynamic, adaptive behavior
- How to upgrade maintenance-heavy configuration lists into zero-maintenance criteria
- How to reverse a formula into its component terms, leading to fewer code, more flexible design and a better separation of concerns
- How to deconstruct a possibly large set of workflows into the few first principles that generate them
- How code refactorings can hint at deeper business insights
- How drawing domain-specific notations, domain language and language structure can suggest business insights
- How splitting the roles of specifying vs. implementing leads to sub-optimal results
- How domain modelling patterns help accelerate discovery of the first principles
- How strategic planning of features can dramatically accelerate discovery of the first principles too
- How modelling from first principles is usually local within a Bounded Context
- AND How this powerful approach can turn boring business specs into a dangerously seductive game, leading to a new form of developer procratination!

## Notes

- Where does this calculation come from? 
- where does this workflow come from?
- Where do lists of values come from? From bigger lists! From extensional to intentional modelling.
- Play the Business Analyst - Specify this feature (and experience yourself the bias of the job)
- Drawing domain-specific notations to hint at business insights (payments, workflow)
- Deconstructing workflows from first principles: where does this workflow come from?
- Discussion: When reasonong by analogy works best
- Discussion: smarter models tend to be rigid, and how to avoid that.
- DRY: similar formulas to refactor into one: anniversary dates & payments calculations
- SRP mix of discount & taxes… FX rate conversion
- if currency == ZAR, PHB, … -> illiquid currencies
- Supermarket kata, the Human Compiler
- Smarter means more rigid: OCP at every level to hedge
- Split/Join dichotomy: Fragmenting into Bounded Context vs Merging special cases into a systematic model
- Strongly Typed, with Generic Extension
- from multiple workflows to one with optional steps: if country == ZAR, NIG, TURKEY or LIBYE then geopolitic risk analysis required -> if country in list of risky countries
- arbitrary workflows to refactor into delegation + constant workflow
- arbitrary workflows to refactor into topological sort + short-circuit + senior ranking
