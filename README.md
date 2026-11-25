# Operating Systems Lab - Python Programs

Simple Python implementations of the Operating Systems lab experiments. Each program is a single file, uses hardcoded sample data (no input needed), and prints the output step by step so it is easy to follow.

## Experiments

| No. | Experiment | File |
|-----|-----------|------|
| 1 | Linux system calls, process creation using `fork()`, `exec()` and `wait()` | `exp01_fork_exec_wait.py` |
| 2 | Thread creation and management (POSIX threads equivalent using `threading`) | `exp02_threads.py` |
| 3 | CPU scheduling: FCFS, SJF, Priority and Round Robin | `exp03_cpu_scheduling.py` |
| 4 | Producer-Consumer problem using semaphores | `exp04_producer_consumer.py` |
| 5 | Readers-Writers problem using semaphores | `exp05_readers_writers.py` |
| 6 | Dining Philosophers problem using semaphores | `exp06_dining_philosophers.py` |
| 7 | Deadlock avoidance using Banker's Algorithm | `exp07_bankers_algorithm.py` |
| 8 | Contiguous memory allocation: First Fit, Best Fit, Worst Fit | `exp08_memory_allocation.py` |
| 9 | Page replacement: FIFO, LRU and Optimal | `exp09_page_replacement.py` |
| 10 | Disk scheduling: FCFS, SSTF, SCAN and C-SCAN | `exp10_disk_scheduling.py` |
| 11 | File allocation: Contiguous, Linked and Indexed | `exp11_file_allocation.py` |

## Requirements

- Python 3.8 or above
- No external libraries needed (only built-in modules like `os`, `threading`, `time`, `random`)
- Experiment 1 uses `os.fork()`, so it works only on **Linux / macOS**. On Windows, run it using WSL.

## How to Run

## Sample Outputs (quick check)

- Exp 7: Safe sequence = `P1 -> P3 -> P4 -> P0 -> P2`
- Exp 9: Page faults - FIFO = 15, LRU = 12, Optimal = 9
- Exp 10: Total head movement - FCFS = 640, SSTF = 236, SCAN = 331, C-SCAN = 382

## Notes

- Experiments 4, 5 and 6 use threads, so the order of output can change slightly on every run. This is normal.
- In Experiment 11, the disk has only 20 blocks, so a file may fail to allocate if there is not enough space. Change `DISK_SIZE` in the code to try bigger sizes.
- Sample data can be edited at the top of each file to test different inputs.

## Topics Covered

Process management, multithreading, CPU scheduling, process synchronization, deadlock avoidance, memory management, virtual memory (page replacement), disk scheduling, file system allocation.

