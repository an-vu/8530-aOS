# CSCI 8530 Advanced Operating Systems Project

## Topic

Debugging Containerized Applications

## Overview

- This project investigates how containerization impacts operating-system–level performance, with a focus on context switching and I/O handling.
- Specifically, we analyze whether Docker-based execution introduces measurable overhead compared to native execution when using polled I/O and interrupt-driven I/O.

- Rather than treating containers as a black box, the project examines low-level mechanisms such as interrupt handling, processor state saving, and kernel scheduling behavior to better understand where performance differences originate.

## Scope and Assumptions

- Containers share the host kernel; no hardware virtualization is involved.
- Any observed overhead is assumed to originate from container abstraction, kernel scheduling behavior, or I/O stack interactions rather than guest kernels.
- Native and containerized executions are designed to differ only in the virtualization layer.

## Experimental Design

The experimental setup will be clearly defined and controlled, including:
- Linux kernel version
- Container runtime and configuration
- I/O subsystem and workload characteristics
- Polled I/O vs interrupt-driven I/O paths

Native execution serves as the baseline for comparison against containerized workloads.

## Measurement and Analysis

We will use appropriate low-level measurement techniques, such as profiling and tracing, to attribute observed overhead to specific mechanisms, including:
- Context switch frequency
- Interrupt latency
- System call paths
- Kernel scheduling behavior

Results will be interpreted at the mechanism level to determine whether differences arise from container abstraction, kernel behavior, or I/O stack interactions.

## Positioning

This project does not claim novelty in identifying container performance overhead. Instead, its contribution lies in:
- Careful experimental control
- Precise attribution of overhead sources
- Clear alignment with existing literature on container and kernel performance analysis

## Team

- Christian Theisen
- An Vu
- David Wang
