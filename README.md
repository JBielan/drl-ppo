# Unity Tennis environment

The goal of both agents is to hit the ball as many times as possible.

![Tennis environment](https://github.com/JBielan/drl-ppo/blob/master/tennis.gif)

The Jupyter notebook in this repository contains a solution using the Unity ML-Agents **Tennis** environment.

## Project Details

The *state space* for this project consists of 8 continuous values representing the position and velocity of a racket and ball in the X-Y plane.

The *action space* is a vector with two continuous values, clamped between -1 and 1, corresponding to the X and Y movements of the racket in the game, where the goal is to move the racket so it collides with the ball in a manner that causes the ball to move over the net, but not "go out" (collide with the back of the court area). 

Code for the Unity **Tennis** agent can be viewed [here](https://github.com/Unity-Technologies/ml-agents/blob/master/UnitySDK/Assets/ML-Agents/Examples/Tennis/Scripts/TennisAgent.cs)

A reward of +0.1 is provided for each step that the agent's shot goes over the net and not out, while a penalty of -0.01 for any failed shot or when the ball collides with the floor.

The environment is considered solved when the agents have an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents).

## Getting Started

#### Install the Anaconda distribution of Python 3

[Anaconda Python](https://www.anaconda.com/download/#macos) installation.

#### Obtain Unity ML-Agents

Install [Unity ML-Agents](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Installation.md) and [NumPy](http://www.numpy.org/).

## Instructions

#### Start Jupyter and 

```
> jupyter notebook
```

Open **ppo-tennis.ipynb**, run cells according to the order and that's it!
