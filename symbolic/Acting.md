# Acting

This document describes how the agent generates actions based on percieved ideas.

What we want is to have a mechanism for the agent to behave in a certain way when a concept/idea is recognised. For example when the agent is beeing greeted, it should greet back. 

The problems arise when the agent needs to work around unexpected situations, ambiguities and solve complex tasks.

Linear behaviour is easy - link behaviour with concepts and allow behvaiour to invoke other concepts. This will allow the agent to have a triggering mechanism, but it will not be able to branch or be recursive.

Next step is to allow branching using code. Behaviour is described with code, so we can add branching, making the behaviour of the agent close to common programming language in terms of abstractness of descriptions that is necessary when descrabing behaviour. Equivalence with common programming exists because we can replace the invocation of an idea with an invocation of a function. The only thing to notice is that such system works like a programming language with dynamic dispatching, because different functions can be invoked for different parameters, for example printing a file will be different from printing a string.

Next level of abstract descriptions comes from text descriptions of behaviour. Text can mean different ideas in different context, but programming languages have to be a lot more specific. This flexibility comes from context-aware pattern matching and reference resolution.

But this still does not provide functionality for highly non-linear adaptive behaviour. (Next is meta pattern matching and I'd like to add something else).

`remove all files in the folder, skip every second file, for every third skipped file print a star to the screen`