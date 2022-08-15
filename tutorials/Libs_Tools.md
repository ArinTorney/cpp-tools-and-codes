Some popular tools and libraries  
| |Console|GUI (native)|GUI (themed)|2D Game|3D Game|3D Rendering|Audio|  
|-|-|-|-|-|-|-|-|  
|C++|Curses, Linenoise, Crossline|wxWidgets, FLTK,<br>Nana<sup>a</sup>|Qt\*,<br>GTK\* (and optionally gtkmm\*)|SDL, SFML, Allegro|Godot, Panda3D|Irrlicht, Ogre,<br>FreeGLUT<sup>b</sup>/GLFW+GLEW (OpenGL<sup>c</sup>), Vulkan<sup>d</sup>|OpenAL Soft\*, irrKlang\*\*\*|  
|Python|Curses, Readline\*\*|tkinter, wxPython|PyGTK\*, PyQt\*\*|Pygame|Godot, Panda3D, Ursina|PyOpenGL (Legacy OpenGL),<br>GLFW+PyGLEW (Modern OpenGL<sup>c</sup>), PyVulkan<sup>d</sup>|PyAudio, Mingus|  

<sub>
*: License is open source, but does not allow static linking.<br>
**: License is open source, but does not allow distributing executable under a different license.<br>
***: License is not open source.<br>
a: Nana supports only Windows and X11. It does not support Wayland and MacOS<br>
b: FreeGLUT does not support native Cocoa on MacOS and uses XQuartz.<br>
c: MacOS has deprecated OpenGL and removed OpenCL.  
d: Vulkan is not supported on MacOS.
</sub>
