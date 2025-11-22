Towers of Hanoi – OpenGL 3D Simulation

This project is a 3D graphical simulation of the classic Towers of Hanoi puzzle, built using C and OpenGL (GLUT). The program visually demonstrates the recursive algorithm used to solve the puzzle, presenting smooth animations of disk movements between the three rods.

🔹 Features

3D visualization using OpenGL + GLUT

Adjustable number of disks (1–9)

Animated movements demonstrating the recursive Hanoi algorithm

Realistic disk stacking, pin drawing, and movement trajectory

Keyboard controls:

1–9 → Select number of disks

+ / - → Zoom in / out

Arrow keys → Rotate view

PageUp/PageDown → Move camera

s/x → Increase / decrease speed

r → Restart animation

f → Fullscreen toggle

Space → Reset view

q / ESC → Exit

Shows total moves and timer

Includes an introduction splash screen

🔹 Technologies Used

Programming Language: C

Graphics Library: OpenGL (GLU, GLUT)

Rendering: 3D cylinders, disks, transformations, lighting, shading

Algorithm: Recursive Tower of Hanoi solution

🔹 How It Works

The program:

Generates all moves using a recursive function

Stores the moves in a queue

Animates each move using a timer function

Draws pins, disks, and movement paths in real-time
