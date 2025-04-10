WIP

Workloads

 - restaurants, orders, and chef analogy (especially with regards to context switching costs)
 - why it's important to break workload into seemingly large chunks
 - why it's also important to keep the large chunks reasonable so no thread is idle
 - worker queue pattern
 - How to determine size of workloads?
 - How Battle Critters does it, and the pros and cons of this, as well as in-game factors that may affect performance
 - Explore other hypothetical RTS games and their specs, and how their multithreaded workloads could play out

Synchronization

 - back to the restaurant analogy, then say lmao we just ignore all that. Why?
 - race condition? why it's not an issue here due to 32 bit data types and SIMD data types
 - thread contention? why it's not an issue here because of the intentional omission of any synchronization. Explain the costs of mutexes and spin locks
 - Cache pollution? Explain the consequences of multiple cores having their own L1 caches.
 - Keep in mind that thread scheduling and waiting is still needed to form job chains.
