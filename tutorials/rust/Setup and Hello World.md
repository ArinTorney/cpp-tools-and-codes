# Rust Tutorial  
## What is Rust?  
Rust is an object based, functional and procedural programming language. Some of its common aspects are:  
1. Good level of flexibility and features: Rust is very flexible, and can work at low level as well as high level, which is why using it in operating system kernels is started. Rust supports anonymous functions, multithreading, regular expressions, containers, tuples, partial support for duck typing (`any`, `option`), automatic type deduction, networking and so on. Rust is directly compiled to native binary code, and so it adds to security of the application (binary executables are more difficult to reverse engineer), and also performance. It can also be used with static and dynamic libraries but it is overly complicated.  
2. Interoperability with C: Rust can relatively easily interact with C than other high level programming languages, except for C++ though, which is almost a superset of C, and Objective C, which is a superset of C.  
3. Growing community: Rust does not have a large community, but the community is growing. Wrappers to C and C++ APIs and libraries like OpenGL, OpenAL soft are constantly being made. Some examples include jeremyletang/rust-sfml (SFML)(C++), Rust-SDL2/rust-sdl2 (SDL)(C), mxpv/stb (stb)(C), godot-rust/godot-rust (Godot)(C++, C# and GDScript), not-fl3/bulletrs (Bullet)(C++ and Python), kens-gelsoft/wxRust (wxWidgets)(C++) etc.  
## Why was Rust Made  
Rust was made as a safer alternative to C and C++. Any possibly unsafe code involving data structures like raw pointers or C function wrappers must be explicitly marked unsafe. Rust allows for some high level programming features through some possibly ugly way.  
## Requirements for this Tutorial:
1. Rust 1.62.0 Complete: Installation instructions are available clear enough on many websites, including Rust's official websites.  
2. Text Editor  
## Hello World  
First let us see the program.
<!--// May be required in some cases
// #![allow(unused_variables)]
// #![allow(unused_braces)]
// #![allow(unused_assignments)]
// #![allow(unused_comparisons)]
// #![allow(unused_parens)]
// #![allow(unused_labels)]
// #![allow(unused_imports)]
// #![allow(while_true)]
// #![allow(large_assignments)]
// #![allow(anonymous_parameters)]-->  

```rust
#![allow(non_camel_case_types)]
#![allow(non_snake_case)]
#![allow(non_upper_case_globals)]
#![allow(unused_mut)]
#![allow(dead_code)]
#![allow(path_statements)]
#![warn(useless_deprecated)]
#![forbid(const_item_mutation)]

fn main() {
    println!("Hello World");
}
```  
1. The first 8 lines do nothing except telling the compiler to or not to display some unnecessary warnings or errors. These may be useful in the future.  
3. Unlike C++, you do not need to include standard library files separately. Rust includes it automatically.  
4. In Rust, `fn main()` is the main function which can return any type, but usually nothing is returned.  
5. `println!()` is the macro used for displaying output in the console. There is another macro called `print!()` which does not add a newline at the end. The equivalent code to `println!()` will be `use std::io; use std::io::write;` at the top and then `print!("\n"); io::stdout().flush().unwrap();` in `main()`.  
## Run the Program  
Let your name of the program be `filename.rs`. Then use the following command to compile it.  
```cmd
rustc filename.rs
```  
Then there will result an executable file named `filename.exe` on Windows, and maybe `filename.out` on Linux. On Windows, if using MinGW based install, or if using Linux, then it will give that one executable file. But if on Windows using MSVC based install(if you don't customise the install, this is the default), it also results in a `filename.pdb` file. Then run the executable like it will usually be run in a terminal.  
