# What if we could automate software design?

You think we're not there yet? But F# Type Providers already infer a complete schema from a plain folder of JSON samples. Academia knows how to use "Latent Semantic Indexing" to suggest modules around lexical clusters (Bounded Contexts anyone?). On the other hand, our industry increasingly codifies our guidelines, which get closer to algorithmic steps, as in the "Rule of 3 before refactoring" or the "Transformation Priority Premise". And we haven’t even mentioned Machine Learning yet, with big players like Google, Facebook or the MIT recently releasing tools to spot and fix bugs automatically.

Still, automated software design is not a thing yet. But what would it take for it to be true? It could help tackle large legacy code bases, or help prevent code from getting out of control in the first place. Beyond that, if we can describe software design so that it can be automated, it can also help developers really understand it.

Through this talk I want to explore the ideas already there, propose some practical directions and experiments, while trying to ignite the audience into trying things as well.

As a human developer I absolutely love doing software design myself, so I'm a bit reluctant to let it go to the machines. Will we have to adapt?

## Additional Information & Outline

This proposal is more like a "position paper" on a topic I've had in my mind for a while, but still not mature. Here's the outline I have at the moment:

- From code accumulation to basic refactoring, and how it can be automated in simple cases
- F# Type Providers, it’s daily life for lucky practitioners already, and we'll see how it works
- "Crime as a Code Scene" code forensic techniques by Adam Thornhill
- MOOSE and how Latent Semantic Indexing can suggest lexically consistent modules, and perhaps Bounded Contexts
- Some other proposals: calls stack clustering, tests subsumption, automating TPP, fuzzy similarity search & compression techniques
- Imagining an Append-Only, self-refactorable programming language that we would name Tetris
- Main Challenges

## Keywords
Software Design, automation, mass refactoring, semi-automatic, inference, TDD, semantic analysis
