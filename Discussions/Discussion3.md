# Name: Chetana Adhikari
##Date: 12/6/2017
###ISTA-320 Discussion 3

1. What are the two scenarios in which you can use PLINQ to speed up operations? Why does using PLINQ in these scenarios speed up processing?
In many scenarios, PLINQ can significantly increase the speed of LINQ to Objects queries by using all available cores on the host computer more efficiently. This increased performance brings high performance computing power onto the desktop.

2. How does AsParallel qualify as an extension method? First, explain what an extension method is and how you define extension methods, and them explain why AsParallel q
Through an extension method one can extend an existing type with additional static methods without affecting the existing code. These static methods become immediately available to your code in any statements that reference data of the type being extended. The AsParallel method extends the ParallelQuery class that acts in a similar manner to the original, except that it provides parallel implementations of many of the LINQ operators, such as join and where.

3.How do you cancel a PLINQ query before it finishes? Be specfic with respect to the variables and methods used for the cancellation operation, and how the variables and methods are used.
To cancel a PLINQ query before it finishes, you specify a CancellationToken object from a CancellationTokenSource and use the WithCancellation extension method of the ParallelQuery. 

4.Why is it important to synchronize concurrent access to a server? Give an example of a specific condition that will cause an error in your application if concurrent access is not synchronized.
It is important to synchronize concurrent access because if a task stores a value in a variable, it needs to ensure that another task doesn't modify that variable before it has a chance to read it. 

5.What does the lock statement do?
The lock statement attempts to obtain a mutual-exclusion lock over the specified object (you can actually use any reference type, not just object), and it blocks if this same object is currently locked by another thread. 

8.Explain how thread safe collection classes are made thread safe.
The methods in thread safe collection classes like ConcurrentBag<T> have to lock and unlock data to guarantee thread safety.
