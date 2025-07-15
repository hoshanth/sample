# ComputerGraphic_Project

Railway Station Simulation
A simple OpenGL project simulating a railway station environment with interactive elements like day/night cycles, a moving train, traffic lights, and animated objects like a plane and comet.

Features
Day and Night Cycle: Toggle between day and night scenes.

Railway Station Scene: Renders a detailed railway station with a platform, track, and station building.

Train Animation: A train that moves along the track, controllable for arrival.

Traffic Signal: An interactive traffic light that changes between red and green.

Dynamic Objects:

An aeroplane that can appear and fly across the sky.

A comet that can appear and traverse the night sky.

User Interaction: Control various aspects of the simulation using keyboard inputs and a right-click menu.

Technologies Used
C Programming Language

OpenGL (GLUT Library) for graphics rendering.

Installation
To compile and run this project, you'll need a C compiler (like GCC) and the OpenGL GLUT library installed on your system.

Prerequisites
GCC (GNU Compiler Collection)

FreeGLUT or MesaLib (for OpenGL development)

On Ubuntu/Debian:
Bash

sudo apt update
sudo apt install build-essential freeglut3-dev
On Fedora:
Bash

sudo dnf install gcc freeglut-devel
On macOS:
You might need to install Xcode Command Line Tools:

Bash

xcode-select --install
Then, you may need to install FreeGLUT via Homebrew:

Bash

/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
brew install freeglut
Compiling the Code
Save the code: Save the provided C code as railway_station.c (or any .c filename).

Open a terminal in the directory where you saved the file.

Compile the code using GCC and link with the OpenGL and GLUT libraries:

Bash

gcc railway_station.c -o railway_station -lGL -lGLU -lglut -lm
-o railway_station: Specifies the output executable name.

-lGL: Links the OpenGL library.

-lGLU: Links the OpenGL Utility Library.

-lglut: Links the OpenGL Utility Toolkit library.

-lm: Links the math library (for sqrt or similar functions, if used, though not explicitly in this code, it's good practice for graphics).

Usage
Run the executable:

Bash

./railway_station
Interact with the simulation: Follow the instructions printed in your terminal:

Press 'r' or 'R' to change the signal light to red.

Press 'g' or 'G' to change the signal light to green.

Press 'd' or 'D' to switch to day mode (sun and blue sky).

Press 'n' or 'N' to switch to night mode (moon and stars).

Press 't' or 'T' to make the train arrive at the station (resets its position and starts animation).

Right-click anywhere on the window to display a menu:

"Aeroplane": Makes an aeroplane appear and fly.

"Comet": Makes a comet appear and fly across the night sky.

Left-click anywhere on the window to quit the program.

Contributing
This is a personal project, but if you have suggestions for improvements or bug fixes, feel free to open an issue or submit a pull request!
