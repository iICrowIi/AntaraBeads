# AntaraBeads
A c# program to solve the Bead Puzzle locks in the game Betrayal in Antara

USAGE:
BeadSolver.exe inputfilename

Input:
Each letter represents a bead of some color. Beads are case sensitive, and no white space is allowed.
START: indicates the beads in the hopper as the puzzle starts.
GOAL: specifies the final state of the hopper that solves the puzzle.
Each line with a pipe in it represents a rule.  The player can input the left side to receive the right, or vice versa.

Output:
All "unique" solutions that take the smallest number of steps to achieve will be output to the console.  As the solver moves forward, it drops any sequence of moves that produces a game state identical to one already observed by the solver - except for the final step, of course.
Each step in the solution will be written with the number of the rule as it was presented in the input file, and A or B to indicate whether to place the beads on the left side of the rule into the drawer to obtain the right side, or vice versa.

Example input file and solution:
START:RWB
GOAL:RWWWB
RW|GYY
B|YOO
WB|OYG
RY|OG
RB|WOOG
YY|WGB
OR|WG
RG|WW

Solution 1: 3A 4B 6A 8A


Enjoy,
Crow!
