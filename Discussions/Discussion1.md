#Name:Chetana Adhikari
##Date: 12/6/2017
###Discussion 1

1. List two reasons for multitasking, and explain the rationale for them.
Multitasking, in an operating system, is allowing a user to perform more than one computer task (such as the operation of an application program) at a time. 

2.Explain Moore's law. What does Moore's law have to do with multitasking?
Moore noticed that the number of transistors per square inch on integrated circuits had doubled every year since their invention.
Based on this observation he predicted that this trend will continue into the foreseeable future.

3.In UWP, what namespace is used as the container for the multitasking methods?
System.Threading.Tasks.

4.What is the difference between tasks and threads? Explain.
A task is a set of program instructions that are loaded in memory.A thread of execution results from a fork of a computer program into two or more concurrently running tasks. The implementation of threads and processes differs from one operating system to another, but in most cases, a thread is contained inside a process.

5.What is the ThreadPool?
A thread pool is a collection of worker threads that efficiently execute asynchronous callbacks on behalf of the application.

6.What parameters does the Task() constructor take?
The Task() constructor is overloaded, but all versions expect you to provide an Action delegate as a parameter.

7.How do you start a thread?
You start a thread by using the Start() method of the task object. So if your task variable was named mytask, you would use mytask.Start();.


