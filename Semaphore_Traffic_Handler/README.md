# OS-CA1 – Concurrent Intersection Traffic Simulation

This project was completed as part of an **Operating Systems assignment**.  
Based on the provided skeleton and assignment requirements, the project was completed to simulate vehicle movement through a **multi-lane intersection** using **concurrency**, **synchronization**, and **Weighted Round Robin scheduling**.

## Overview

The simulator models vehicles arriving from different lanes and manages their movement through the intersection safely and fairly.  
Each vehicle is defined by attributes such as:

- `vehicle_id`
- `vehicle_type`
- `priority`
- `lane`
- `route`
- `crossing_time`

Vehicles are placed in lane-based queues, and the system decides which lane should be served next using the **Weighted Round Robin** policy.

## Features

- Multi-lane intersection simulation
- Lane-based vehicle management
- Weighted Round Robin scheduling
- Priority-aware vehicle handling
- Safe vehicle entry and exit
- Concurrent execution using threads
- Synchronization for shared intersection control

## Core Functions

The project includes the main required functions of the assignment:

- `get_next_lane`
- `can_enter_intersection`
- `enter_intersection`
- `exit_intersection`
- `is_lane_turn`

## Implementation Note

This project was initially provided as a **base/skeleton**, and the required logic was completed and extended according to the assignment description.

## Run
```bash
python3 main.py
