# Advanced Dynamic Typing for C++  
C++ is a statically typed language. Recently, it is getting dynamic typing features, like generic programming using templates, `auto` and `decltype(auto)`, and `std::any` and `std::variant` since C++17. But I thought of making a class for all primitive types. This is named `_var` It is inspired from Python's dynamic typing. It will be released afterwards, after a few modifications, and also possibly additions.  
## Syntax  
### Initialise a variable
To initialize a variable, just use  
```
_var x = (integer or decimal or string(std::string or char*) or wide character(std::wstring or wchar_t*) string or boolean);
```  
You can typecast it into any of `int`, `float`, `double`, `char*`, `wchar_t*` or `bool`. For typecasting use typecasting operators.  
### `print` and `input`  
---TO-BE-WRITTEN---
## Uses  
You can use it to make dynamically typed arrays(with pointers, `std::vector`, `std::list`, `std::deque`, `std::array` etc.), maps(with `std::map`, `std::unordered_map`, `std::multimap` etc.) and tuples(with `std::tuple` etc.), which will be very similar to Python's lists, dictionaries and tuples respectively.
You can use it to make anything advanced which is dynamically typed, such as a programming language.  
# Messages  
6 Marrch 2022: README is formed.  

2 April 2022: Till now constructor is ready, and typecasts are also ready (C-style typecasts, unlike `std::any`). Also `std::ostream << var` operator overload is ready. But after few more features are added like `var + var`, a few other operator overloads etc. the source will be released.  

9 June 2022: Till now over the previously ready things, `operator+` is ready, and `print` and `input` functions are ready.  

19 June 2022: Some fixes in `operator+`, and basic arithmetic operator overloads are ready. Wide character string support is deprecated for now but will not be removed so soon, since UTF-16 strings lack their own good library, and Win32 API cannot accept `char16_t*` or some type like that.  
# Testing  
This project is being tested with GCC 11.2(MSYS2 MinGW64), but compatibility with GCC 9(for Focal Fossa Ubuntu) and Clang 9 will be kept at least for now.  
# License  
This project is licensed under Apache License 2.0  
# Plan  
Stage 1. To make a class which can store value of any commonly used primitive or string type.  
Stage 2: To make a class which can store value of any commonly used non-primitive type, like the current `var`, `var*`, or maybe even `std::vector<var>`, `std::unordered_map<var>` etc.  
