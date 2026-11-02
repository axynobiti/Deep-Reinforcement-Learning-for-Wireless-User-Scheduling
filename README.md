# Deep Reinforcement Learning for Wireless User Scheduling

Implementation and evaluation of Deep Q-Networks (DQN) for wireless user scheduling, developed as part of the **Reinforcement Learning and Dynamic Optimization** course at Technical University of Crete.

## Overview

The project considers a wireless network where a base station schedules users based on their queue lengths and channel conditions, aiming to maximize throughput while minimizing packet drops.

A DQN agent is developed to learn scheduling decisions, using a neural network to approximate the long-term value of each action.

## Implementation & Evaluation

- Implemented a DQN agent using experience replay and a target network.
- Explored different state representations and neural network configurations to improve learning.
- Compared DQN against conventional scheduling policies, including Max-Weight, Longest Queue, and Greedy Throughput.
- Implemented a **lookahead beam-search heuristic** as an additional benchmark.

Performance was evaluated through simulations measuring average reward, throughput, packet drops, and queue occupancy.

## Results

The DQN learned a competitive scheduling policy, achieving performance close to Max-Weight and the lookahead benchmark. Max-Weight slightly outperformed DQN overall, suggesting that it already captures much of the useful scheduling structure.

## Tools

Python · PyTorch · NumPy · Matplotlib
