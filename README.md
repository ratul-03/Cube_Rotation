# ASCII Rotating Cubes Animation

This C program creates an animated ASCII art of three rotating cubes using mathematical transformations. It continuously renders and updates the rotation of the cubes in a terminal window.

## Features
- Displays three rotating cubes in ASCII art
- Uses trigonometric functions to simulate 3D rotation
- Implements z-buffering for proper depth management
- Supports cross-platform execution (Windows and Unix-based systems)

## Prerequisites
- A C compiler (GCC, Clang, or MSVC)
- A terminal that supports ANSI escape sequences

## How It Works
1. **Mathematical Transformations**:
   - Uses rotation matrices to transform 3D cube coordinates into 2D screen coordinates.
   - Adjusts the z-depth for proper perspective rendering.
2. **ASCII Rendering**:
   - Uses different ASCII characters (`@`, `$`, `~`, `#`, `;`, `+`) to represent cube faces.
   - Updates the terminal screen in real-time for animation.
3. **Performance Optimization**:
   - Uses a z-buffer to determine which surfaces are visible.
   - Optimized sleep function for smooth rendering.

## Compilation and Execution

### On Linux/macOS:
```sh
gcc cube_animation.c -o cube_animation -lm
./cube_animation
```

### On Windows:
```sh
gcc cube_animation.c -o cube_animation.exe -lm
cube_animation.exe
```

## Controls
- The cubes rotate continuously with time.
- Modify `incrementSpeed`, `distanceFromCam`, and other parameters in the code to adjust speed and perspective.

## Notes
- The animation requires a sufficiently large terminal window to display properly.
- The frame rate can be adjusted by changing `usleep(8000 * 2);` in the loop.

## License
This project is released under the MIT License.

## Author
Md. Arifin Hasan Ratul
