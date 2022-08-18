Some popular tools and libraries  
| |Console|GUI (native)|GUI (themed)|2D Game|3D Game|3D Rendering|Audio|Image Processing|CPU and GPU Computation|Threading|  
|-|-|-|-|-|-|-|-|-|-|-|  
|C++|Curses, Linenoise, Crossline|wxWidgets<sup>a</sup>, FLTK,<br>Nana<sup>b</sup>|Qt\*,<br>GTK\* (and optionally gtkmm\*)|SDL, SFML, Allegro|Godot, Panda3D|Irrlicht, Ogre,<br>FreeGLUT<sup>c</sup>/GLFW+GLEW (OpenGL<sup>d</sup>), Vulkan<sup>e</sup>|OpenAL Soft\*, irrKlang\*\*\*|Magick++, stb|OpenCL<sup>d</sup>, OpenGL Compute Shaders<sup>df</sup>|Standard Library (`std::thread`, `std::mutex`, `std::atomic`), Boost.Thread, Native (Win32 and POSIX Threads), OpenMP<sup>g</sup>|  
|Python|Curses, Readline\*\*|tkinter, wxPython<sup>a</sup>|PyGTK\*, PyQt\*\*|Pygame, Pyglet, PySDL2|Godot, Panda3D, Ursina|PyOpenGL (Legacy OpenGL<sup>h</sup>),<br>GLFW+PyGLEW (Modern OpenGL<sup>d</sup>), PyVulkan<sup>e</sup>|PyAudio, Mingus|wand|PyOpenCL<sup>d</sup>||  
|Rust||||||||||Standard Library|  
|Java||AWT|Swing|LWJGL||||||`Thread` class|  
<sup>
*: License is open source, but does not allow static linking.<br>
**: License is open source, but does not allow distributing executable under a different license.<br>
***: License is not open source.<br>
a: wxWidgets does not use native API on Linux. It uses either GTK, Qt or Motif. A port for Xorg is being developed, though, but is not actively developed. Also, wxWidgets has poor Wayland support.<br>
b: Nana supports only Windows and X11. It does not support Wayland and MacOS.<br>
c: FreeGLUT does not support native Cocoa on MacOS and uses XQuartz.<br>
d: MacOS has deprecated OpenGL (and last version it supports in 4.1) and removed OpenCL.<br>
e: Vulkan is not supported on MacOS.<br>
f: Compute Shaders are only supported in OpenGL 4.3+.<br>
g: OpenMP relies on compiler support. GCC, Clang and MSVC support it, though.<br>
h: Legacy OpenGL is deprecated, uses deprecated concepts, and very few vendors support it.
</sup>
