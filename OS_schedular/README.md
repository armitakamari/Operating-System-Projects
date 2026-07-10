# OS CPU Scheduling Simulator

An operating systems project that simulates CPU process scheduling using a modular, concurrent design.  
The project is built around three main components: **Process Generator**, **Scheduler**, and **CPU**, and models the execution of processes based on scheduling attributes such as arrival time, burst time, and start time.

## Overview

This project was developed as part of an Operating Systems course assignment.  
It demonstrates the core concepts of process scheduling, shared-resource coordination, and concurrent execution using multithreading and synchronization primitives.

The system is designed to:

- generate processes dynamically or read them from input,
- manage processes in a ready queue,
- schedule processes according to the selected policy,
- simulate CPU execution,
- and prevent race conditions using synchronization mechanisms.

## Features

- Modular architecture with separated responsibilities
- Process generation with timing attributes
- Ready queue management
- CPU scheduling simulation
- Concurrent execution using threads
- Protection of shared data using mutexes and semaphores
- Process state handling and execution flow control
- Clean separation between generator, scheduler, and CPU logic

## Project Structure

- **`ProcessGenerator`**  
  Responsible for creating processes and assigning scheduling-related attributes.

- **`Scheduler`**  
  Manages the ready queue and selects the next process for execution.

- **`CPU`**  
  Simulates the execution of the selected process.

- **`Process`**  
  Represents a process with attributes such as arrival time, burst time, and start time.

- **`Main`**  
  Entry point of the project.

- **`OSProject`**  
  Core project logic and overall coordination.

## Concurrency and Synchronization

Because multiple threads may access shared resources at the same time, the project uses:

- **pthread**
- **mutex**
- **semaphore**

These synchronization tools help coordinate the generator, scheduler, and CPU modules while avoiding race conditions and inconsistent states.

## Scheduling Concepts

The project is based on classic operating-system scheduling ideas such as:

- process arrival time
- burst time
- ready queue
- CPU dispatching
- synchronized process execution

Depending on the implementation, different scheduling policies can be supported or extended in the future.

## Requirements

- Java
- Standard concurrency support
- Compatible IDE such as IntelliJ IDEA or Eclipse

## How to Run

1. Clone the repository
2. Open the project in your Java IDE
3. Run `Main.java`

If you are using command line:
```bash
javac *.java
java Main

