# 1. SFML  
Current Version: 2.5  
License: zlib, Freetype (FreeType), public doman (libjpeg and stb_image), LGPL (OpenAL Soft), BSD (libogg, libvorbis and libflac)  
SFML is a C++ library for creating hardware accelerated 2d graphics, OpenGL and multimedia based applications. In all, it is a library which makes excellent use of every good C++ feature. Another thing is that the graphics and terminal can run as two separate processes (at least on Linux). It also has a really amazing documentation, and dozens of tutorials are made on it, including its official one. But there is one flaw I noticed, though it is possibly under development for the 2.6 of it, and that flaw is unicode support. I tried to print some chess piece emojis and CJK glyphs, but falied even with unicode based fonts. But later I realised that it lacks unicode support. I hope this is added in the close future.  

# 2. SDL
Current Version: 2.0  
License: zlib, LGPL (<= 1.2)  
SDL is a C library (and is also used with C++) for creating 2d graphics (both system rendered and hardware accelerated), OpenGL and graphics based multimedia applications. In all it is a very reliable library and supports unicode. It supports both software and hardware based rendering. It has a font and image loading library, capable of even loading unicode, though both of them need to be installed separately. One flaw of it is that the quality of documentation did not seem to be that good. It is reliable, but very technical, and examples are given for no single function. It has dozens of tutorials, though. Another flaw is lack of graphics primitives. This is a good challenge for a curious programmer, like me, though. Also, it is also a good library for developing high level graphics frameworks like game engines. But it should be used with another libraries for audio, networking etc., since this library has only graphics based utilities.  

# 3. WxWidgets  
Current Version: 3.1 - 3.2 (latest is 3.2.1)  
License: LGPL with WxWindows exception (WxWindows Library License)  
WxWidgets and a C++ library for creating GUI using widgets. Its biggest advantage is that it has several backends, and recommends the most native looking and most developed (by them) backend as the default on each system (Win32 API on Windows, Cocoa on MacOS, GTK (although native only to certain DEs) on Linux), a rare way (only a few like Tk use this way), which is unlike a few (e.g. QT, GTK, FLTK etc.) which draw all the widgets on a canvas. For developing applications which look truly native across all platforms, this is possibly one of the best choices. It also supports unicode using a conditional macro called `wxT` and a data type called `wxString`. But, I doubt about its OpenGL support. I know it supports that, but I think it is possibly not installed by default. Also, it is complicated (though possible through its API itself) to get control over the main function of our program.  

# 4. Dear ImGui  
Current Version: 1.89  
License: MIT  
Dear ImGui, or ImGui in short is a library for creating immediate mode GUI inside a window. It is used in C++ for the same purpose as tweakpane and dat.gui are used with threejs in JavaScript/HTML. It has several backends (namely Allegro 5, GLFW, GLUT, Mac OS, SDL and Win32, and there maybe third party backends) and supports various renderers (namely DirectX 9, DirectX 10, DirectX 11, DirectX 12, Metal, OpenGL 2, OpenGL 3, SDL Renderer and Vulkan, don't know about others). According to my experience, it is good looking and somewhat easy to manage, at least for simple controls. But I found the SDL renderer backend is somewhat slow and laggy.
