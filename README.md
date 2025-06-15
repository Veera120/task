==============================

Multithreaded Histogram (C++)
Description:

What This Program Does:
It creates 1 million random numbers between 0 and 255.
Then, it counts how many times each number appears (this is called a histogram).
It does this in two ways:
One by one (normal way)
Using 8 threads at the same time (faster way)
Why Two Ways?
The first way (sequential) is simple but slow.
The second way (multithreaded) is faster because it splits the work into 8 parts.
How It Works:
Data is generated randomly.
Histogram is calculated in both ways.
Time taken by each method is shown.
It checks if both results are the same.
How to Run:
Save the code as histogram.cpp
Open terminal or command prompt.
Compile: g++ histogram.cpp -o histogram -std=c++17 -pthread
Run: ./histogram
Sample Output:
Running Sequential Histogram... Running Multithreaded Histogram (8 threads)...

Summary: Sequential Time : 11 ms Multithreaded Time: 1 ms Histograms Match : YES