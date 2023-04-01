# **Operating Systems**

---

## **What is Operating System?**

---

### **Introduction:**

OS Acts as the Interface between computer hardware components and the user.

OS is a software that manages computer hardware.

OS helps you communicate with the computer without knowing the computer's langauge.

>OS is the middle man between users/programs and the hardware.

### **Kernel:**

A Kernal is a special program, which handles most of the Tasks (Random-access memory,Input/Output devices,Resourc Management,Memory Management,Device Management) deligated by the OS.

![kernel in operating system](../../images/Computer%20Fundamentals/Operating%20Systems/kernel-in-operating-system.jpeg "kernel in operating system")

### **Types of Operating Systems:**

**`Simple Batch Systems:`**

Simple batch systems uses software known as monitor, which interfaces with the processor directly and refrains users from accessing the processors directly.

User fed an input to the computer operator, who gathered similar jobs(tasks to be performed) and placed an entire batch (group of similar type tasks) for utilization by the monitor.
Each program is built to branch back to the monitor when it completes processing.
At this point, the monitor automatically begins loading the following program.

With Batch OS, Processor time alternates between their execution of the user's program and the execution of the monitor.

However, now some main memory is given to the monitor, and the monitor consumes some processor time.Both of these are some forms overheaad. Despite this overhead, simple batch systems improve the utilization of the processor.

>Monitor is the bouncer to the processor, it takes multiple tasks/batch at a time. and Monitor montiors the end of the batch too :wow: and runs following programs.

**`Multi-programmed Batch Systems:`**

Inspite of the automatic job sequencing provided by the Simple Batch OS, the processor is often idle.
The culprit is I/O devices are much slower than processors in terms of speed.
so main idea off Multi Batch is while one job is waiting on I/O, OS could hotswap/switch to a different task/job asnd start executing that.
When the I/O devies finished execution, then we again swap back to the first job,resume where we left off.
simple enough.

![multi programmed batch system](../../images/Computer%20Fundamentals/Operating%20Systems/multi-programmed-batch-systems.jpeg "multi programmed batch system")

**`Time-Sharing Systems:`**

If we wanted to give user interactio directly to the computer, instead of waiting on the processor to return control to the OS for each run.
What can be done is have a system clock interrupt at a rate of around 0.2 seconods.

At each interrupt, the OS reclaims control and could assign the processor to another user.
This is called time slicing,
if we have n users interacting with the computer, each user sees 1/nth of the effective capacity.at regular time intervals.

each slice if the old user program code and data are inserted to main memory, for the program to execute in their next turn.
`turn tables`

### **Functions of Operating Systems:**

1. `GUI`  
2. `File Management`
3. `Memory Management`
4. `Security Management`
5. `Resource Management`

### **Advantages of OS:**

- `Reduces startup time of apps`
- `OS promotes abstraction`
- `Maximizes Processor Utilization`
- `Memory Protection between processes`
- `handles overhead of setting up apps to run`
- `GUI/CLI for users`

### **Disadvantages of OS:**

- `Higher memory access times`
- `Language behind OS is complex`
- `Meh there are more but who cares`

---

## **Types of Operating System**

---

### **Batch Operating Systems:**
