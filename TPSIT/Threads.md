# What are threads
Threads are light tasks that can do small tasks and are more interactive than processes with other threads. These can be defined as "light processes" but it's an inaccurate description. 

# TCB
Or Thread Control Block, they work like the [[Processes#Process Control Block|PCB]] in a process but it doesn't contain the full code pointer but just a pointer to the processes' PCB Code pointer, that points only to the function(s) needed by the thread.