# Artificial Intelligence Problem Implementations

## Project Overview

This project contains Python implementations of different problems and concepts in **Artificial Intelligence**.

The implementations demonstrate basic AI concepts such as intelligent agents, search algorithms, constraint satisfaction, human-computer interaction, and path finding.

## Problems Implemented

The following AI problems are implemented in this project:

1. **Vacuum World**
2. **8-Puzzle Problem**
3. **8-Queens Problem**
4. **Route Finding Problem**
5. **Turing Test**
6. **Robot Navigation Problem**

## Technologies Used

* Python
* VS Code / Jupyter Notebook
* GitHub

---

## 1. Vacuum World

### Description

The Vacuum World is a simple example of an **intelligent agent**.

The environment contains two rooms, and each room can be either clean or dirty. The vacuum agent checks the current room and performs an appropriate action.

### Actions

* **Suck** – cleans a dirty room.
* **Move Right** – moves from room A to room B.
* **Move Left** – moves from room B to room A.

### Implementation

The program uses simple condition-based rules to decide the action of the vacuum agent.

### Example

Room A = Dirty
Room B = Dirty

Vacuum at A
    ↓
Suck
    ↓
Move Right
    ↓
Suck
    ↓
Both rooms are Clean

## 2. 8-Puzzle Problem

### Description

The 8-Puzzle is a classic **search problem**.

It consists of a 3 × 3 board containing numbers from 1 to 8 and one empty space. The objective is to move the tiles and reach the required goal state.

### Example Goal State

1 2 3
4 5 6
7 8 _


### Implementation

The problem is implemented using **Breadth First Search (BFS)**.

BFS explores possible states level by level until the goal state is reached.

### Basic Process


Initial State
      ↓
Generate Possible Moves
      ↓
Check New States
      ↓
Goal State?
   ↓       ↓
  No      Yes
  ↓        ↓
Continue  Solution


## 3. 8-Queens Problem

### Description

The 8-Queens problem requires placing **8 queens on an 8 × 8 chessboard** so that no two queens attack each other.

No two queens should be in:

* The same row
* The same column
* The same diagonal

### Implementation

The problem is implemented using the **Backtracking** technique.

The program places queens one row at a time. If a queen cannot be safely placed, the program goes back and tries another position.

### Example

```text
. Q . . . . . .
. . . . Q . . .
. . . . . . Q .
Q . . . . . . .
. . . Q . . . .
. . . . . Q . .
. . Q . . . . .
. . . . . . . Q
```

`Q` represents a queen and `.` represents an empty position.

## 4. Route Finding Problem

### Description

The Route Finding Problem involves finding a route from a **starting location to a destination**.

Each connection between locations has a **cost**. The objective is to find a route with the lowest total cost.

### Example

A ----2---- B
|          |
5          1
|          |
C ----2---- E
           |
           2
           |
           F

For example, a route from **A to F** can be:

A → B → E → F


The total cost is:

2 + 1 + 2 = 5


### Implementation

The problem is implemented using **Uniform Cost Search (UCS)**.

Uniform Cost Search always expands the route with the **lowest total cost** first.

### Basic Process

```text
Start
  ↓
Generate Possible Routes
  ↓
Calculate Route Costs
  ↓
Select Lowest-Cost Route
  ↓
Continue Searching
  ↓
Destination Reached


## 5. Turing Test

### Description

The **Turing Test** is a concept proposed by **Alan Turing** to evaluate whether a machine can demonstrate behavior that is similar to human intelligence.

In this implementation, the user interacts with a computer program by asking questions.

The program generates responses based on the question.

### Implementation

The program:

1. Accepts a question from the user.
2. Checks the question for specific keywords.
3. Generates an appropriate response.
4. Continues the interaction until the user enters `exit`.

### Example

Human: Hello
Computer: Hello! Nice to meet you.

Human: What is your name?
Computer: I am an intelligent computer.

Human: Who created you?
Computer: I was created by humans.

Human: exit
Test ended.


## 6. Robot Navigation Problem

### Description

The Robot Navigation Problem involves finding a path for a robot from a **starting position to a goal position** while avoiding obstacles.

The environment is represented using a grid.

```text
0 = Free space
1 = Obstacle
```

### Implementation

The problem is implemented using **Breadth First Search (BFS)**.

The robot can move:

* Up
* Down
* Left
* Right

The program searches for a valid path from the starting position to the goal.

### Basic Process


Start
  ↓
Check Possible Moves
  ↓
Avoid Obstacles
  ↓
Move to Next Position
  ↓
Continue Searching
  ↓
Goal Reached

## Algorithms / Techniques Used

| Problem          | Technique Used             |
| ---------------- | -------------------------- |
| Vacuum World     | Rule-Based Agent           |
| 8-Puzzle         | Breadth First Search (BFS) |
| 8-Queens         | Backtracking               |
| Route Finding    | Uniform Cost Search (UCS)  |
| Turing Test      | Keyword-Based Interaction  |
| Robot Navigation | Breadth First Search (BFS) |

---

## Project Structure

AI-Problem-Implementations/
│
├── vacuum_world.py
├── eight_puzzle.py
├── eight_queens.py
├── route_finding.py
├── turing_test.py
├── robot_navigation.py
│
└── README.md



## Conclusion

This project provides simple Python implementations of different Artificial Intelligence problems.

The implementations help demonstrate important AI concepts including **intelligent agents, search techniques, backtracking, human-computer interaction, route finding, and robot path finding**.
