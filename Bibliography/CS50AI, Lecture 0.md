# Lecture 0

Author:: Harvard University
URL:: https://cs50.harvard.edu/ai/2020/notes/0/
Date Created:: 2022-01-01
- - - 

## Search
Search problems consists of an [[CS50AI, Lecture 0#^eeb615|agent]] that is given an initial state and a goal state through which the agent is to find a path or a solution to get from the initial to the final state. Google maps for example employs the use of search algorithms by taking your current location as the initial state and searches for the best path to your final state.

![[Pasted image 20220101173129.png]]

### Agent 
An agent is an entity which perceives its environment and acts upon it. ^eeb615

### State
This is the configuration or condition of an agent in its environment.
- **Initial State**: This is the state from which the search algorithm starts.

### Actions 
These are the plausible reactions given a state. The set of all possible actions can be defined as a function of the current state.

### Transition Model
A description of the state that can be obtained after performing a specified action in the preceding state. Upon receiving state `s` and action `a` as input, `Results(s, a)` returns the state resulting from performing action `a` in state `s`.

### State Space
This is the set of all states reachable from the initial state by any sequence of actions. The state space can be seen as a directed graph with states, represented as nodes, and actions, represented as arrows between nodes.

![[Pasted image 20220101185616.png]]

### Goal Test
This is a condition which tests if a given state is a goal state. For example, in a navigator app, the goal test would be whether the current location of the agent (the representation of the car) is at the destination. If it is — problem solved. If it’s not — we continue searching. ^b9b3c2

### Path Cost
A numerical cost which is associated with the paths taken during the search process. For example, a navigator app does not simply bring you to your goal; it does so while minimizing the path cost, finding the fastest way possible for you to get to your goal state.

## Solving Search Problems
**Solution:** A sequence of actions that leads form the initial state to the goal state.
**Optimal Solution:** A solution that minimizes the path cost.

In a search process, each node consists of the following data:

- A **State** ← This is useful to perform a [[CS50AI, Lecture 0#^b9b3c2|goal test]]
- The **path cost** from the initial state to the current state
- The **parent node** which generated this current state
- The **action** which took the agent from the parent node to the current node.

Nodes contain information that makes them very useful for the purposes of search algorithms.

Once the node is chosen, by virtue of storing the *parent node* and the action that led from the parent to the current node, it is possible to trace back the steps taken to get to this presumed goal state from the initial state. And the set of steps would then be known as the *solution*.

**Nodes** are nothing but a data structure, they just hold necessary information and nothing more. To search through the nodes, we make use of **Search algorithms**.

**Frontier** → The frontier is a mechanism (or data-structure) that contextually manages the nodes.