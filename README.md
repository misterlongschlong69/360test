Question 1->semaphores and threads
Question 3->threading+pipes
Question 5-> Server
Question 7 ->Client

Threads are more lightweight, have access to shared data, creating a thread is easier, switching between threads in a process is easier than switching between processes but difficult to write and debug code. Processes have memory protection and fault tolerance.

During a process fork the working directory, heap and threads are copied. Handle requests in child processes so not in serial.

Threads have individual granularity for program counter stack allocation.

Function pointers breakdown: https://denniskubes.com/2013/03/22/basics-of-function-pointers-in-c/

For multi user chat room use TCP multithreading for data sharing, each thread caters to one user
For web server running user CGI programs use TCP with fork to handle requests
For game server use UDP with recv() on a thread

