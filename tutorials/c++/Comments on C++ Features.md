# Comments on C++ Features  
### 1. goto labels  
`goto` is a keyword based on a concept from assembly language retained in C and C++. If used wisely, it can be an excellent feature, but when used messily, it can make the code very confusing.  
RECOMMENDATION: Do not use goto labels, unless the logic of the code is not going to be copied in another programming language, since other programming languages lack the feature.  
### 2. Implicit type conversions  
Implicit type conversions can make the library more magical, but can also hide the logic behind the code.  
RECOMMENDATION: Use implicit type conversions when you know what conversion is happening behind the scenes (no need to know exactly, but just know the result of the conversion).  
