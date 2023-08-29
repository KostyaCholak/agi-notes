# Entities

This document describes the way to represent complex abstract ideas using data structures.  
Here we will not conver how to transform text (or other formats of raw data) to the structured format, this is covered in pattern matching.

## Internal vs External
Ship of Theseus is an example of a problem of identity, but under the logic of this theory, it is an evidence for the abscence of a strong link between the external (objective) world and subjective representations of this world. Objectively there was never  defined and contained object of ship, only particles in space time. Subjectively people are able to give an internal label to some particles, without giving a strong definition for which particles are included in the definition. So this definition is about the internal idea, not something external. And when the parts of the ship are being replaced, the internal idea stays the same, because it's not strongly linked to the particles of what's being called ship. So the problem of identity arises when we don't clearly separate internal world representation and external world. Identity problem does not make sense in the external world, and there is no such problem in our minds, the problem is only in linking the one world to the other - should the link between the internal ship and the particles that we initially labeled as "ship" hold after some of those particles were replaced?

## Internal representation

Can we say thay internal representations have structure?
If yes, on what level do they have it - what are the building blocks?
If no, ...???


We will use object-oriented approach to represent ideas:  
```python
ConceptName {
    field1: ...,
    field2: ...,
    ...
}
```
Here is a representation of a string literal "hello":
```python
String {
    value: "hello",
}
```

Name for the idea `String` was chosen arbitrary, it can be any random name (like `j28k01Q`), but it must be the same every time we want to refer to the idea of a literal string. Same goes for the fields. Here we will be giving meaningful names so that it's easier to understand the ideas.

Here is a representation of an idea of the command:  
`print "hello"`

```python
ImperativeCommand {
    action: ActionOnEntity {
        action: Concept {
            value: "PrintAction"
        },
        entity: String {
            value: "hello",
        }
    }
}
```

Let's make it a bit more complex:  
`print "hello" to the console`

```python
ImperativeCommand {
    action: ActionWithDescription {
        action: ActionOnEntity {
            action: Concept {
                value: "PrintAction"
            },
            entity: String {
                value: "hello",
            }
        },
        description: WhereToDescription {
            to: EntityReference {
                concept: Concept {
                    value: "Console"
                }
            }
        }
    }
}
```

