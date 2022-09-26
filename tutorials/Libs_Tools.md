Some popular tools and libraries  
| |Console|GUI(native)|&emsp;GUI&nbsp;(themed)&emsp;|2D Game|3D Game|3D Rendering|Audio|Image Processing|CPU and GPU Computation|Threading|  
|-|-|-|-|-|-|-|-|-|-|-|  
|C++|Curses, Linenoise-ng, Crossline|tk, wxWidgets<sup>a</sup>|FLTK, Nana<sup>b</sup>, Qt\*<sup>c</sup>,<br>GTK\* (and optionally gtkmm\*, its official C++ binding)|SDL, SFML, Allegro|Godot<sup>d</sup>, Panda3D, Unreal\*\*\*|Irrlicht, Ogre,<br>FreeGLUT<sup>e</sup>/GLFW+GLEW (OpenGL<sup>f</sup>), Vulkan<sup>g</sup>|OpenAL Soft\*, OpenAL\*\*\*<sup>h</sup>, irrKlang\*\*\*|Magick++, stb|OpenCL<sup>f</sup>, OpenGL Compute Shaders<sup>fi</sup>|Standard Library (`std::thread`, `std::mutex`, `std::atomic`), Boost.Thread, Native (Win32 and POSIX Threads), OpenMP<sup>j</sup>|  
|Python|Curses, Readline\*\*|tkinter, wxPython<sup>a</sup>|PyGTK\*, PyQt\*\*<sup>c</sup>, PySide\*<sup>c</sup>|Pygame, Pyglet, PySDL2|Godot<sup>d</sup>, Panda3D, Ursina|PyOpenGL (Legacy OpenGL<sup>k</sup>),<br>GLFW+PyGLEW (Modern OpenGL<sup>f</sup>), PyVulkan<sup>g</sup>|PyAudio, Mingus|wand|PyOpenCL<sup>f</sup>||  
|Rust|Console|Azul|fltk-rs, gtk-rs, iced|||||||Standard Library|  
|Java||AWT|Swing|LWJGL||||||`Thread` class|  
<sup>
*: License is open source, but does not allow static linking. (suitable for most cases, but if both static and shared libraries exist it may add up complexity in linking)<br>
**: License is open source, but does not allow distributing executable under a different license. (suitable only for open source projects which will be released under the same license)<br>
***: License is not open source. (suitable for open source projects and basic proprietary projects)<br>
a: wxWidgets does not use native API on Linux. It uses either GTK, Qt or Motif. A port for Xorg is being developed, though, but is not actively developed. GTK looks native on GNOME, Xfce, MATE and Cinnamon though, and Qt on LXQt, KDE and Deepin.<br>
b: Nana supports only Windows and Xorg. It does not support Wayland and MacOS.<br>
c: Qt has both open source and proprietary licenses. As open source it is dual licensed under LGPLv3 and GPLv3. As closed source a license can be bought allowing static linking. PyQt is also licensed the same way, except that there is no option for LGPLv3. PySide is an alternative Python binding licensed under LGPLv2.1.<br>
d: Godot officially supports C#, C++ and GDScript. Unofficial bindings supported by community are Rust, Nim, JavaScript, Haskell, Go, Python, Clojure, Haskell, Swift and D.<br>
e: FreeGLUT does not support native Cocoa on MacOS and uses XQuartz.<br>
f: MacOS has deprecated OpenGL (and last version it supports in 4.1) and removed OpenCL.<br>
g: Vulkan is not supported on MacOS.<br>
h: Older versions of OpenAL are open sourced under LGPL, and even older versions are under BSD.<br>
i: Compute Shaders are only supported in OpenGL 4.3+.<br>
j: OpenMP relies on compiler support. GCC, Clang and MSVC support it, though.<br>
k: Legacy OpenGL is deprecated, uses deprecated concepts, and very few vendors support it.
</sup>
