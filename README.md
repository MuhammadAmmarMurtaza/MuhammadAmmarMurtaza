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

## Main Projects

- `drl-drone-navigation-thesis`
- `flightmare-gymnasium-wrapper`
- `pybullet-drone-rl-baselines`
- `ros2-drone-policy-inference`
- `realsense-ros2-drone-perception`
- `autonomous-drone-racing-literature`

### `flightmare-headless-rl-wrapper`

Modern Gymnasium/SB3 wrapper for headless Flightmare quadrotor RL training using Python 3.10, PyTorch and Stable-Baselines3.

Current status:

- Flightmare headless backend connected
- Raw vector wrapper implemented
- Gymnasium-compatible single-env wrapper implemented
- SB3 VecEnv wrapper implemented
- Scaled-action VecEnv wrapper implemented
- PPO headless training and evaluation working
- Best current action scale: ±0.5
- Latest PPO evaluation: mean reward 2.5187 ± 0.0925, mean length 36.1

### `drl-drone-navigation-thesis`

Main public research hub for my MS thesis project on Deep Reinforcement Learning-Based Autonomous Drone Navigation.

This repository tracks the research pipeline, setup notes, simulator decisions, progress logs and future experimental roadmap.

## Research Goal

My long-term goal is to develop reliable DRL-based drone navigation policies that can be trained in simulation and later adapted for real-world autonomous flight.

## Main Thesis Repositories

### `drl-drone-navigation-thesis`

Main public research hub for my MS thesis project:

**Deep Reinforcement Learning-Based Autonomous Drone Navigation**

This repository tracks the research pipeline, simulator decisions, setup notes, progress logs and future experimental roadmap.

---

### `flightmare-headless-rl-wrapper`

Mode A of my Flightmare thesis pipeline.

Modern Gymnasium/SB3 wrapper for headless Flightmare quadrotor RL training using Python 3.10, PyTorch and Stable-Baselines3.

Current highlights:

- Raw Flightmare vector wrapper
- Gymnasium-compatible single-env wrapper
- SB3-compatible VecEnv wrapper
- Scaled-action VecEnv wrapper
- PPO headless training and evaluation
- Action-scale ablation
- Best current internal action scale: ±0.5

---

### `flightmare_racing_visualization`

Mode B of my Flightmare thesis pipeline.

Configurable Flightmare UnityBridge tools for quadrotor racing visualization, YAML-driven racing tracks, local-origin calibration, onboard camera capture and gate-passing CSV logging.

Current highlights:

- YAML track loader
- Scene selection for Warehouse, Industrial, Garage and NatureForest
- Local-origin coordinate calibration
- RGB/depth/segmentation camera capture testing
- Gate-passing CSV logger
- UZH/RPG-inspired SplitS, Figure 8 and Kidney track templates
- GIF previews for visual demonstration