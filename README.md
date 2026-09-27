# Quantum-Enhanced Traffic-Aware Path Planning for Autonomous Delivery Robots

A research-oriented conceptual framework exploring the integration of **ROS 2** and the **Quantum Approximate Optimization Algorithm (QAOA)** for traffic-aware path planning in autonomous delivery robots.

## Overview

Autonomous delivery robots operating in urban environments must continuously account for changing traffic conditions, obstacles, energy constraints, and delivery priorities. Traditional path-planning approaches can become increasingly computationally demanding as the number of robots and environmental constraints grows.

This work proposes a **conceptual quantum-enhanced path-planning framework** that combines ROS 2 with QAOA. The path-planning problem is formulated as a **Quadratic Unconstrained Binary Optimization (QUBO)** problem, allowing route selection to be represented as an optimization problem suitable for quantum and hybrid quantum-classical approaches.

## Research Scope

This work is presented as a **research and conceptual study** focusing on:

* Theoretical formulation of traffic-aware path planning
* QUBO-based mathematical modelling
* Integration architecture between ROS 2 and quantum optimization
* Multi-robot coordination
* Traffic, battery, load, and delivery-priority constraints
* Feasibility of applying QAOA to autonomous robotic path planning

The proposed framework is intended to provide a foundation for subsequent simulation, implementation, and experimental validation.

## System Architecture

The proposed architecture consists of the following functional components:

```text
┌─────────────────────┐
│   Traffic Data      │
│       Node          │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│   Robot Status      │
│       Node          │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ QUBO Formulation    │
│       Node          │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Quantum Optimizer   │
│      (QAOA)         │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  Navigation Node    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Autonomous Delivery │
│       Robots        │
└─────────────────────┘
```

## Methodology

The proposed approach models route selection as a QUBO optimization problem:

```text
C(x) = Σ wij xi xj + Σ hi xi
```

where:

* `xi` represents binary route-selection variables.
* `wij` represents traffic-aware costs between route segments.
* `hi` represents constraints such as battery level and delivery priority.

The optimization framework considers:

* Traffic density
* Robot battery level
* Delivery priority
* Delivery deadlines
* Robot load capacity
* Multi-robot coordination

The resulting optimization process is intended to provide route information to the navigation layer through the ROS 2 architecture.

## Technology & Concepts

| Area                     | Technology / Concept         |
| ------------------------ | ---------------------------- |
| Robotics Middleware      | ROS 2                        |
| Quantum Optimization     | QAOA                         |
| Mathematical Formulation | QUBO                         |
| Application              | Autonomous Delivery Robots   |
| Optimization             | Traffic-Aware Path Planning  |
| System Architecture      | Multi-Robot ROS 2 Framework  |
| Research Area            | Quantum Computing + Robotics |

## Research Objectives

The primary objectives of this work are:

1. Develop a traffic-aware path-planning architecture integrating ROS 2 and QAOA.
2. Formulate autonomous robot path planning as a QUBO optimization problem.
3. Design a modular architecture for integrating quantum optimization with ROS 2.
4. Investigate the feasibility of quantum-enhanced optimization for multi-robot path planning.
5. Establish a foundation for future simulation and experimental implementation.

## Nature of the Work

**This repository contains a research-oriented conceptual framework.**

The work focuses on theoretical modelling, system architecture, mathematical formulation, and feasibility analysis. It does not represent a fully deployed real-world quantum robotic system.

Further development is required to validate the proposed methodology through simulation, quantum computing experiments, and physical robotic platforms.

## Limitations

Several challenges remain before practical deployment, including:

* Availability and scalability of quantum hardware
* Quantum noise and error
* Optimization latency
* Real-time traffic-data acquisition
* Integration across different robotic platforms
* Computational scalability
* Need for experimental validation

## Future Work

Potential future directions include:

* ROS 2 simulation-based implementation
* Evaluation using quantum simulators
* Testing on available quantum computing platforms
* Integration of real-time traffic data
* Experimental validation using autonomous delivery robots
* Comparative evaluation with classical path-planning methods
* Extension to multi-modal transportation systems involving aerial and ground robots

## Project Timeline

**Concept / Research Development:** October 4, 2025

## Authors

**Deepak K**
Department of Electrical and Electronics Engineering
New Horizon College of Engineering, Bangalore, India

**A M Likhitha**
Department of Electrical and Electronics Engineering
New Horizon College of Engineering, Bangalore, India

## Repository Contents

```text
├── PROJECT-2_GitHub.pdf
└── README.md
```

The PDF contains the complete research document, including the proposed methodology, mathematical formulation, system architecture, limitations, and future research directions.

## References

The research document includes references covering:

* Classical path-planning algorithms
* QAOA
* QUBO / Ising formulations
* ROS 2
* Multi-robot systems
* Smart-city planning and urban logistics

---

**Research Area:** Quantum Computing • Robotics • ROS 2 • Path Planning • Autonomous Systems
