---
layout: project
type: project
image: img/Queue.png
title: "Queue Simulation"
date: 2024
published: true
labels:
  - Java
  - Software Engineering
  - Simulation
summary: "This Java program simulates customer queueing and service times using either a single queue or multiple queues, comparing their total wait times over the course of a day."
---

<img class="img-fluid" src="../img/line.png">

This Java program simulates a queue system for servicing customers using either a single queue or multiple queues. The program generates random customer arrival and service times, then sorts the customers by their arrival time. It evaluates the system's performance by calculating the total wait time for all customers.

### Key Components:
1. **Customer Class**: Each customer has a randomly generated arrival time (between 0 and 86,099 seconds, equivalent to a full day) and a service time (between 30 and 300 seconds). It implements the Comparable interface to sort customers by arrival time.

2. **Server Class**: Represents a service provider that tracks when it will finish serving a customer. Servers can be idle or busy based on the current time.

3. **Queue Management**: The program can simulate one queue or 10 parallel queues. The method shortestQueueIndex identifies the queue with the fewest customers.

4. **Simulation Logic**:
   - Customers are generated and sorted by their arrival time.
   - Each customer is assigned to the shortest queue.
   - Servers process customers, and the total waiting time is calculated for both single-queue and multiple-queue configurations.

### Method:
- simulator(boolean singleQueue, int numCustomers): This method simulates customer servicing. It runs a loop over the course of a day (86,400 seconds), managing customer arrivals, assigning them to queues, and having servers process them. It calculates the total waiting time for all customers based on the selected queue configuration (single or multiple queues).

### Main Execution:
The program simulates customer servicing for 5,000 customers using both a single queue and 10 queues. It prints the total wait time for each configuration, allowing comparison between the two queue structures.

This system is useful for evaluating queue performance and can help determine whether single or multiple queues lead to more efficient customer service.
