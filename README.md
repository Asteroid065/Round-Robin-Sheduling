# Round-Robin-Sheduling

Introduction:

Round-robin scheduling algorithm is one of the simplest scheduling algorithms. It is designed especially for time-sharing systems.
The ready queue is treated as a circular queue. The algorithm assigns a time slice (also called time quantum) to each process in the 
ready queue in order, handling all processes without priority. A maximum of one time slice is allocated at once.
If the remaining request is less than a time slice, only the remaining request time is allocated. 
Round-robin scheduling is both simple and easy to implement. It is also starvation-free.

The project may be used to find the scheduling order, the average turn-around time and average wait time when round-robin scheduling is applied.
About the Code

The code is very simple. The design consists of a class roundrobin. This class consists of functions:

    read()

    This function is used to read the input to an object of this class. The inputs required are:
        n: The number of processes
        a[]: The arrival times of processes
        rq[]: The request times of processes
        q: The time quantum
        
    calc()

    This function is used to calculate:
        t[]: The turnaround time of each process
        w[]: The wait time of each process
        order: The scheduling order 
        
    display()

    This function does two tasks:
        Calculates tav and wav, the average turn-around time and average wait time respectively,
        from t[] and w[] respectively.
        Displays the scheduling order and the average turn-around and average wait time.


ABOUT THE CODE:-

    The code uses for loop which terminates when all processes have completed.
    j is used to count the number of processes completed.
    i is used to consider a process for scheduling in the circular-queue fashion.
    The array r[] is used to keep note of the remaining request of each process.
    sp gives the time spent till the given instant. 
    
    
    
REFERENCE FROM: 
    Silberschatz, Galvin and Gagne; Operating System Concepts; Sixth Edition; Wiley
    WIKIPEDIA
    CODE PROJECT: KBSBNG
