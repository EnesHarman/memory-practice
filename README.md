# Custom Memory Allocator with Visualization  

This project is based on the Rust code example from *Rust in Action*. The original code does not run on Apple M-series (ARM-based) machines due to the use of Thread Local Storage. To resolve this, I implemented alternative approaches to ensure compatibility.  

## Overview  

The project utilizes the [Piston game engine](https://github.com/PistonDevelopers/piston) to visualize memory usage in real time. Each dot on the screen represents a struct allocated on the heap using a `Box` pointer.  

A custom global allocator is implemented to track allocation metrics. Unlike the original example, these metrics are logged into a file instead of being printed to the console.  
