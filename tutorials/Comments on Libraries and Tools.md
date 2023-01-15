# 1. SFML  
Current Version: 2.5  
License: zlib, Freetype (FreeType), public domain (libjpeg and stb_image), LGPL (OpenAL Soft), BSD (libogg, libvorbis and libflac)  
SFML is a C++ library for creating hardware accelerated 2d graphics, OpenGL and multimedia based applications. For 2D graphics it uses OpenGL. In all, it is a library which makes excellent use of every good C++ feature. Another thing is that the graphics and terminal can run as two separate processes (at least on Linux). Also, it has a really amazing documentation, and dozens of tutorials are made on it, including its official one. But there is one flaw I noticed, though it is possibly under development for the 2.6 version of it, and that flaw is unicode support. I tried to print some chess piece emojis and CJK glyphs, but falied even with unicode based fonts. But later I realised that it lacks unicode support. I hope this is added in the close future, since unicode support is important for cross language applications or applications that require emojis or utilities like text editors with unicode support.  

# 2. SDL
Current Version: 2.0 
License: zlib, LGPL (<= 1.2)  
SDL is a C library (and is also used with C++) for creating 2d graphics, OpenGL and graphics based multimedia applications. In all it is a very reliable library and supports unicode. For 2D graphics, it either implements its own software based renderer or uses OpenGL. It supports both software and hardware based rendering. It has a font and image loading library, capable of even loading unicode, though both of them need to be installed separately. One flaw of it is that the quality of documentation did not seem to be that good. It is reliable, but very technical, and examples are given for no single function. It has dozens of tutorials, though. Another flaw is lack of graphics primitives. This is a good challenge for a curious programmer, like me, though. Also, it is also a good library for developing high level graphics frameworks like game engines. Also, the core SDL does only provide a basic interface for graphics, and other libraries must be used to extend it. The SDL_ttf library, which is a separate package, but a part of the library, is an extension to it based of FreeType, allowing excellent support for TrueType and OpenType fonts. The SDL_image is another such extension which allows loading images of various formats. SDL_rtf allows loading Rich Text Format files into the program, while SDL_mixer allows to use audio in it. SDL_net is a small networking library.  

# 3. WxWidgets  
Current Version: 3.1 - 3.2 (latest is 3.2.1)  
License: WxWindows Library License  
WxWidgets and a C++ library for creating GUI using widgets. Its biggest advantage is that it has several backends, and recommends the most native looking and most developed (by them) backend as the default on each system (Win32 API on Windows, Cocoa on MacOS, GTK (although native only to certain DEs) on Linux), a rare way (only a few like Tk use this way), which is unlike a few (e.g. QT, GTK, FLTK etc.) which draw all the widgets on a canvas. For developing applications which look truly native across all platforms, this is possibly one of the best choices. It also supports unicode using a conditional macro called `wxT` and a data type called `wxString`. One thing I did not like about this library is its highly object oriented nature. Even though it can be good at some cases for organising code, in all it is a bit too lengthy and complex. It makes writing the simplest programs difficult. I really wish that syntax would have been similar to QT or SDL or SFML. But in all it is an excellent choice.  

# 4. FLTK
Current Version: 1.3.(0-8), 1.4 (development)  
License: FLTK License  
FLTK is a C++ library for creating GUI using widgets. These widgets are hardcoded using native APIs (previously OpenGL). At least for me, the widgets look a bit too ugly and old fashioned, and its feature set is very limited.  

# 5. Dear ImGui  
Current Version: 1.89  
License: MIT  
Dear ImGui, or ImGui in short is a library for creating immediate mode GUI inside a window. It is used in C++ for the same purpose as tweakpane and dat.gui are used with threejs in JavaScript/HTML. It has several backends (namely Allegro 5, GLFW, GLUT, Mac OS, SDL and Win32, and there maybe third party backends) and supports various renderers (namely DirectX 9, DirectX 10, DirectX 11, DirectX 12, Metal, OpenGL 2, OpenGL 3, SDL Renderer and Vulkan, don't know about others). According to my experience, it is good looking and somewhat easy  and straightforward to manage, at least for simple controls. But I found the it is very slow and laggy.
