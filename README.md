# cs370

# CS-370 Portfolio README — Pirate Intelligent Agent

## Project Overview

This repository contains the artifact for CS-370: Current and Emerging Trends in Computer Science at Southern New Hampshire University. The primary artifact is `TreasureHuntGame.ipynb`, a Jupyter Notebook implementing a deep Q-learning algorithm to train a pirate non-player character (NPC) to navigate a maze and locate hidden treasure before the human player.

---

## Reflection

### What code were you given? What code did you create yourself?

I was provided with two supporting Python files — `TreasureMaze.py`, which defines the maze environment as a matrix and handles state representation, and `GameExperience.py`, which implements the experience replay buffer used during training. The Jupyter Notebook itself (`TreasureHuntGame.ipynb`) was partially provided with the neural network architecture, environment setup, and supporting functions already in place.

What I created was the core of the Q-Training Algorithm section: the training loop that drives the agent's learning. This included implementing the epsilon-greedy exploration strategy with decay, sampling experiences from the replay buffer, computing Bellman equation target Q-values, fitting the neural network on each training batch, and defining the termination condition based on the agent's win rate. Essentially, I connected the provided infrastructure into a functioning deep reinforcement learning pipeline.

---

### What do computer scientists do and why does it matter?

Computer scientists solve problems through the design and analysis of algorithms, systems, and models. At its core, the work involves abstracting complex real-world problems into formal structures that can be reasoned about and automated — whether that means designing a data structure, architecting a distributed system, or, as in this project, training an intelligent agent to navigate an unknown environment.

It matters because these solutions increasingly underpin critical infrastructure: healthcare, finance, communications, and national security all rely on software systems built on computer science principles. As AI and machine learning move further into domains that affect people's lives directly, the stakes for getting those systems right — and for understanding their limitations — only increase.

---

### How do I approach a problem as a computer scientist?

My approach starts with understanding the problem structure before writing a line of code. For the pirate agent, that meant asking: what are the states, what are the actions, what is the reward signal, and what algorithm is appropriate given those constraints? Once I had a mental model, I worked iteratively — implementing a minimal version first, observing behavior, and refining from there.

I also try to distinguish between what is given and what I am responsible for building. In this project, respecting the boundary between the provided files and my own code required carefully reading the specifications before modifying anything. That kind of disciplined, specification-driven approach transfers directly to professional software engineering, where understanding the existing system before changing it is essential.

---

### What are my ethical responsibilities to the end user and the organization?

Building intelligent systems carries genuine ethical weight. In the context of a game agent, the stakes are relatively low — but the same techniques scale to higher-risk applications like autonomous vehicles, medical diagnostics, and cybersecurity tools. My responsibility as a developer is to be honest about what a model can and cannot do, to test it rigorously rather than assuming it generalizes, and to design systems that fail gracefully rather than catastrophically.

I also have a responsibility to be transparent about the limitations of AI outputs. An agent that achieves a high win rate in training may still fail in edge cases. Communicating that uncertainty honestly — to teammates, stakeholders, and end users — is as important as building a system that performs well under normal conditions.
