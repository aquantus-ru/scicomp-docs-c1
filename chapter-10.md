# CHAPTER 10: Operating Systems & Concurrency

The OS manages hardware resources and provides services for programs.

## 1. Kernel vs. User Space
- **Kernel Space**: Where the core of the OS executes. Has full access to hardware and memory. Crashing here brings down the system.
- **User Space**: Where applications run. restricted access. System calls (syscalls) are used to request kernel services (e.g., reading a file). This separation ensures stability and security.

## 2. Process and Thread Management
- **Process**: An instance of a running program. Isolated, has its own memory space. Heavyweight context switching.
- **Thread**: A unit of execution within a process. Shares memory with other threads in the same process. Lightweight context switching.
- **Scheduling**: The OS scheduler decides which process/thread runs on the CPU (Round-robin, Priority-based).

## 3. Deadlocks and Race Conditions
- **Race Condition**: Occurs when multiple threads access shared data simultaneously and the outcome depends on the timing of execution. Solved using synchronization (locks, semaphores).
- **Deadlock**: A situation where two or more processes are blocked forever, each waiting on a resource held by the other.
  - Necessary conditions (Coffman conditions): Mutual Exclusion, Hold and Wait, No Preemption, Circular Wait.

## 4. Virtual Memory and Paging
**Virtual memory** gives processes the illusion of a large, contiguous memory space, even if physical RAM is fragmented or full.
- **Paging**: Memory is divided into fixed-size blocks called pages.
- **Page Table**: Maps virtual addresses to physical addresses.
- **Page Fault**: Occurs when a program accesses a page not currently in RAM. The OS swaps it in from the disk (swap space). Excessive paging leads to "thrashing."
