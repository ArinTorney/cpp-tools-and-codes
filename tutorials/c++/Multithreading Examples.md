# Multithreading Examples  
## Introduction  
Modern C++(C++11 and later) has introduced standard header files for handling threads.  
## Basic Examples  
This one just loops forever, just it synchronises 3 threads.  
Note: Don't forget to press Ctrl+C after you have seen enough.  
```c++
#include <iostream>
#include <thread>

void f1() {
    while (1) {
        std::cout << 1 << std::flush;
    }
}

void f2() {
    while (1) {
        std::cout << 2 << std::flush;
    }
}

void f3() {
    while (1) {
        std::cout << 3 << std::flush;
    }
}

int main()
{
    std::thread t1(f1);
    std::thread t2(f2);
    std::thread t3(f3);
    t1.join();
    t2.join();
    t3.join();
    return 0;
}
```
This one is an improved version, which only goes on for 1 second. There is a for loop in each thread so that the multithreaded nature is clearly visible.  
```c++
#include <iostream>
#include <thread>
#include <chrono>

void f1() {
    for (int i = 1; i <= 10; i++) {
        std::cout << 1 << std::flush;
    }
}

void f2() {
    for (int i = 1; i <= 10; i++) {
        std::cout << 2 << std::flush;
    }
}

void f3() {
    for (int i = 1; i <= 10; i++) {
        std::cout << 3 << std::flush;
    }
}

int main() {
    bool loop = true;
    auto now = std::chrono::system_clock::now();
    while (loop) {
        std::thread t1(f1);
        std::thread t2(f2);
        std::thread t3(f3);
        t1.join();
        t2.join();
        t3.join();
        if (std::chrono::system_clock::now() >= now + std::chrono::seconds(1)) {
            break;
	}
    }
    return 0;
}
```
