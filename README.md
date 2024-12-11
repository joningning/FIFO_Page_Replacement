# FIFO Page Replacement Algorithm

## Overview
This project implements the **FIFO (First-In-First-Out)** page replacement algorithm in Python. The algorithm simulates how pages are managed in memory when the number of available frames is limited. It calculates and visualizes page hits, page faults, and the state of frames at each step.

## Features
- Simulates the FIFO page replacement process.
- Tracks page hits and page faults.
- Displays results in tabular format with a visual representation using Matplotlib.

## Requirements
The following Python libraries are required to run the script:
- `pandas`
- `matplotlib`

You can install them using:
```bash
pip install pandas matplotlib
```

## Usage
1. Run the script.
2. Provide the number of frames (memory slots).
3. Enter the page reference string (space-separated).

### Example Input
```
Enter the number of frames: 3
Enter the page reference string (space-separated): 7 0 1 2 0 3 0 4
```

### Example Output
```
Page sequence: [7, 0, 1, 2, 0, 3, 0, 4]
Page hits: 2
Page faults: 6
Hit ratio: 0.25
Fault ratio: 0.75
```
A table will also be displayed showing the state of frames and whether each step resulted in a hit or a fault.

## How It Works
- Pages are added to frames in the order they are referenced.
- When a page fault occurs:
  - If there is an empty frame, the page is added.
  - If all frames are full, the oldest page (the one that entered first) is replaced.
- The simulation outputs the page replacement process step-by-step, including hits and faults.

## Key Methods
- `access_page(page)`: Handles a single page reference.
- `simulate(page_sequence)`: Simulates the algorithm for the given page sequence.
- `print_results()`: Prints the hit/fault statistics.
- `display_table()`: Displays the page replacement process as a table using Matplotlib.

## Visualization
The `display_table` function shows a visual representation of:
- Frame state after each page reference.
- Hits marked in white.
- Faults highlighted in red.
