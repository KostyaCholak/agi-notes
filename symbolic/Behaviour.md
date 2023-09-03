# Behaviour

Work In Progress

This document describes how the agent behaves.

In the proposed theory behvaiour arises as a response to an observation. Observations can be about the external world (*the sun has risen*) or the internal process of reasoning (*I've been tricked*).  
People simplify the process of observation and reasoning about it by being concerned only with abstract concepts, not the raw world. We don't think about specific atoms that compose an apple, we think about an idea of the apple that does not have a strong link to the world, meaning that it's a subjective simplification of the reality.  

We make an assumption that every idea can be represented as some structured data.
With this assumption we can create links between ideas and actions.

## Linearity of behaviour

What we want is to have a mechanism for the agent to behave in a certain way when a concept/idea is recognised. For example when the agent is beeing greeted, it should greet back. 

The problems arise when the agent needs to work around unexpected situations, ambiguities and solve complex tasks.

Linear behaviour is easy - link behaviour with concepts and allow behvaiour to invoke other concepts. This will allow the agent to have a triggering mechanism, but it will not be able to branch or be recursive.

Next step is to allow branching using code. Behaviour is described with code, so we can add branching, making the behaviour of the agent close to common programming language in terms of abstractness of descriptions that is necessary when descrabing behaviour. Equivalence with common programming exists because we can replace the invocation of an idea with an invocation of a function. The only thing to notice is that such system works like a programming language with dynamic dispatching, because different functions can be invoked for different parameters, for example printing a file will be different from printing a string.

Next level of abstract descriptions comes from text descriptions of behaviour. Text can mean different ideas in different context, but programming languages have to be a lot more specific. This flexibility comes from context-aware pattern matching and reference resolution.

But this still does not provide functionality for highly non-linear adaptive behaviour. (Next is meta pattern matching and I'd like to add something else).

## Representation of behaviour

The idea is to find an entity that describes what we need to achieve (behvaiour entity) and we will be able to find actions to do that using associations of actions to the concepts behind the behaviour entity.


## Problems 
There is no direct link between entity that is represented by impercal commands and the behaviour entitiy. 
Here is an example:  

`remove all files in the folder, skip every second file. For every third skipped file print a star to the screen`

There are two sentences in this description. 

---
WIP:  
Can the two sentences be combined into something single?
And why do we want them to be combined into something single?

Because behaviour is fully controlled by a combination of a few things, one of each is the entity of the idea that originated the behvaiour.

Behaviour must have a start and at the moment it starts from some idea that has actions connected to it.

Let's set a goal to understand what internal factors control the behvaiour of an agent, this will show us what elements are required.

What internal factors control the behaviour of an agent?
Internal factors that control behvaiour of a regular computer program are code and initial state of the memory.


## Getting from an idea to actions
Hard-wiring of ideas to actions seems to be working only for simple step-by-step actions, often planning is required.  
Planning itself is an action (process).  
One way to understand what functionality is needed would be to list ideas of actions and try to see how people process them.  
*Situation:*   
Person expects a guest. Doorbell rings.  
*Thinking process:*  
Person models what can be the cause of this event and somehow understands that probably there is someone at the door.
But is this really modeling?  
Can it be, that this event is hard-wired to the idea of someone being at the door?  
Such hard-wiring would be much more effective, but is it sufficient to replicate the way people think?  
Let's for now imaging that there is no actual modeling going on.  
How do we get an idea to open the door?  
I'm not sure how this is being developed in our brain, but later it's most likely being done automatically, so also hird-wired.  
But an idea of someone being at the door will not always trigger us to open the door.   
What if there is someone we don't want to see?  
Is this behaviour (of deciding not to open) still explainable only with hard-wiring?  
Then probably the chain of "wires" will be like this:
- *Doorbell rings* -> "There is someone unknown at the door"
- "There is someone unknown at the door" -> "Who could it be?"
- I don't know how the resolution of "Who could it be?" is done, but we get to conclusion "There is someone unpleasant at the door"  

