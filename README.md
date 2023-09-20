# MDP REPRESENTATION

## AIM:
The goal is to make traffic flow better. By using smart decisions for traffic lights and other actions.

## PROBLEM STATEMENT:

### Problem Description
In this traffic managing project, the goal is to optimize the flow of traffic in a given road network using Markov Decision Process (MDP) and Reinforcement Learning techniques. 

### State Space
The state space includes current traffic status at intersections, vehicle count on roads, traffic light colors, and environment factors like weather. It's like gathering puzzle pieces for making traffic smoother.

### Sample State
A sample state could include the number of vehicles waiting at each intersection, the current signal state at each intersection, and the congestion levels on different roads.

### Action Space
The action space holds choices for traffic control: changing signal colors, timing adjustments, and even redirecting vehicles.

### Sample Action
An example of an action could be changing the traffic signals from red to green at a specific intersection, allowing traffic to flow in a certain direction.

### Reward Function
The reward function is designed to provide feedback to the reinforcement learning agent on how well it's performing.

##### Smooth flow of traffic without sudden stops or traffic jams
##### Efficient utilization of road capacity
##### Minimization of delays for vehicles

### Graphical Representation:

![Screenshot 2023-09-20 150548](https://github.com/TamilVenthanRS/mdp-representation/assets/75235477/44b3b2a5-00a4-4bb0-a69f-fb02ceeb17e8)

## PYTHON REPRESENTATION:
```python
pip install git+https://github.com/mimoralea/gym-walk#egg=gym-walk

import gym
import gym_walk

P ={
    0: {
        0: [(1.0, 0, 0.0, True), (0.0, 0, 0.0, True), (0.0, 0, 0.0, True)],
        1: [(1.0, 0, 0.0, True), (0.0, 0, 0.0, True), (0.0, 0, 0.0, True)]
    },
    1: {
        0: [(1.0, 0, 0.0, True), (0.0, 1, 0.0, False), (0.0, 2, 1.0, True)],
        1: [(1.0, 2, 1.0, True), (0.0, 1, 0.0, False), (0.0, 0, 0.0, True)]
    },
    2: {
        0: [(1.0, 2, 0.0, True), (0.0, 2, 0.0, True), (0.0, 2, 0.0, True)],
        1: [(1.0, 2, 0.0, True), (0.0, 2, 0.0, True), (0.0, 2, 0.0, True)]
    }
}
```
## OUTPUT:
![Screenshot 2023-09-20 151135](https://github.com/TamilVenthanRS/mdp-representation/assets/75235477/f99a2cf5-4167-4627-a6cc-948669bc3e93)

## RESULT:
Thus, the MDP is used to create a smart traffic management approach to reduced congestion and shorter travel times. 
