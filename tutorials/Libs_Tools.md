Some popular tools and libraries  
| |Console|GUI (native)|GUI (themed)|2D Game|3D Game|3D Rendering|Audio|Image Processing|CPU and GPU Computation|Threading|  
|-|-|-|-|-|-|-|-|-|-|-|  
|C++|Curses, Linenoise, Crossline|wxWidgets<sup>a</sup>|FLTK, Nana<sup>b</sup>, Qt\*,<br>GTK\* (and optionally gtkmm\*)|SDL, SFML, Allegro|Godot<sup>c</sup>, Panda3D, Unreal***|Irrlicht, Ogre,<br>FreeGLUT<sup>d</sup>/GLFW+GLEW (OpenGL<sup>e</sup>), Vulkan<sup>f</sup>|OpenAL Soft\*, OpenAL\*\*\*<sup>g</sup>, irrKlang\*\*\*|Magick++, stb|OpenCL<sup>e</sup>, OpenGL Compute Shaders<sup>eh</sup>|Standard Library (`std::thread`, `std::mutex`, `std::atomic`), Boost.Thread, Native (Win32 and POSIX Threads), OpenMP<sup>i</sup>|  
|Python|Curses, Readline\*\*|tkinter, wxPython<sup>a</sup>|PyGTK\*, PyQt\*\*|Pygame, Pyglet, PySDL2|Godot<sup>c</sup>, Panda3D, Ursina|PyOpenGL (Legacy OpenGL<sup>j</sup>),<br>GLFW+PyGLEW (Modern OpenGL<sup>e</sup>), PyVulkan<sup>f</sup>|PyAudio, Mingus|wand|PyOpenCL<sup>e</sup>||  
|Rust|Console|Azul|fltk-rs, gtk-rs, iced|||||||Standard Library|  
|Java||AWT|Swing|LWJGL||||||`Thread` class|  
<sup>
*: License is open source, but does not allow static linking. (suitable for most cases, but if both static and shared libraries exist it may add up complexity in linking)<br>
**: License is open source, but does not allow distributing executable under a different license. (suitable only for open source projects which will be released under the same license)<br>
***: License is not open source. (suitable for open source projects and basic proprietary projects)<br>
a: wxWidgets does not use native API on Linux. It uses either GTK, Qt or Motif. A port for Xorg is being developed, though, but is not actively developed. GTK looks native on GNOME, Xfce, MATE and Cinnamon though, and Qt on LXQt, KDE and Deepin.<br>
b: Nana supports only Windows and Xorg. It does not support Wayland and MacOS.<br>
c: Godot officially supports C#, C++ and GDScript. Unofficial bindings supported by community are Rust, Nim, JavaScript, Haskell, Go, Python, Clojure, Haskell, Swift and D.<br>
d: FreeGLUT does not support native Cocoa on MacOS and uses XQuartz.<br>
e: MacOS has deprecated OpenGL (and last version it supports in 4.1) and removed OpenCL.<br>
f: Vulkan is not supported on MacOS.<br>
g: Older versions of OpenAL are open sourced under LGPL, and even older versions are under BSD.<br>
h: Compute Shaders are only supported in OpenGL 4.3+.<br>
i: OpenMP relies on compiler support. GCC, Clang and MSVC support it, though.<br>
j: Legacy OpenGL is deprecated, uses deprecated concepts, and very few vendors support it.
</sup>
