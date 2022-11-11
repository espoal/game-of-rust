# Introduction

Learning Rust as if it was a game: start with the easy mode, write some code and then move
on to the next difficulty level. The goal is to reduce the entry barrier and to reduce
the large gap between when you start learning and when you star using, because usage
is what drives proficiency in the language

At the end of easy mode you will be able to write a lot of code, although single threaded
and not very efficient. Normal mode will let you face with the infamous borrow checker,
the nightmare of many young rustaceans. The hard mode is where the real heros shine:
unsafe, no_std and other challanges.

Couple of hours per day, at the end of the first week you will be able to write Rust
code. Evolvability it's an important feature if you want to learn a language.


# About this book

# Why Rust

Not speed, not simplicity, but correctness, readibility and maintainability.
Use Rust for the code you plan to use a lot.

# The computer model

CPU, memory and I/O
Stack and heap

CPU is a small fleet of fighter jets, GPUs and accelerators are like cargo ships.
Both transport stuff, but with different speeds and latencies.
GPUs highly parallel, CPUs highly concurrent.

Fighter jets are more manouvreable, easier to adapt, but have low cargo.
With cargo ships you need to plan a lot.
For both memory patterns are important

- Registers (1 ns, few kb)
- Cache (1-10 ns, 1 kb - 128 mb)
- Ram (10-50 ns, 1 mb - 1 Tb)
- NVMe (50-150 ns, 1 Tb - 10 Tb)
- Disks (150-1000 ns, 10 Tb- 100Tb)
- Internet (1 ms - 100 ms, infinite)

Locality refers to the distance, measured as time, between different memory areas.

# Stack and heap

Stack is a small contiguous chunk of memory, which benefits from locality.
Heap is a large pool of memory, where speed is sacrified for capacity.