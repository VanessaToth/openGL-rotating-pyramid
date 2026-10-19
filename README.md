
#  3D Rotating Pyramid in OpenGL (GLUT)

A 3D computer graphics application built in C++ using OpenGL and the GLUT utility toolkit. The project renders a color-interpolated 4-sided pyramid rotating smoothly in a 3D perspective projection space.

---
 Key Features

- **3D Perspective Rendering:** Utilizes `gluPerspective` and `glViewport` to maintain scene proportions dynamically during window resizing.
- **Smooth Animation Loop:** Implements a 16ms timer callback (`glutTimerFunc`) achieving ~60 FPS real-time rotation.
- **RGB Vertex Interpolation:** Applies distinct RGB color channels per vertex to create smooth gradient lighting effects across triangle primitives.
- **Depth Testing (Z-Buffering):** Enables `GL_DEPTH_TEST` for correct spatial ordering and hidden surface removal.

---
 Tech Stack & Dependencies

- **Language:** C++
- **Graphics Library:** OpenGL Legacy Pipeline
- **Windowing & Input:** GLUT (OpenGL Utility Toolkit) / FreeGLUT

---

 How to Build & Run
-Firsly download the txt file 
### On MacOS:
```bash
mv 3Dpyramid.txt main.cpp
g++ src/main.cpp -o pyramid -framework OpenGL -framework GLUT
./pyramid
```
### On Linux (Ubuntu/Debian):
```bash
sudo apt-get install freeglut3-dev
g++ src/main.cpp -o pyramid -lGL -lGLU -lglut
./pyramid
