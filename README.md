# FIFO_Page_Replacement
First in First Out page replacement algorithm in python 
---

### **LRU Page Replacement Algorithm**

# LRU Page Replacement Algorithm with Visualization

Implementation of the Least Recently Used (LRU) page replacement algorithm in Python.

## Features

- **Simulates LRU Page Replacement**: Handles memory management by replacing the least recently used page when a page fault occurs.
- **User Input**: Prompts for the number of frames and a sequence of page accesses (space-separated).
- **Visualization**: Uses **matplotlib** to plot the page replacement process and display the pages present in memory frames at each step.
- **Page Fault Tracking**: Records and displays the total number of page faults.

## Key Functions

1. **`lru_page_replacement(frames_count, page_sequence)`**:
   - Simulates the LRU page replacement process.
   - Adds new pages, removes the least recently used page if memory is full, and tracks page faults.
   - Returns the total number of page faults and the history of memory frames.

2. **`visualize_lru(frames_count, page_sequence)`**:
   - Visualizes the frame state at each time step using **matplotlib**.
   - Includes a tabular representation of frame states with hit/miss information.

## Workflow

- **Page Hit**: Keeps the accessed page in memory, moving it to the most recently used position.
- **Page Fault**: Replaces the least recently used page if memory is full and loads the new page.

## Running the Program

1. **Dependencies**:
   - `matplotlib`
   - `pandas`

2. **Execution**:
   - Run the Python script.
   - Input the number of memory frames and a space-separated page sequence.
   - The program simulates the LRU algorithm and displays a visualization of memory state changes.

