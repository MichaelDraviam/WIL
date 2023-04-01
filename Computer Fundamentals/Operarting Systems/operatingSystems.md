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

Simple batch systems uses software known as `Monitor`, which interfaces with the processor directly and refrains users from accessing the processors directly.

>User fed an input to the computer operator, who gathered similar jobs(tasks to be performed) and placed an entire batch (group of similar type tasks) for utilization by the Monitor.

>Each program is built to branch back to the monitor when it completes processing.
At this point, the monitor automatically begins loading the following program.

With Batch OS, Processor time alternates between their execution of the user's program and the execution of the Monitor.

However, now some main memory is given to the monitor, and the monitor consumes some processor time.Both of these are some forms of overhead. 

Despite this overhead, simple batch systems improve the utilization of the processor.

>Monitor is the bouncer to the processor, it takes multiple tasks/batch at a time. and Monitor montiors the end of the batch too :wow: and runs following programs.

**`Multi-programmed Batch Systems:`**

Inspite of the automatic job sequencing provided by the Simple Batch OS, the processor is often idle.

The culprit is `I/O devices are much slower than processors in terms of speed`.
so main idea of Multi Batch is while one job is waiting on I/O, OS could hotswap/switch to a different task/job asnd start executing that.

When the I/O devices finished execution, then we again swap back to the first job,resume where we left off.
simple enough.

![multi programmed batch system](../../images/Computer%20Fundamentals/Operating%20Systems/multi-programmed-batch-systems.jpeg "multi programmed batch system")

**`Time-Sharing Systems:`**

If we wanted to give user interaction directly to the computer, instead of waiting on the processor to return control to the OS for each run.
What can be done is have a system clock interrupt at a rate of around 0.2 seconods.

At each interrupt, the OS reclaims control and could assign the processor to another user.

This is called `time slicing`,
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
- `Handles overhead of setting up apps to run`
- `GUI/CLI for users`

### **Disadvantages of OS:**

- `Higher memory access times`
- `Language behind OS is complex`
- `Meh there are more but who cares`

---

## **Types of Operating System**

---

### **Batch OS:**

A batch operating system grabs all programs and data in the batch form and then processes them.

Main idea is to decrease set-up time while submitting simialar jobs to the CPU.

A batch monitor is started for executing all pooled jobs, after removing them.

![batch os](../../images/Computer%20Fundamentals/Operating%20Systems/batch-os.jpeg "batch os")

**`Advantages:`**

- All jobs performed in repeating form without user's permission

- Can feed input data in the batch processing system without using extra hardware components.

- less time to execute all jobs.

- multiple users per system.

- idle time is less.

- can specify a time to execute when the system is idle.

- can handle large repeated work.

**`Disadvantages`**

- Jobs could end up in infinite loop.

- difficult to debug batch systems.

### **Time-sharing OS**

CPU runs multiple jobs by switching quickly among them, its so frequent the users can interact with each program without percieved delays.

TS-OS uses `CPU Scheduling` and `multi-programming` to provide each user with a small portion of time-shared computer.

TS-OS jobs are kept simultaneously in memory, so system must have memory management and protection.

![time-sharing os](../../images/Computer%20Fundamentals/Operating%20Systems/time-sharing-operating-system.jpeg "time sharing os")

**`Advantages:`**

- Tasks get equal opportunity.
- Fewer chances of duplication of software.
- CPU Idle time is reduceed.

**`Disadvantages:`**

- Reliability Problem.
- Security and integrity of user programs and data.
- Data communication problem.

### **Distributed OS**

Distributed OS has entire system across multiple central processsors, All processes connected through high-speed buses or ethernet.

Distributed OS also known as `lossely coupled systems`.
invlove multiple computers,nodes and sites.

Distributed OS can share computational capacity and I/O files while also allowing virtual machine abstractions for users.

![distributed os](../../images/Computer%20Fundamentals/Operating%20Systems/distributed-operating-system.jpeg "distributed os")

**`Advantages:`**

- Shares all resources from one site to another,increasing data availability across the entire system.

- Reduces probability of data corruption, because of replicated data.

- If one node fails others can still carry on.

- Helps reduce data processing time.

**`Disadvantage:`**

- System must decide which jobs to execute when and where to execute.
    The Scheduler has limitations, which can lead to underutilized hardware and unpredictable runtimes.

- Hard to implement security across all Nodes.

- More distributed more the latency.

- Monitoring,gathering,processing across the Nodes can be an issue.

### **Network OS:**

Connects computers and devices into local-area network.

1. **Peer-to-Peer Network OS:**

    allows users to share network resources saved in a common, accesible network location.

    all devices are treated equally,and its cheaper.
2. **Client/Server Network OS:**

    Provides users with access to resources througgh a server.

![network os](../../images/Computer%20Fundamentals/Operating%20Systems/network-operating-system.jpeg "network os")

**`Advantages:`**

- Higly stable centralized servers.
- Security concerns are handled through servers.
- Server access is possible remotely from different locations and types of systems.

**`Disadvantages:`**

- Servers are expensive.
- User has to depend on central location for most operations.
- Maintenance and updates are required regularly.

### **MultiProcessor OS:**

Utilizes multiple processorss connected with Physcial memory,Computer Buses,Clocks.

it's main objective is to consume high computational power and increase execution speed.

![multiprocessor os](../../images/Computer%20Fundamentals/Operating%20Systems/multiprocessor-operating-system.jpeg "multiprocessor os")

**`Advantages:`**

- Great Reliability.
- Improve Throughput.
- Cost-Efficient.
- Parallel Processing.

**`Disadvantages:`**

- Speed can degrade due to one failing processor.
- needs context switching, can impact performance.
