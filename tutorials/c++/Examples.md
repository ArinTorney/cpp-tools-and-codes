## Object Based Programming in C  
### 1: Using Plain C  
```c
// Vec3.h

typedef struct Vec3_struct *Vec3; // opaque pointer is used for encapsulation (named differently to be compatible with C++)
Vec3 Vec3_new(double x, double y, double z);
void Vec3_delete(Vec3 _inst); // _inst is used as a convention, using any other name e.g. self is also fine
                              // just don't use this, so that it can be successfully compiled on a C++ compiler
Vec3 Vec3_fromVec3(Vec3 _inst);
double Vec3_get(Vec3 _inst, char param);
void Vec3_set(Vec3 _inst, char param, double value);

// Vec3.c

#include "Car.h"

#include <stdlib.h>
#include <stdio.h>

struct Vec3_struct {
    double vec[3];
};

Vec3 Vec3_new(double x, double y, double z) {
    Vec3 _inst = (Vec3)malloc(sizeof(Vec3_struct));
    _inst->vec[0] = x;
    _inst->vec[1] = y;
    _inst->vec[2] = z;
    return _inst;
}

void Vec3_delete(Vec3 _inst) {
    free(_inst);
}

Vec3 Vec3_fromVec3(Vec3 _inst) {
    return Vec3_new(_inst->vec[0], _inst->vec[1], _inst->vec[2]);
}

double Vec3_get(Vec3 _inst, char param) {
    if (param == 'x') { // mind the single quotes, they are used for single character
        return _inst->vec[0];
    }
    else if (param == 'y') {
        return _inst->vec[1];
    }
    else if (param == 'z') {
        return _inst->vec[2];
    }
    else {
        printf("ERROR: \'%c\' is not a valid option for double Vec3_get(Vec3{aka struct Vec3_struct *}, char)", param);
        exit(0);
        return 0;
    }
}

void Vec3_set(Vec3 _inst, char param, double value) {
    if (param == 'x') { // mind the single quotes, they are used for single character
        _inst->vec[0] = value;
    }
    else if (param == 'y') {
        _inst->vec[1] = value;
    }
    else if (param == 'z') {
        _inst->vec[2] = value;
    }
    else {
        printf("ERROR: \'%c\' is not a valid option for void Vec3_set(Vec3{aka struct Vec3_struct *}, char, double)", param);
        exit(0);
        return 0;
    }
}

// main.c

#include "Vec3.h"

void main() { // use int main() while testing on a C++ compiler
    Vec3 vector3 = Vec3_new(10.5, 20.1, 10.0);
    Vec3 another_vector3 = Vec3_fromVec3(vector3);
    Vec3_delete(vector3);
    
    double X = Vec3_get(another_vector3, 'x');
    Vec3_set(another_vector3, 'y', x * 2);
    Vec3_delete(another_vector3);
}
```
### 2: Using Cello
