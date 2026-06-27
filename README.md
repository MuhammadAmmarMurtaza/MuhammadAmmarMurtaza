# Muhammad Ammar Murtaza

I am an MS Mechatronic Engineering student working on:

## Deep Reinforcement Learning-Based Autonomous Drone Navigation

My research focuses on developing, training, testing and eventually deploying DRL-based quadrotor navigation policies using a simulation-first robotics pipeline.

## Research Focus

- Deep Reinforcement Learning for autonomous drone navigation
- Flightmare-based quadrotor simulation
- PyBullet drone RL baselines
- ROS 2-based robotics integration
- RealSense-based perception
- Jetson Orin Nano edge deployment
- Sim-to-real transfer for aerial robots

## Current Technical Stack

- Ubuntu 22.04 native Linux
- Python virtual environments
- PyTorch
- Gymnasium
- Stable-Baselines3
- RLlib / Ray
- PyBullet drone simulation
- Flightmare
- ROS 2 Humble
- Gazebo Fortress
- RealSense RGB-D / VIO sensors
- Jetson Orin Nano deployment target

## Current Research Pipeline

1. Validate DRL algorithms on simple Gymnasium environments
2. Test drone control baselines in PyBullet
3. Use Flightmare as the main thesis simulator
4. Build a modern Gymnasium-compatible Flightmare wrapper
5. Train policies using SB3, RLlib and PyTorch
6. Integrate policy inference with ROS 2
7. Test RealSense-based perception
8. Move toward Jetson-based deployment


## Research Goal

My long-term goal is to develop reliable DRL-based drone navigation policies that can be trained in simulation and later adapted for real-world autonomous flight.

## Main Projects

- `drl-drone-navigation-thesis`
- `flightmare-gymnasium-wrapper`
- `pybullet-drone-rl-baselines`
- `ros2-drone-policy-inference`
- `realsense-ros2-drone-perception`
- `autonomous-drone-racing-literature`

## Main Thesis Repository Ecosystem

My MS thesis/research direction is:

**Deep Reinforcement Learning-Based Autonomous Drone Navigation**

Current focused technical direction:

**From Privileged State to Vision Features: A Practical Flightmare Pipeline for DRL-Based Drone Gate Navigation**

The portfolio is organized as a staged research pipeline.

| Repository | Role |
|---|---|
| `drl-drone-navigation-thesis` | Main thesis hub, roadmap, setup notes, and progress tracking |
| `rl-gym-pybullet-drone-baselines` | Foundational Gymnasium, SB3, RLlib, continuous-control, and PyBullet drone baseline work |
| `flightmare-headless-rl-wrapper` | Flightmare headless RL wrapper and early Flightmare RL environment work |
| `flightmare_racing_visualization` | Flightmare UnityBridge visualization, YAML racing tracks, and gate-logging tools |
| `flightmare-vision-aware-drl-pipeline` | Implementation/pipeline repo for vision-aware DRL gate-navigation experiments |
| `flightmare-vision-aware-drl-results` | Curated thesis results and visual evidence archive |

---

### `drl-drone-navigation-thesis`

Main public research hub for my MS thesis project.

This repository tracks the research pipeline, simulator decisions, setup notes, progress logs, and future experimental roadmap.

---

### `rl-gym-pybullet-drone-baselines`

Foundational RL and PyBullet drone baseline repository.

This repository documents early reinforcement learning algorithm exploration using Gymnasium, Stable-Baselines3, RLlib/Ray, PyTorch, and PyBullet.

Current highlights:

- SB3 CartPole-v1 experiments with PPO, A2C, and DQN
- RLlib CartPole-v1 experiments with PPO and DQN
- SB3 Pendulum-v1 continuous-control experiments with PPO and SAC
- SB3 MountainCarContinuous-v0 experiments with SAC, TD3, and PPO
- Initial external `gym-pybullet-drones` visual simulation testing
- Continuous-control learning path toward drone RL

---

### `flightmare-headless-rl-wrapper`

Reusable headless RL wrapper around Flightmare.

This repository modernizes Flightmare headless RL training using Python 3.10, Gymnasium-style wrappers, Stable-Baselines3, and PyTorch.

Current highlights:

- Raw Flightmare vector wrapper
- Gymnasium-compatible single-env wrapper
- SB3-compatible VecEnv wrapper
- Scaled-action VecEnv wrapper
- PPO headless training and evaluation
- Action-scale ablation

---

### `flightmare_racing_visualization`

Flightmare UnityBridge visualization and racing-track tooling.

Current highlights:

- YAML track loader
- Scene selection for Warehouse, Industrial, Garage, and NatureForest
- Local-origin coordinate calibration
- RGB/depth/segmentation camera capture testing
- Gate-passing CSV logger
- UZH/RPG-inspired SplitS, Figure 8, and Kidney track templates
- GIF previews for visual demonstration

---

### `flightmare-vision-aware-drl-pipeline`

Reusable Flightmare vision-aware DRL gate-navigation pipeline.

This repository contains implementation-oriented tools for:

- Privileged-state teacher PPO training
- Teacher rollout dataset generation
- Compact gate/vision-feature observations
- 25D vision-proprioceptive student observations
- Imitation-learning student policy training
- PPO-from-scratch baselines
- IL-initialized PPO fine-tuning
- Robustness evaluation
- UnityBridge replay export

This repository shows the engineering implementation and reusable research pipeline.

---

### `flightmare-vision-aware-drl-results`

Curated Flightmare visual evidence and result archive for DRL-based autonomous drone gate navigation.

This repository documents the progression from privileged PPO teacher training to teacher rollout generation, imitation learning, PPO-from-scratch baselines, robustness evaluation, and UnityBridge replay validation.

Highlights:

- Phase-wise thesis reports
- Policy comparison tables
- Failure-mode analysis
- Observation-space comparison
- Phase 5 imitation-learning diagnostics
- Phase 8 robustness plots
- Phase 9 UnityBridge replay GIFs and MP4s
- Onboard RGB and feature-camera consistency evidence

Primary result:

A 25D vision-proprioceptive imitation-learning student completed the T02 three-gate Flightmare replay in UnityBridge visual validation.

Boundary:

This is replay-based visual validation of a compact vision-proprioceptive policy, not raw RGB end-to-end real-drone deployment.