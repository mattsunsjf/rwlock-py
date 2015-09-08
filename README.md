# rwlock-py
A writer-biased Reader-Writer Lock

Forked from: http://code.activestate.com/recipes/577803-reader-writer-lock-with-priority-for-writers/
Original Author: Mateusz Kobos http://workshop.mkobos.com/

The enhancement based on original implementation:
- Protect the critical section of writer-acquire and writer-release. Several writers waiting for readers to release the lock will get the lock in the order of arriving time.
