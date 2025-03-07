# FOS - Operating System Project  

## Overview  

The **FOS (Faculty Operating System)** project is part of our **Operating Systems** course, structured into three milestones. Each milestone involves implementing various functions and system features, allowing us to gain hands-on experience in **operating system design** and **low-level programming**.  

## Learning Outcomes  

Throughout this project, we have learned:  

- The fundamentals of **OS-level programming**.  
- How **system calls** work and how to implement them.  
- **Dynamic memory allocation** strategies in user and kernel space.  
- **Process synchronization** using sleep locks and semaphores.  
- **Memory management** techniques such as paging and shared memory.  
- Implementation of **process scheduling algorithms**.  
- Handling **page faults** and **memory faults** efficiently.
- Ensure correctness by design  not testes 

## Project Structure  

The project is divided into **three milestones**, each focusing on different aspects of operating system functionality.  

### Milestone 1: Core OS Functions  

This milestone focuses on basic OS functionalities such as **command processing, system calls, dynamic memory allocation, and sleep locks**.  

#### Implemented Functions:  

- **Command Processing:** `process_command`  
- **System Calls:** Implementation of **three system calls**.  
- **Dynamic Allocator:**  
  - Block allocation: `alloc_block_FF`, `alloc_block_BF`  
  - Deallocation: `free_block`  
  - Reallocation: `realloc_block_FF`  
- **Sleep Locks:** `Sleep`, `Wakeup One`, `Wakeup ALL`, `Acquire`, `Release`  

### Milestone 2: Advanced Memory Management  

This milestone extends **memory management** to include **user heap, fault handling, and kernel heap operations**.  

#### Implemented Functions:  

- **User Heap:** `sys_sbrk()`, `malloc()`, `allocate_user_mem()`, `free_user_mem()`  
- **Fault Handling:**  
  - **Kernel Dynamic Alloc for a Process**  
  - **Check Invalid Pointers**  
  - `Page_fault_handler`  
- **Kernel Heap:**  
  - `kmalloc()`, `kfree()`, `kheap_virtual_address()`, `kheap_physical_address()`, `krealloc()`  
  - **Fast Page Allocator**  
- **Shared Memory:** `smalloc()`, `sget()`, `createSharedObject()`, `deleteSharedObject()`  

### Milestone 3: Process Management & Scheduling  

The final milestone covers **fault handling improvements, process scheduling, and synchronization**.  

#### Implemented Functions:  

- **Fault Handling:** `Nth Chance Clock Replacement`  
- **User-Level Semaphores:** `Create Semaphore`, `Get Semaphore`, `Wait Semaphore`, `Signal Semaphore`  
- **Priority RR Scheduler:**  
  - `Set Process Priority & Threshold`  
  - `Initialize Priority RR Scheduler`  
  - `Schedule Next Process`  
  - `Timer Tick Handler`  

## Conclusion  

The **FOS project** has provided valuable experience in understanding how **operating systems manage memory, processes, and system resources**. Through this project, we have gained **practical insights into system-level programming**, which will be beneficial for future **OS-related development and research**.  

This project not only strengthened our **C programming skills** but also enhanced our ability to design **efficient and optimized system software**. 
