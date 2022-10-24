# To choose a programming language and tool  
## General purpose GUI applicatiions  
### Windows  
For Windows, C#, Visual Basic and C++/CLI are programming languages built for the purpose. However, since the original API is written for C, even C and C++ can be used. The best option can be the native API for Windows, but MFC can also be used.  
### MacOS  
For MacOS, Objective C and Swift are programming languages built for the purpose. Swift, however, has poor compatibility with C code. And Objective C is less memory safe. C++ can still be used, but it is really complicated.  
### Linux  
Linux has not made a separate programming language for its apps, but most developers prefer C or C++. For GUI applications, the native Wayland libries (for Wayland) and Xlib or XCB (for X11) can be used. But generally they are quite complex. So GTK (native to GNOME, Cinnamon, Xfce etc.) or QT (native to KDE, LXQt etc.) or GNUStep (in Objective C) may be preferred for most applications.  
### Cross platform  
FOr cross platform applications there are many ways to make them. Usually C++ should be good, though. But there are many others too like Rust, Python etc. For a library, WxWidgets is one of the best cross platform ones, which has the speciality of using native widgets from the native toolkit on each platform. For a GUI toolkit which emulates a native look across all platofrms, Qt may be a good choice. Tk can be an alternative to Qt.  
### Text User Interface  
For this C++ or Python are usually used. Ncurses is possibly the best library to go with.  
## Console applications  
These should possibly use C++, because it is extremely fast in terms of performance. Libraries like Crossline, Linenoise-ng may assist.
## Games  
For games, it is good to squeeze up all the performance. So C++ or Rust shall be good. But C++ may be better because it has a ton of libraries for it, and it has a properly designed object oriented paradigm. But somebody worrying about so called clean code may take Rust. For a rendering engine, pure OpenGL is excellent. SDL or SFML or Allegro can be used for 2D game development. For 3D games Irrlicht or Ogre may work well. If a game engine is needed, Godot (C++
, C#, GDScript), Unreal (C++), Unity (C#) or CryEngine (C++) may be good choices.
