# Exp.No: 11  
# PRIORITY QUEUE

## AIM :

To implement a Python program to calculate the Average Waiting Time and Average Turnaround Time for a set of processes using the First Come First Serve (FCFS) scheduling algorithm.

## ALGORITHM :

Step 1 : Input the burst times of all processes.

Step 2 : Initialize waiting time (wt) and turnaround time (tat) arrays.

Step 3 : Set waiting time of the first process to 0.

Step 4 : For each process from 2nd onward, calculate:

         wt[i] = wt[i-1] + bt[i-1]

Step 5 : Calculate turnaround time for each process as:

         tat[i] = wt[i] + bt[i]

Step 6 : Display burst time, waiting time, and turnaround time for each process.

Step 7 : Compute and print the average waiting time and average turnaround time.

## PROGRAM : 

```
# Python3 program for implementation
# of FCFS scheduling

# Function to find the waiting
# time for all processes
def findWaitingTime(processes, n,
					bt, wt):

	# waiting time for
	# first process is 0
	wt[0] = 0

	# calculating waiting time
	for i in range(1, n ):
		wt[i] = bt[i - 1] + wt[i - 1]

# Function to calculate turn
# around time
def findTurnAroundTime(processes, n,
					bt, wt, tat):

	# calculating turnaround
	# time by adding bt[i] + wt[i]
	for i in range(n):
		tat[i] = bt[i] + wt[i]

# Function to calculate
# average time
def findavgTime( processes, n, bt):

	wt = [0] * n
	tat = [0] * n
	total_wt = 0
	total_tat = 0

	# Function to find waiting
	# time of all processes
	findWaitingTime(processes, n, bt, wt)

	# Function to find turn around
	# time for all processes
	findTurnAroundTime(processes, n,
					bt, wt, tat)

	# Display processes along
	# with all details
	print( "Processes Burst time " +
				" Waiting time " +
				" Turn around time")

	# Calculate total waiting time
	# and total turn around time
	for i in range(n):
	    total_wt=total_wt+wt[i]
	    total_tat=total_tat+tat[i]
	    print(" "+str(i+1)+"   "+
	              str(bt[i])+"  "+
	              str(wt[i])+"    "+
	              str(tat[i]))
	print( "Average waiting time = "+
				str(total_wt / n))
	print("Average turn around time = "+
					str(total_tat / n))

# Driver code
if __name__ =="__main__":
	
	# process id's
	processes = [ 1, 2, 3]
	n = len(processes)

	# Burst time of all processes
	t0=int(input())
	t1=int(input())
	t2=int(input())
	burst_time = [t0,t1,t2]

	findavgTime(processes, n, burst_time)

```

## OUTPUT : 

![image](https://github.com/user-attachments/assets/01da449b-3e06-4907-b8dc-0e74d2aa5625)

## RESULT : 

Thus the implemention of a Python program to calculate the Average Waiting Time and Average Turnaround Time for a set of processes using the First Come First Serve (FCFS) scheduling algorithm is successfully verified.

