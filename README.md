# LearnOpenGL: Hello Triangle

My solution to the [Hello Triangle](https://learnopengl.com/Getting-started/Hello-Triangle) chapter of learnopengl.com, with a color for each vertex.

## Requirements

- CMake 4.1+ and a C++20 compiler
- [GLFW](https://www.glfw.org/) 3.5+

## Build

If GLFW isn't installed in a standard location, tell CMake where it is with `CMAKE_PREFIX_PATH`:

```sh
cmake -S . -B build -DCMAKE_PREFIX_PATH=/path/to/glfw
cmake --build build
./build/learnopengl
```

In an IDE, add the same `-DCMAKE_PREFIX_PATH=...` flag to its CMake options (in CLion: *Settings → Build, Execution, Deployment → CMake*).

Press **Esc** to close the window.
