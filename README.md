# java_concurrency_in_practise

Finding the right balance of sequentiality and asynchrony is often a characteristic of efficient people

Locking is not just about mutual exclusion; it is also about memory visibility.

Semaphores are used to control the number of concurrent threads that are using a resource.

CountDownLatch allows one or more threads to wait until a set of operations being performed in other threads completes.

Semaphore Use cases:
1）Limiting concurrent access to disk (this can kill performance due to competing disk seeks)
2）Thread creation limiting
3）JDBC connection pooling / limiting
4）Network connection throttling
5）Throttling CPU or memory intensive tasks

CountDownLatch Use cases:
1）Achieving Maximum Parallelism: Sometimes we want to start a number of threads at the same time to achieve maximum parallelism
2）Wait N threads to completes before start execution
3）Deadlock detection.

