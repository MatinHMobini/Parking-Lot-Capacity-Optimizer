# Parking Lot Capacity Optimizer

## Project Overview

This project simulates a parking lot to determine the optimal number of parking spots required to avoid excessive queue buildup at the entrance. The goal is to find the minimum number of parking spots needed to efficiently manage car arrivals and departures while preventing underutilization.

## Key Features

- **Simulation of Parking Lot**: The simulation runs for 24 simulated hours, with varying numbers of parking spots to determine the smallest number that meets demand.
- **Queue Management**: The simulator tracks the size of the entrance queue and adjusts the parking lot size to ensure the average queue length remains under a specified threshold.
- **Repetitive Simulation**: To account for random variations in car arrivals and departures, the simulation is repeated multiple times, averaging the results to ensure accuracy.
- **Exception Handling**: Implemented robust exception handling for key methods to ensure the program runs smoothly even with unexpected inputs.

## How It Works

1. **Initialization**: The simulation starts with a single parking spot and progressively increases the number of spots.
2. **Repetitive Simulation**: For each number of spots, the simulation runs 10 times, each for 24 simulated hours.
3. **Queue Length Evaluation**: After each simulation, the average length of the entrance queue is calculated. If the average queue length is ≤ 5, the current number of spots is deemed sufficient.
4. **Output**: The program outputs the smallest number of spots required to meet demand, along with the simulation details.

## Files

- **CapacityOptimizer.java**: Implements the main algorithm to find the optimal number of parking spots.
- **ParkingLot.java**: Manages parking spot allocation using lists.
- **Simulator.java**: Handles the simulation logic, including car arrival and departure.
- **LinkedQueue.java**: Implements the queue used for managing the entrance queue.
- **Additional Files**: Various support files like Car.java, Queue.java, and others provided as-is or with minor adjustments.

## Usage

To run the simulation:

```bash
java CapacityOptimizer <hourly rate of arrival>
```

Example:

```bash
java CapacityOptimizer 11
```

This command runs the simulation for a car arrival rate of 11 cars per hour.

Thanks for viewing!
