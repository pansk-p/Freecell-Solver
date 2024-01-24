# Solitaire Solver

## Overview
The Solitaire Solver is a versatile C program designed to tackle various solitaire card games through the implementation of different search algorithms. By representing the solitaire game as a set of card stacks, the program employs Breadth-First Search, Depth-First Search, Best-First Search, and A* Search to explore potential moves, ultimately aiming to discover a sequence of moves that lead to a victorious state.

### Key Components

#### 1. Search Algorithms
   - **Breadth-First Search:** Explores the game state tree level by level, ensuring that all nodes at a given depth are expanded before moving deeper.
   - **Depth-First Search:** Traverses as far as possible along one branch of the tree before backtracking, providing an alternative exploration strategy.
   - **Best-First Search:** Selects the most promising nodes based on a heuristic evaluation, allowing for more informed exploration.
   - **A* Search:** Combines the principles of both Breadth-First and Best-First searches, incorporating a heuristic to estimate the cost of reaching the goal from the current state.

#### 2. Input Format
   - The solitaire game is initialized by reading card stack configurations from an input file.
   - The input file format is flexible, enabling users to define various solitaire scenarios by specifying the number and type of cards in each stack.

#### 3. Memory Management
   - Efficiently manages memory during the creation and traversal of tree nodes representing game states.
   - Implements loop detection mechanisms to avoid redundant exploration of identical game states.

#### 4. Solution Extraction
   - Upon finding a solution, the program extracts and outputs the sequence of moves necessary to achieve the winning state.
   - Output is formatted based on specific move types, providing clarity on how to manipulate cards between stacks and foundation piles.

### Usage
To utilize the program, users must specify the desired search algorithm and provide an input file as command-line arguments. Supported search algorithms include "breadth," "depth," "best," and "astar." The input file should adhere to the defined format, outlining the initial solitaire game configuration.

**Example Command:**
```bash
./solitaire_solver breadth input.txt solution.txt
