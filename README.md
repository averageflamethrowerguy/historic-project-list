# historic-project-list
A list of projects that I've worked on. These projects are not all public.
Projects are listed most-recent-first.



## ChungOS (Fall 2022)
### Please ask for access to this repository.
This is a simple operating system for CS58 (Operating Systems) following the Yalnix spec, as modified by Professor Sean Smith. It is probably my most impressive academic project to date. I wrote approximately 8,000 lines of C for this project. It has the following features:
1. Boots, intializing virtual memory and loading an init program
2. Handles switching between processes using traps (such as the clock trap)
3. Handles process sycalls, such as `Fork`, `Exec`, `Wait`, `Exit`
4. Implements communication and synchronization datastructures, such as pipes, locks, and cvars
5. Handles communicating with a user via multiple terminals.




## YAME (Yet Another Maze Escaper) (Fall 2022)
### Repository is here: https://github.com/averageflamethrowerguy/cs69-final-project
This is a maze escaper for CS69.13 (Multirobot Systems). Several robots start in unknown initial positions, and must completely explore a maze. I wrote approximately 2,500 lines of Python for this project.
1. Each robot will explore the maze using a wall-following algorithm, and a SLAM mapping approach.
2. When two robots are within line-of-sight of one another, they detect each other with cameras
3. They then initiate a map-merge, where each robot updates the other's map.
4. When a complete map is found, a connected traversal graph is generated with a feature-detection approach
5. Robots can then escape the map using a Djisktra's-algorithm approach.




## MIDI Keyboard Converter (Summer 2022)
### Please ask for access to this repository.
This is a MIDI keyboard converted for ENGS31 (Digital Electronics). When wired into a MIDI keyboard, this programs an FPGA to convert MIDI signals into the bits to drive an analog speaker. I wrote approximately 2,500 lines of VHDL for this project. It has the following components:
1. Byte Reader (Controller & Datapath). This reads the bitstream from the keyboard into byte-long chunks.
2. Finite State Machine. This reads the bytestream from the Byte Reader to determine when start-note and stop-note commands are sent, and which notes to play.
3. Frequency Converter. Given a bit-value of a note, this module uses a lookup-table and a clock to sample voltages across a sine wave. This produces an oscillating voltage of the desired frequency.
4. D-to-a Converter. This (confusingly named) module interfaces with an actual hardware d-to-a converter. The module simply sends bits one at a time to that module.




## Parallel Ray Tracer (Spring 2022)
### Repository is here: https://github.com/BoxianWang/cs77-final-project
This is a parallel ray tracer for CS78 (Computer Graphics). By moving a naive C++ implementation into CUDA, using alternative data types, tree-based collision detection and unrolled supersampling, we were able to get an approximately 2000x improvement in ray tracing speed. For this project, I wrote around 3,000 lines of CUDA (though most of this was just converted C++).




## Simulated 32-bit CPU (Spring 2022)
### Please ask for access to this repository.
This is a simulated 32-bit CPU in Logisim. It uses the Y86 instruction set. The CPU does the following:
1. Fetches instructions from memory
2. Loads information into registers
3. Performs any necessary ALU operations
4. Reads and writes information into memory
In order to do this, the CPU has a separate datapath and controller. The controller is programmed with state-control information from an Excel file. The datapath is programmed by loading a program (in hex) into the ROM at the right of the circuit.
Custom test files (in both assembly and hex format) are included in the repository.




