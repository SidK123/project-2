# Project 2: Dynamic Analysis using VM Instrumentation

In this project, you will implement some dynamic analysis monitors for the [Wizard](https://github.com/titzer/wizard-engine.git)
Wasm engine.

You are required to implement **any 3** the following four monitors:

1. [Instruction Class Monitor](docs/iclass.md)
2. [Memory Allocation Monitor](docs/malloc-prof.md)
3. [Path Profiling Monitor](docs/path-prof.md)
4. [Cache Simulation Monitor](docs/cache-prof.md)

In order to enable grading, we enforce an output specification for each monitor that is expected to be met. See each link for details


## Submitting the Project

This repo serves as the project specification. For grading, we would like you to fork [Wizard](https://github.com/titzer/wizard-engine/tree/63e11f0343f4e4343660d9f395078b1083d69a2e) 
privately, and build it with this exact commit hash of [Virgil](https://github.com/titzer/virgil/tree/454a941b93ea25137d3ad12dcfdb8d82f1449d1b).
Note that these aren't the HEAD of the main branch since both Virgil & Wizard are under active development. 
We intend to use these exact commits specified for grading. 

Make sure all the implemented monitors are present within `src/monitors` in the repository during submission. Add the TA (Github ID: arjunr2) as a
collaborator to the project.



