# Markov Decision Process (MDP)
* Markov decision processes give us a way to formalize sequential decision making. This formalization is the basis for structuring problems that are solved with reinforcement learning.
* In an MDP, we have a decision maker, called an agent, that interacts with the environment it's placed in. These interactions occur sequentially over time. At each time step, the agent will get some representation of the environment's state. Given this representation, the agent selects an action to take. The environment is then transitioned into a new state, and the agent is given a reward as a consequence of the previous action.
## Components of an MDP 
* Agent
* Environment
* State
* Action
* Reward
## Trajectory
The process of selecting an action from a given state, transitioning to a new state, and receiving a reward happens sequentially over and over again, which creates something called a trajectory that shows the sequence of states, actions, and rewards.
## Goal
Throughout this process, it is the agent's goal to maximize the total amount of rewards that it receives from taking actions in given states. This means that the agent wants to maximize not just the immediate reward, but the cumulative rewards it receives over time.
## Mathematical Notation
Let's say that we have a set of actions **A**, a set of states **S** and a set of rewards **R** and all of them have finite number of elements.
At each time step t = **0,1,2,..** , the agent receives some representation of the environment's state S<sub>t</sub> ∈ **S**. Based on this state, the agent selects an action  A<sub>t</sub> ∈ **A**. This gives us the state-action pair (S<sub>t</sub> , A<sub>t</sub>).
Time is then incremented to the next time step t+1 , and the environment is transitioned to a new state S<sub>t+1</sub> ∈ **S** . At this time, the agent receives a numerical reward R<sub>t+1</sub> ∈ **R** for the action A<sub>t</sub> taken from state S<sub>t</sub>.
We can think of the process of receiving a reward as an arbitrary function **f**  that maps state-action pairs to rewards. At each time **t** , we have 

**f(S<sub>t</sub> , A<sub>t</sub>) = R<sub>t+1</sub>**  
The trajectory representing the sequential process of selecting an action from a state, transitioning to a new state, and receiving a reward can be represented as  
S<sub>0</sub>, A<sub>0</sub>, R<sub>1</sub>,S<sub>1</sub>, A<sub>1</sub>, R<sub>2</sub>,S<sub>2</sub>, A<sub>2</sub>, R<sub>3</sub>,...  
  
Representing diagrammatically,  
![](https://github.com/sanjay-thiyagarajan/Reinforcement_Learning/blob/main/Markov%20Decision%20Process%20(MDP)/MDP-diagram.jpg)
