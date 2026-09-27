# Quantum-Enhanced Traffic-Aware Path Planning for Autonomous Delivery Robots

> A conceptual research study exploring the possible application of **Quantum Approximate Optimization Algorithm (QAOA)** and **Quadratic Unconstrained Binary Optimization (QUBO)** to traffic-aware path planning for autonomous delivery robots.

---

## About

This project was developed as a **conceptual research study** to explore how ideas from quantum computing could potentially be applied to robotics and autonomous navigation.

The work focuses on the possibility of combining **ROS 2**, **QUBO-based optimization**, and **QAOA** to address path-planning problems where multiple factors such as traffic, battery level, delivery priority, and multiple robots need to be considered.

The concept was developed on **October 4, 2025** as an initial research idea. The purpose of this work was to study the problem, develop a possible mathematical formulation, and propose an architecture that could be explored further through implementation and experimentation.

**This work is conceptual and has not been implemented or experimentally validated.**

---

## Problem Statement

Autonomous delivery robots may need to select suitable routes while dealing with changing traffic conditions, limited battery capacity, delivery priorities, and the presence of other robots.

As the number of possible routes and constraints increases, the path-planning problem can become more complex.

This project explores whether such a problem could potentially be represented as a **QUBO optimization problem** and investigated using **QAOA**.

---

## Proposed Approach

The basic idea is:

```text
Traffic Information
        │
        ▼
Robot Information
(Battery / Load / Priority)
        │
        ▼
Path Planning Problem
        │
        ▼
QUBO Formulation
        │
        ▼
QAOA
(Proposed Approach)
        │
        ▼
Route Selection
        │
        ▼
ROS 2 Navigation
        │
        ▼
Delivery Robot
```

The above represents the **proposed concept**, not an implemented system.

---

## QUBO Formulation

The path-selection problem is conceptually represented using a QUBO objective of the form:

```text
C(x) = Σ wij xi xj + Σ hi xi
```

where:

* `xi` represents binary route-selection variables.
* `wij` represents costs or interactions between route segments.
* `hi` represents individual costs and constraint-related terms.

The proposed formulation considers factors such as:

* Traffic conditions
* Battery level
* Delivery priority
* Delivery deadlines
* Robot load
* Route availability
* Multi-robot coordination

The formulation presented in this project is part of the **conceptual study** and requires further implementation and testing.

---

## Proposed System Architecture

```text
┌─────────────────────┐
│    Traffic Data     │
│        Node         │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│    Robot Status     │
│        Node         │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  QUBO Formulation   │
│   Proposed Model    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│  QAOA Optimization  │
│   Proposed Method   │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│      ROS 2          │
│ Navigation Layer    │
└──────────┬──────────┘
           │
           ▼
┌─────────────────────┐
│ Autonomous Delivery │
│       Robot         │
└─────────────────────┘
```

---

## Research Objectives

The main objectives of the study were:

1. To understand the possibility of formulating autonomous robot path planning as a QUBO problem.
2. To explore the use of QAOA as a possible optimization method.
3. To propose a basic architecture connecting quantum optimization concepts with ROS 2.
4. To consider traffic and robot-specific constraints in route selection.
5. To identify possible directions for future implementation and experimentation.

---

## Current Status

| Area                    | Status          |
| ----------------------- | --------------- |
| Concept Development     | Completed       |
| Problem Study           | Completed       |
| Proposed Architecture   | Completed       |
| QUBO Formulation        | Conceptual      |
| QAOA Implementation     | Not implemented |
| ROS 2 Integration       | Not implemented |
| Simulation              | Not performed   |
| Hardware Testing        | Not performed   |
| Experimental Validation | Not performed   |

---

## Limitations

Since this project is currently conceptual, the proposed approach has not yet been tested in a simulation or on a physical robot.

Some of the main areas requiring further investigation are:

* Practical implementation of the QUBO formulation
* Scalability for larger path-planning problems
* QAOA performance on the proposed problem
* Comparison with classical path-planning methods
* Real-time traffic data integration
* Computational requirements
* Integration with an actual ROS 2 navigation system

Therefore, no conclusion is made in this work regarding whether QAOA would provide an advantage over existing classical approaches.

---

## Future Work

The concept could be developed further through:

* Implementing the proposed QUBO model
* Testing the model using classical optimization methods
* Experimenting with QAOA simulators
* Studying the effect of increasing problem size
* Integrating the optimization approach with ROS 2
* Creating a multi-robot simulation environment
* Comparing the results with classical path-planning methods
* Eventually testing the concept on a physical robot

---

## Project Timeline

**Concept / Research Development:** October 4, 2025

The initial concept and research work documented in this repository were carried out on **October 4, 2025**.

The repository is being published later to document and preserve the work.

---

## Repository Contents

```text
Quantum-Enhanced-Traffic-Aware-Path-Planning/
│
├── PROJECT-2_GitHub.pdf
└── README.md
```

### PROJECT-2_GitHub.pdf

The PDF contains the original conceptual research document, including the proposed methodology, mathematical formulation, system architecture, limitations, and future scope.

---

## Team

### Deepak K

Department of Electrical and Electronics Engineering
New Horizon College of Engineering
Bangalore, India

### A M Likhitha

Department of Electrical and Electronics Engineering
New Horizon College of Engineering
Bangalore, India

This work was developed as a collaborative conceptual research study by the two team members.

---

## Research Areas

**Quantum Computing · Robotics · ROS 2 · QAOA · QUBO · Path Planning · Autonomous Systems**

---

### Project Status

**Conceptual Research — Proposed Approach**

**Concept Date:** 04 October 2025

**Implementation / Experimental Validation:** Not yet performed
