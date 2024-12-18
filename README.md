# Data Race with Raw Pointers in Rust
This repository demonstrates a common error in Rust when dealing with raw pointers and mutable references. The code modifies the value pointed to by the raw pointer, which can lead to data races or undefined behavior if not managed correctly. The solution demonstrates a safer approach using proper memory management and avoiding potential data races.
## Bug
The `bug.rs` file contains the buggy code. The main issue is directly modifying the memory location pointed to by a raw pointer without considering potential data races or memory safety violations. This approach can lead to unpredictable and unreliable behavior. 
## Solution
The `bugSolution.rs` file presents a safer and more reliable method. It correctly manages memory and avoids potential data races by using safe Rust techniques.