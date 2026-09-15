# 📅 Weekly Planner in C

A lightweight, console-based weekly schedule and activity organizer written in standard C. The application demonstrates user-defined data structures, dynamic array allocation with `malloc()`, and formatted tabular reporting in the terminal.

---

## Overview

Managing daily tasks requires a clean structure to store day names, calendar dates, and activity notes. This project models a weekly schedule using a `struct planner` composite type. Memory for the desired number of days (up to 7) is allocated dynamically at runtime, populated via terminal prompts, displayed in an organized table, and safely freed upon exit.

---

## Features

- **Dynamic Memory Allocation**: Allocates exactly the required memory at runtime using `malloc()` based on user-specified day counts.
- **Custom Data Structure**: Employs `struct planner` containing fields for day name, numeric date, and activity description.
- **Multi-Word Activity Support**: Reads multi-word task descriptions containing spaces seamlessly using formatted `scanf`.
- **Input Validation**: Restricts input to valid weekly day ranges (1 to 7 days).
- **Tabular Report Display**: Prints a clean, left-aligned tabular overview of all planned days and activities.
- **Memory Safety**: Explicitly releases allocated heap memory using `free()` prior to program termination.

---

## Tech Stack

| Component | Specification |
| --- | --- |
| Language | C (C99 standard or higher) |
| Data Structure | Array of Structures (`struct planner`) |
| Memory Management | Dynamic Heap Allocation (`malloc`, `free`) |
| Interface | Command Line Interface (CLI) |

---

## Project Structure

```
Weekly-planner/
├── planner.c        # Source code (structure definition, memory management, CLI logic)
└── README.md        # Project documentation
```

---

## Getting Started

### Prerequisites

You need a C compiler such as GCC, Clang, or MSVC installed on your system.

To check if GCC is installed:

```bash
gcc --version
```

### Installation

Clone the repository to your local machine:

```bash
git clone https://github.com/Kumar44developer/Weekly-planner.git
```

### Compile & Run

1. Navigate into the project folder:

   ```bash
   cd Weekly-planner
   ```

2. Compile the source code using GCC:

   ```bash
   gcc planner.c -o planner
   ```

3. Run the compiled executable:

   - **On Windows:**

     ```bash
     planner.exe
     ```

   - **On Linux / macOS:**

     ```bash
     ./planner
     ```

---

## Sample Execution

```text
Enter the number of days (max 7): 3
Enter the details of each day:

Day 1
Enter day name: Monday
Enter date (numeric): 15
Enter activity: Team Sprint Planning

Day 2
Enter day name: Tuesday
Enter date (numeric): 16
Enter activity: Code Review and Debugging

Day 3
Enter day name: Wednesday
Enter date (numeric): 17
Enter activity: System Deployment

=== Weekly Planner ===
Day          Date     Activity    
Monday       15       Team Sprint Planning
Tuesday      16       Code Review and Debugging
Wednesday    17       System Deployment
```

---

## Author

**Kumar44developer** — [GitHub Profile](https://github.com/Kumar44developer)
