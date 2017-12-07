#Name: Chetana Adhikari
##Date: 12/6/2917
###Discussion 2

1.What is an asynchronous method? When the book talks about a contract, what is the contract and who is it with?
In multithreaded computer programming, asynchronous method invocation (AMI), also known as asynchronous method calls or the asynchronous pattern is a design pattern in which the call site is not blocked while waiting for the called code to finish. Instead, the calling thread is notified when the reply arrives.

2.What can be the problem with decomposing a series of discrete method calls into a set of tasks, such as we saw in chapter 23?
It can create problems during multitasking.

3.What can be the problem with decomposing a series of discrete method calls into a set of continuations? What does the last continuation "complete" as compared to the previous continuations?
It can create problems with multitasking.

4.What might be the problem with implementing to previous solution as a continuation passing a delegate? What would be interpretation with this error message:"The application called an interface that was marshaled for a different thread"?
A continuation simply specifies an operation to be performed when a given task completes. The .NET Framework automatically executes the continuation operation as a task that it schedules when the original task finishes.

5. The book suggests a solution using a continuation delegate calling another continuation delegate via an anonymous function. What does the book identify as a problem with this suggested solution?

6.What does the async modifier do? What does the await operator do?
An await expression can occur only in the body of its enclosing method, lambda expression, or anonymous method, which must be marked with an async modifier. The term await serves as a keyword only in that context. Elsewhere, it is interpreted as an identifier. 

7. What is awaitable object? Be specific?
There's also a keyword dedicated to pull a value from a coroutine: await. Given an awaitable, await tries to get a value from it, and if the awaitable suspends, await also suspends the current coroutine, and so on, up to the .send() caller.

8. In a method definition, how do you create and run a Task and return a reference to the Task?
When you create a task, you give it a user delegate that encapsulates the code that the task will execute. The delegate can be expressed as a named delegate, an anonymous method, or a lambda expression.

