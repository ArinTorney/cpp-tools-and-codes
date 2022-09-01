# Multithreading Examples  
## Introduction  
Modern C++(C++11 and later) has introduced standard header files for handling threads.  
## The Most Basic Example  
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
