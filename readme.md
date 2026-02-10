# CSCI 8530 Advanced Operating Systems Project

## Topic
Debugging Containerized Applications

## Description
This project examines how containerization affects operating system level performance, with a focus on overhead introduced during context switches and I/O handling.

We compare:
- Polled I/O vs interrupt-driven I/O
- Docker-based workloads vs native execution

The analysis focuses on whether interrupt handling, Interrupt Vector Table (IVT) usage, and processor state saving introduce measurable performance overhead.
The goal is to better understand container-related performance costs and their implications for OS-level debugging.

## Team
- Christian Theisen
- An Vu
- David Wang  
