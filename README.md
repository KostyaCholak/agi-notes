# AGI Notes

## Required Components

### Sensory interfaces
**Why are they required:**  
Agents need feedback from an environment in order to reason. 

### Motor interfaces
**Why are they required:**  
AGI is supposed be useful for people -> it's supposed be able to act -> motory interfaces are required.


### Aknowledgement of the subjectivity
**What is it:**
External sources of knowledge are always subjective (be it a book or a person).
They communicate their view on the real world, not how it really is.  
Second source of subjectivity is medium of communication.  When two agents are unaligned in some underlying knowledge or use/understand words/symbols differently, they will not be able to properly understand each other and often even understand that the misunderstanding took place.

**Why is it required:**  
Outside sources of knowledge can be conflicting or false, so if an agent fully trusts them, it could lead tto inability to learn.
Because if someone has given an agent false information multiple times, then the agent shouldn't believe this source by default.
Otherwise this source could "overwrite" correct and tested knowledge. 
This is also required in order to use scientific method.

### Aknowledgement of 

```mermaid
graph LR;
    EXT_ABS[Subjective External Idea] -->|imperfect| WORDS[Word representation];
    WORDS -->|imperfect| INT_ABS[Internal Idea];
```

### Learning
What it is:
Learning takes ideas an agent got from reasoning and modifies the "knowledge base" of the agent.

**Why is it required:**  
Learning is required because it's unlikely to know everything. And considering that knowledge is subjective, I would say it's impossible to know everything.

Required learning scenarios (the list is not exhaustive and probably overlapping):
- Agent's action had an effect -> associate the action with the effect
- Expected effect wasn't observed -> invalide the association between the cause and the expected effect, look for more complex theory of the relation
- Another agent gives new information about a hierarchical relation between ideas (a don is an animal) -> learn the abstract relation

### Abstraction Processing
**Why is it required:**  
Processing of raw inputs from sensory interfaces into abstract ideas is required because abstract ideas help to learn.   
The agent can only learn statistics from raw input (requiring tons of raw input), while abstract ideas allow the agent to apply different reasoning methods that don't require tons of examples (this is why few-shot "learning" works so well).  

### Reasoning
**Why is it required:**  
Reasoning is an essential step of learning, so it's required.

