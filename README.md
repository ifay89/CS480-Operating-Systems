# CS480-Operating-Systems
This is my small project for course CS480
The task in this project is write a C code to implement SJF for any number of processes and useing liunx command to display and run the code.
This some information about SJF:



Algorithm:

  Shortest Job First (SJF) is an algorithm in which the process having the smallest execution time is chosen for the next execution. This scheduling method can be       preemptive or non-preemptive. It significantly reduces the average waiting time for other processes awaiting execution. The full form of SJF is Shortest Job First.

basically, two types of SJF methods

1. Non-Preemptive SJF:

   In non-preemptive scheduling, once the CPU cycle is allocated to process, the process holds it till it reaches a waiting state or terminated.

2. Preemptive SJF:

   In Preemptive SJF Scheduling, jobs are put into the ready queue as they come. A process with shortest burst time begins execution. If a process with even a shorter    burst time arrives, the current process is removed or preempted from execution, and the shorter job is allocated CPU cycle.






Steps:

Step 1: 
Create a list of processes with their arrival times and burst times.

Step 2: 
Sort the list of processes in ascending order based on their arrival times.

Step 3: 
Initialize a variable "time" to the arrival time of the first process in the sorted list.

Step 4: 
Initialize a list "ready queue" with the first process in the sorted list.

Step 5: 
Initialize a variable "current process" with the first process in the ready queue.

Step 6:
For each subsequent process in the sorted list, check if its arrival time is less than or equal to the current time. If it is, add it to the ready queue.
 
Step 7:
Sort the ready queue in ascending order based on their burst times.

Step 8:
Set the current process to the first process in the ready queue.

Step 9:
Set the current time to the current time plus the burst time of the current process.

Step 10: 
Remove the current process from the ready queue and add it to a list of completed processes.

Step 11: 
Repeat steps 6-10 until all processes have been added to the list of completed processes.

Step 12: 
Calculate the turnaround time and waiting time for each process using the completion time and arrival time.
Using:  - turnaround time = waiting time + burst time 
        - waiting time = turnaround time - burst time
        
Step 13: 
Return the list of completed processes along with their turnaround and waiting times.


The Output will be like:

![image](https://user-images.githubusercontent.com/94137414/209414627-729836be-d7d8-4b5c-913f-36a858d4dbfa.png)

