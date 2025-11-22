🧩 Towers of Hanoi – 3D OpenGL Simulation

A fully animated 3D visualization of the classic Towers of Hanoi puzzle, implemented using C with OpenGL (GLU/GLUT).
This project demonstrates how recursion, data structures, and computer graphics can be combined to create an interactive educational simulation.

🚀 Features
🎮 Interactive 3D Simulation

Real-time animation of all disk movements

Smooth lifting, rotation, and placement of disks

Fully rendered pegs, rods, and disks in 3D

🔢 Custom Disk Selection

Press keys 1–9 to choose the number of disks.

🎥 Camera & View Controls
Control	Action
Arrow Keys	Rotate view
PageUp/PageDown	Move camera up/down
+ / -	Zoom in / out
Spacebar	Reset view
Mouse Left/Right	Zoom
Mouse Middle	Reset
⚙️ Simulation Controls
Key	Function
s	Increase animation speed
x	Decrease animation speed
r	Restart simulation
f	Toggle fullscreen
q / ESC	Quit
📷 Screens & Introduction Screen

The program includes an intro splash screen showing project title, team members, and guide details.
After pressing Enter, the simulation starts.

🧠 How the Algorithm Works

The project uses the classic recursive algorithm for Towers of Hanoi:

move(n, from, to, temp):
    move(n-1, from, temp, to)
    move 1 disk from 'from' to 'to'
    move(n-1, temp, to, from)


All moves are stored in a linked list queue, then animated with OpenGL timers.

🛠️ Technologies Used

C Programming Language

OpenGL

GLUT (OpenGL Utility Toolkit)

GLU (OpenGL Utility Library)

📦 Project Structure
/TowersOfHanoi
│── main.c               # Full source code (OpenGL + Logic)
│── README.md            # Project documentation
│── Makefile (optional)  # Build automation
└── assets/              # Screenshots (optional)

🔧 How to Compile & Run
Windows (CodeBlocks / Visual Studio / MinGW)

Make sure GLUT is installed and linked.

For MinGW:

gcc main.c -lglu32 -lopengl32 -lfreeglut -o hanoi
./hanoi

Linux

Install required packages:

sudo apt-get install freeglut3-dev build-essential
gcc main.c -lGL -lGLU -lglut -o hanoi
./hanoi

📊 Output Details

Shows current move, total moves, timer, controls

Displays dynamic updates of disk positions

Move count for N disks: 2ⁿ − 1
