Some popular tools and libraries  
| |Console|GUI (native)|GUI (themed)|2D Game|3D Game|3D Rendering|Audio|Image Processing|CPU and GPU Computation|  
|-|-|-|-|-|-|-|-|-|-|  
|C++|Curses, Linenoise, Crossline|wxWidgets<sup>a</sup>, FLTK,<br>Nana<sup>b</sup>|Qt\*,<br>GTK\* (and optionally gtkmm\*)|SDL, SFML, Allegro|Godot, Panda3D|Irrlicht, Ogre,<br>FreeGLUT<sup>c</sup>/GLFW+GLEW (OpenGL<sup>d</sup>), Vulkan<sup>e</sup>|OpenAL Soft\*, irrKlang\*\*\*|Magick++, stb|OpenCL<sup>d</sup>|  
|Python|Curses, Readline\*\*|tkinter, wxPython<sup>a</sup>|PyGTK\*, PyQt\*\*|Pygame|Godot, Panda3D, Ursina|PyOpenGL (Legacy OpenGL<sup>f</sup>),<br>GLFW+PyGLEW (Modern OpenGL<sup>d</sup>), PyVulkan<sup>e</sup>|PyAudio, Mingus|wand|PyOpenCL<sup>d</sup>|  
<sup>
*: License is open source, but does not allow static linking.<br>
**: License is open source, but does not allow distributing executable under a different license.<br>
***: License is not open source.<br>
a: wxWidgets does not use native API on Linux. It uses either GTK, Qt or Motif. A port for Xorg is being developed, though. Also, wxWidgets has poor Wayland support.<br>
b: Nana supports only Windows and X11. It does not support Wayland and MacOS.<br>
c: FreeGLUT does not support native Cocoa on MacOS and uses XQuartz.<br>
d: MacOS has deprecated OpenGL and removed OpenCL.<br>
e: Vulkan is not supported on MacOS.<br>
f: Legacy OpenGL is deprecated, uses deprecated concepts, and very few vendors support it.
</sup>
