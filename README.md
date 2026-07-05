# CPU Scheduling Algorithm Visualizer

A browser-based tool that simulates and visualizes classic CPU scheduling algorithms with Gantt charts and performance metrics.

## Features
- Add/edit/remove processes (arrival time, burst time, priority)
- Simulates four scheduling algorithms:
  - First Come First Served (FCFS)
  - Shortest Job First (Non-Preemptive)
  - Round Robin (with configurable time quantum)
  - Priority Scheduling (Non-Preemptive, lower number = higher priority)
- Interactive Gantt chart with per-process color coding
- Auto-calculated metrics: completion time, turnaround time, waiting time, and averages

## Tech Stack
Vanilla HTML, CSS, and JavaScript — no frameworks or build step required.

## How to Run
1. Clone this repo
2. Open `scheduler.html` in any modern browser

No installation or server needed.

## How it Works
Each algorithm is implemented as a pure function that takes the process list (and quantum, for Round Robin) and returns a list of Gantt chart segments plus completion times. Metrics (turnaround time, waiting time) are derived from completion time, arrival time, and burst time:

```
Turnaround Time = Completion Time - Arrival Time
Waiting Time = Turnaround Time - Burst Time
```

## Possible Extensions
- Preemptive SJF (Shortest Remaining Time First)
- Preemptive Priority Scheduling
- Multilevel queue scheduling
- Export results as CSV/PDF

## Author
Mahesh — B.Tech IT, Sipna College of Engineering & Technology
