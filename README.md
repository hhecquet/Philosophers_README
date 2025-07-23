# Philosophers

> [!IMPORTANT]
> None of my code is publicly available here, but if you're a recruiter, I'd be happy to share it with you upon request.

<p align="center"> 
<img width="317" height="270" alt="Screenshot from 2025-07-23 15-12-33" src="https://github.com/user-attachments/assets/ff747202-bc39-406b-8b8f-ad117a654685" />
</p>

The ***Philosophers*** project is a classic concurrency challenge at 42 that simulates the Dining Philosophers problem — a fundamental exercise in understanding multithreading, synchronization, and resource sharing. The goal is to create a program where multiple philosopher threads alternately think, eat, and sleep without causing deadlocks or starvation.
This project deepened my knowledge of thread management and synchronization primitives in C, reinforcing the importance of careful concurrency control.

What I had to do:
* Create philosopher **threads** that perform actions in cycles: *think*, *eat*, and *sleep*
* Use **mutexes** to represent *forks* and protect shared resources
* Prevent **deadlocks** by implementing strategies to control fork acquisition order
* Manage timing accurately so philosophers eat for the specified time, then sleep and think accordingly
* Detect if a philosopher dies by not eating within the allotted time and gracefully terminate the simulation
* Synchronize console output to avoid mixed or corrupted messages when multiple threads print simultaneously
* To accomplish this, I had to:
  * Use **pthread library** functions for thread creation, joining, and mutex handling
  * Implement timing functions with gettimeofday or similar to manage delays and timeouts
  * Design an efficient way to monitor philosophers’ states without busy waiting
  * Ensure safe access to shared variables and avoid race conditions

What I Learned:
* Fundamentals of multithreading and synchronization in C
* Using **mutexes** and locks to protect shared resources and prevent data races
* Strategies to avoid deadlocks and starvation in concurrent programs
* Accurate timing and sleeping within threads without blocking the entire program
* Writing robust, thread-safe code and managing the lifecycle of threads carefully

Philosophers taught me how challenging and subtle concurrency problems can be. It pushed me to think critically about synchronization and thread safety, preparing me for more complex multithreaded applications.
