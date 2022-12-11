Some popular tools and libraries  
||Console|GUI<br>Native API|GUI<br>Native|GUI<br>Themed|GUI<br>Game|GUI<br>Immediate Mode|GUI<br>3D Game|GUI<br>3D Rendering|Audio|Image Processing|CPU and GPU Computation|Threading|JSON|  
|-|-|-|-|-|-|-|-|-|-|-|-|-|-|  
|C++|Curses, Linenoise-ng, Crossline, Readline\*\*|Win32 API (Windows),<br> Xlib, XCB(Linux (and other Nix), X11),<br> Wayland API (Linux (and a few BSD), Wayland)<br> Carbon(deprecated), Cocoa(MacOS)|wxWidgets<sup>a</sup>, Tk|FLTK, Nana<sup>b</sup>, Qt\*\^<sup>c</sup>,<br>GTK\* (and optionally gtkmm\*, its official C++ binding)|SDL, SFML, Allegro|Dear ImGUI, Nuklear, FlatUI|Godot<sup>d</sup>, Panda3D, Unreal\*\*\*|OpenFrameworks, Irrlicht, Ogre,<br>FreeGLUT<sup>e</sup>/GLFW+GLEW (OpenGL<sup>f</sup>), Vulkan<sup>g</sup>|SoLoud, Maximilian, PortAudio, OpenAL Soft\*, JUCE\*\*^<sup>h</sup>, OpenAL\*\*\*<sup>i</sup>, irrKlang\*\*\*|Magick++, stb|OpenCL<sup>f</sup>, OpenGL Compute Shaders<sup>fj</sup>|Standard Library (`std::thread`, `std::mutex`, `std::atomic`), Boost.Thread, Native (Win32 and POSIX Threads), OpenMP<sup>k</sup>|nlohmann/json|  
|Python|Curses, Readline\*\*||wxPython<sup>a</sup>, Tkinter|PyGTK\*, PyQt\*\*\^<sup>c</sup>, PySide\*<sup>c</sup>|Pygame, Pyglet, PySDL2||Godot<sup>d</sup>, Panda3D, Ursina|PyOpenGL (Legacy OpenGL<sup>l</sup>),<br>GLFW+PyGLEW (Modern OpenGL<sup>f</sup>), PyVulkan<sup>g</sup>|PyAudio, Mingus|wand|PyOpenCL<sup>f</sup>|*Not possible due to Global Interpreter Lock<br>However, stackless python is a variant which does not have this lock.*|Standard Library `json` module|  
|Rust|Console||Azul|fltk-rs, gtk-rs, iced||||||||Standard Library||  
|Java|||AWT|Swing|LWJGL|||||||`Thread` class||  
<sup>
Category 0- : License is open source, and allows linking anyhow. All permissive and a few weak copylefts come under this category. (suitable everywhere)
Category 1- *: License is open source, but does not allow static linking. All moderately weak copylefts come under this category. (suitable for most cases, but is a bit problematic on Windows, because external shared libraries are not a part of system)<br>
Category 2- **: License is open source, but does not allow distributing executable under a different license. All strong network protective copylefts come under this category. (suitable only for open source projects which will be released under the same license)<br>
Category 3- *^ or **^: License is dual, both open source and proprietary and/or parts of the code are open source but rest is proprietary.<br>
Category 4- ***: License is not open source, and places restrictions on using it. (suitable for open source projects and basic proprietary projects)<br>
a: wxWidgets does not use native API on Linux. It uses either GTK or Motif. A port for Xorg is being developed, though, but is not actively developed. Same is the case with a port for Qt. GTK looks native on GNOME, Xfce, MATE and Cinnamon though, and Qt on LXQt, KDE and Deepin.<br>
b: Nana supports only Windows and Xorg. It does not support Wayland and MacOS.<br>
c: Qt has both open source and proprietary licenses. As open source it is dual licensed under LGPLv3 and GPLv3. As closed source a license can be bought allowing static linking. PyQt is also licensed the same way, except that there is no option for LGPLv3. PySide is an alternative Python binding licensed under LGPLv2.1.<br>
d: Godot officially supports C#, C++ and GDScript. Unofficial bindings supported by community are Rust, Nim, JavaScript, Haskell, Go, Python, Clojure, Haskell, Swift and D.<br>
e: FreeGLUT does not support native Cocoa on MacOS and uses XQuartz.<br>
f: MacOS has deprecated OpenGL (and last version it supports in 4.1) and removed OpenCL. There is a project called ANGLE, though, which is attempting to translate OpenGL ES (a subset of OpenGL) calls to Metal (and other native APIs) (only ES 2.0 supported on MacOS, 3.0 support in progress, according to GitHub). Also, a proprietary project, MoltenGL is being developed to support OpenGL ES 2.0.<br>
g: Vulkan is not supported on MacOS. There is an open source project, called KhronosGroup/MoltenVK, which translates Vulkan calls to Metal for MacOS.<br>
h: juce_audio_basics, juce_audio_devices, juce_core and juce_events are licensed under ISC license. Other modules are covered under GPL or JUCE Personal (revenue upto $50/month), Education (legal educational institutions), Indie (revenue upto $500/month, $40/month or $800) or Pro ($130/month or $2600) EULAs.<br>
i: Older versions of OpenAL are open sourced under LGPL, and even older versions are under BSD.<br>
j: Compute Shaders are only supported in OpenGL 4.3+.<br>
k: OpenMP relies on compiler support. GCC, Clang and MSVC support it, though.<br>
l: Legacy OpenGL is deprecated, uses deprecated concepts, and very few vendors support it.
</sup>
