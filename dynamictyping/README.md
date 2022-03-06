# Advanced Dynamic Typing for C++  
C++ is a statically typed language. Recently, it is getting dynamic typing features, like generic programming using templates, `auto` and `decltype(auto)`, and `std::any` and `std::variant` since C++17. But they have their own limitations. So as a solution I made a class called `var`, which is very powerful. It is inspired from Python's dynamic typing. It will be released afterwards, after a few modifications, and also possibly additions.  
## Syntax  
To initialize a variable, just use  
```
var x = (integer or decimal or string or wide character string or boolean);
```  
You can typecast it into any of `int`, `double`, `char*`, `wchar_t*` or `bool`. For typecasting use operators. 
## Uses  
You can use it to make dynamically typed arrays(with pointers, `std::vector`, std::list`, std::deque`, `std::array` etc.), maps(with `std::map`, `std::unordered_map`, `std::hash_map` etc.) and tuples(with `std::tuple` etc.), which will be very similar to Python's lists, dictionaries and tuples respectively.
You can use it to make anything advanced which is dynamically typed, such as a programming language.
