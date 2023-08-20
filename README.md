# AGI Notes

## Required Components

### Sensory interfaces
Why is it required:
They are required because agents need feedback from environment in order to reason. 

### Motor interfaces
Why are they required:  
AGI is supposed be useful for people -> it's supposed be able to act -> motory interfaces aree required.


### Aknowledgement of the subjectivity
> [!NOTE]
> Highlights information that users should take into account, even when skimming.

Why is it required:
When someone talks to the agent or when when the agent reads a books there is always subjectivity in the information.  
Second source of subjectivity is the way we process the incoding information.

```mermaid
  Test graph;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

### Learning
What it is:
Learning takes ideas an agent got from reasoning and modifies the "knowledge base" of the agent.

Why is it required:
Learning is required because it's unlikely to know everything. And considering that knowledge is subjective, I would say it's impossible to know everything.

Required learning scenarios (the list is not exhaustive and probably overlapping):
- Agent's action had an effect -> associate the action with the effect
- Expected effect wasn't observed -> invalide the association between the cause and the expected effect, look for more complex theory of the relation
- Another agent gives new information about a hierarchical relation between ideas (a don is an animal) -> learn the abstract relation

### Abstraction Processing
Why is it required:
Processing of raw inputs from sensory interfaces into abstract ideas is required because abstract ideas help to learn.   
The agent can only learn statistics from raw input (requiring tons of raw input), while abstract ideas allow the agent to apply different reasoning methods that don't require tons of examples (this is why few-shot "learning" works so well).  

### Reasoning
Why is it required:
Reasoning is an essential step of learning, so it's required.

