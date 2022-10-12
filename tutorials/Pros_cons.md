## C++  
Pros:  
1. It is a very flexible programming language. It has a lot many features and syntaxes which can help create various modern and traditional control flows.  
2. It is very fast and compiled to native code. This is something which lets build kernel components, applications relying on real time data, games etc.  
3. It has a wide community. There are dozens of good libraries, even open source ones, out there for each particular job. There are many good compilers (e.g. GCC, Clang, MSVC etc.), standard libraries (e.g. libstdc++, libc++, MSVC STL, etc.), linters and formatters (e.g. VSCode's Linter, various other code editor extensions), documentation tools(e.g. Doxygen, Sphinx etc.), build tools (e.g. CMake, MSBuild etc.), package managers (e.g. MSYS2 pacman, Linux default package managers etc.) and other tools out there.  

Cons:  
1. It can be found as overly complex by a few, since it has a lot many syntaxes.
2. It is difficult to write error free code. Nevertheless, this thing enhances debugging skills by a huge extent. But debugging gets easier on practice.  

## Rust  
Pros:  
1. It is very fast and compiled to native code. This is something which lets build kernel components, applications relying on real time data, games etc.  
2. It is very safe and protected language because it uses smart pointers in the default safe mode and defines some lints to warn or throw error. In unsafe cases an `unsafe` keyword must be turned on, and to grant some permissions to the entire file, a few lints must be turned off.  
3. It has standardised tooling, namely rustc as compiler, rust-std as standard library, cargo as build tool and package manager, clippy and rustfmt as linter and formatter and rust-docs as documentation tool.  
4. It has a good foreign function interface.  

Cons:  
1. It sometimes shows unncessary warnings, like nonstandard style or unused code, which have no reason to raise a problem. They need to be turned off in every main file.  
2. Safe mode is less flexible, which may be obvious enough. Also, working with smart pointers can sometimes be difficult to adjust to.  
3. It lacks some basic concepts like function overloading, which has to be done indirectly through traits, and object oriented features like inheritence.  
