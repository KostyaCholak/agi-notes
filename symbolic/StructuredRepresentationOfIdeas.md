# Structured Representation of Ideas

This document describes the way to represent complex abstract ideas using data structures.  
Here we will not conver how to transform text (or other formats of raw data) to the structured format, this is covered in pattern matching.

## Entity
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

