# Data Structure Visualizer

An interactive C++ desktop application that makes data structures visible through SFML graphics. Users can enter values, explore how structures are organized, and search for elements through a graphical interface.

## Features

- **Stacks and queues:** visualize push/pop and enqueue/dequeue operations.
- **Binary search trees and AVL trees:** inspect node placement and balanced-tree structure.
- **Tries:** insert and search words.
- **Graphs:** add nodes and edges.
- Shared controls for searching, resetting, and navigating visualizations, with scrolling for larger structures.

## Technology

C++, SFML 2.6.2, and a Code::Blocks project configured for MinGW on Windows. The source uses `windows.h` and a `WinMain` entry point.

## Build and run

1. Clone the repository:
   ```bash
   git clone https://github.com/stevenrashid/Data-Structure-Visualizer.git
   cd Data-Structure-Visualizer
   ```
2. Install Code::Blocks/MinGW and an SFML 2.6.2 build that matches the compiler and architecture.
3. Open `Data Structure Visualizer.cbp`.
4. Replace the machine-specific SFML include and library directories in the project settings with your local paths. Check the selected target's SFML linker settings; Debug uses debug libraries, while Release is configured for static linking.
5. For a dynamically linked build, make the matching SFML DLLs available to the executable.
6. Build and launch with the repository root as the working directory so the program can load `arial.ttf`, `logo.png`, `background.png`, and `WORDART2.png`.

## Using the visualizer

Select a structure from the menu, enter values in the input box, and use the available operation buttons. For graphs, enter node values separated by spaces; enter a start and end node value to add an edge.

## Files

| File | Purpose |
| --- | --- |
| [main.cpp](main.cpp) | Application, UI controls, and data-structure implementations. |
| [Data Structure Visualizer.cbp](Data%20Structure%20Visualizer.cbp) | Code::Blocks build configuration. |
| [README.txt](README.txt) | Detailed class and method documentation. |
| [Source code 37.txt](Source%20code%2037.txt) | Additional source snapshot. |

## Scope

This is an educational desktop project. The checked-in build configuration is Windows-specific; other platforms require source and build adjustments. The AVL view's estimated BST timing is an illustrative comparison, not a controlled benchmark.
