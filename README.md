COMP 371 CD Programming Project Assignment 1
Siguang Zhao (27827709)
Mengge He (40229748)
Wei Yuan (40074494)
OpenGL Basketball Scene Rendering Project (assignment1)
This is a modern OpenGL 3D rendering project that simulates a bouncing textured 
basketball with dynamic lighting, shadow effects, and interactive camera control.
Project Structure
assignment1/
├── A1.cpp # Main C++ source file
├── basketball.jpg # Texture image for the basketball
├── floor.jpg # Texture image for the floor
├── README # Project documentation file
├── stb/
 └── stb_image.h # Header for image loading using stb_image
Features
- Realistic basketball physics with bounce and gravity
- Two dynamic point lights with Phong lighting
- Simulated shadow using flattened dark sphere projection
- Textured objects (basketball and floor)
- First-person camera with mouse look and WASD controls
- Left-click to trigger bouncing effect
COMP 371 CD Programming Project Assignment 1
Controls
Input Action
'W / A / S / D' Move forward / left / back / right
'Shift' Sprint (move faster)
'Space' Move down (descend)
'F' Move up (ascend)
Mouse Move Look around (camera view)
Scroll Wheel Zoom (adjust FOV)
Left Mouse Trigger ball bounce
'ESC' Exit the program
Requirements
- C++17 or higher
- OpenGL 3.3+
- [GLFW](https://www.glfw.org/)
- [GLEW](http://glew.sourceforge.net/)
- [GLM](https://github.com/g-truc/glm)
- [stb_image.h](https://github.com/nothings/stb) (included)
Notes
1. Make sure basketball.jpg and floor.jpg are in the working directory.
2. Shadows are rendered using a separate fragment shader with alpha blending.
Bash
macOS
g++ A1.cpp -o basketball -I/opt/homebrew/include -L/opt/homebrew/lib -lGLEW -
lglfw -framework OpenGL
COMP 371 CD Programming Project Assignment 1
./basketball
linux subsystem
g++ A1.cpp -o basketball -lGLEW -lGL -lglfw
./basketball
Screenshot
COMP 371 CD Programming Project Assignment 1
