# Rust Tutorial  
## What is Rust?  
Rust is an object based (inheritence is not possible but can be made possible to some extent with hacks), functional and procedural programming language. Some of its common aspects are:  
1. Good level of flexibility and features: Rust is very flexible, and can work at low level as well as high level, which is why using it in operating system kernels is started. Rust supports anonymous functions, multithreading, regular expressions, containers, tuples, partial support for duck typing (`any`, `option`), automatic type deduction, networking and so on. Rust is directly compiled to native binary code, and so it adds to security of the application (binary executables are more difficult to reverse engineer), and also performance. It can also be used with static and dynamic libraries but it is overly complicated.  
2. Interoperability with C: Rust can relatively easily interact with C than other high level programming languages, except for C++ though, which is amost a superset of C.  
3. Growing community:Rust does not have a large community, but the community is growing. Wrappers to C APIs and libraries like OpenGL, OpenAL soft are constantly being made.  
## Requirements for this Tutorial:
1. Rust 1.62.0 Complete: Installation instructions are available clear enough on many websites, including Rust's official websites.  
2. Text Editor  
## Hello World  
First let us see the program.
```rust
#![allow(non_camel_case_types)]
#![allow(unused_mut)]
#![allow(dead_code)]
#![allow(unused_variables)]

fn main() {
    println!("Hello World");
}
```  
1. The first 4 lines do nothing except telling the compiler not to display some unnecessary warnings.  
2. Unlike C++, You do not need to include standard library files separately. Rust includes it automatically.  
3. In Rust, `fn main()` is the main function which can return any type, but usually nothing is returned.  
4. `println!()` is the macro used for displaying output in the console. There is another macro called `print!()` which does not add a newline at the end. The equivalent code to `println!()` will be `use std::io; use std::io::write;` at the top and then `print!("\n"); io::stdout().flush().unwrap();` in `main()`.  
## Run the Program  
Let your name of the program be `filename.rs`. Then use the following command to compile it.  
```cmd
rustc filename.rs
```  
Then there will result an executable file named `filename.exe` on Windows, and maybe `filename.out` on Linux. On Windows, if using MinGW based install, or if using Linux, then it will give that one executable file. But if on Windows using MSVC based install(if you don't customise the install, this is the default), it also results in a `filename.pdb` file. THen run the executable like it will usually be run in a terminal.  
