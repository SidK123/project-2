# Project 2: Dynamic Analysis using VM Instrumentation

This project involves developing a set of dynamic analyses which we will use to 
learn more about runtime properties of Wasm bytecode. For this project, we will
be using the [Wizard](https://github.com/titzer/wizard-engine.git) research
Wasm engine. Wizard allows users to specify dynamic instrumentation for Wasm
programs using [monitors](https://dl.acm.org/doi/10.1145/3620666.3651338).
Monitors can attach probes, which are VM-level operations which run atop
Wasm bytecode. Wizard already contains a comprhensive suite of monitors, which
you can find in `wizard-engine/src/monitors/`, or you can read documentation 
[here](https://github.com/titzer/wizard-engine/blob/master/doc/Monitors.md).

In this project, you will implement your own monitors for wizard. You are 
required to implement **any 3** the following four monitors:

1. [Instruction Class Monitor](docs/iclass.md)
2. [Memory Allocation Monitor](docs/malloc-prof.md)
3. [Path Profiling Monitor](docs/path-prof.md)
4. [Cache Simulation Monitor](docs/cache-prof.md)

In order to enable grading, we enforce an output specification for each monitor 
that is expected to be met. See each link for details.

Since Wizard is implemented in the Virgil programming language, you will also
have to write your monitors in Virgil. See the link below for how you can get
Virgil (and Wizard).

We have provided some tests and expected output with each monitor in `tests`.
Unlike project 1, there's no specific requirement to write test programs. 
Although you probably should, anyway.

## Submitting the Project

This repo serves as the project specification. Like project 1, please make a
private fork of this repo.

For grading, we would like you
to add your new monitors to this exact commit hash of 
[Wizard](https://github.com/titzer/wizard-engine/tree/b58bfdff631500a5c57f057b32a1e5b702b3197c),
and build it with this exact commit hash of 
[Virgil](https://github.com/titzer/virgil/tree/a72a35f7f139706c1db293c4e239f735196db4bf).
Note that these aren't the HEAD of the main branch since both Virgil and Wizard
are under active development. We intend to use these exact commits specified
for grading. 

Make sure all the implemented monitors are present within `src/monitors` in the
repository during submission (and are not hidden inside the `wizard-engine`
submodule. Submit your code on Gradescope.



