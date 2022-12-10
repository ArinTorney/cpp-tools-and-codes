## XCB Basic Example  
```c
// C/C++ example to create a basic X11 window with white background using XCB
// XCB is an alternative to XLib for creating X11 applications. A port of it is available for Windows.
#define X11_NO_WINDOW_DECORATIONS 0 // set this to 1 to disable default window decorations done by DEs

#include <string.h>
#include <stdlib.h>
#include <iostream>

#include <unistd.h>
#include <xcb/xcb.h>

typedef struct {
    uint32_t flags;
    uint32_t functions;
    uint32_t decorations;
    int32_t input_mode;
    uint32_t status;
} MotifHints;

int main() {
    xcb_connection_t *connection = xcb_connect(NULL, NULL);

    const xcb_setup_t *setup = xcb_get_setup(connection);
    xcb_screen_iterator_t iter = xcb_setup_roots_iterator(setup);
    xcb_screen_t *screen = iter.data;

    xcb_window_t window = xcb_generate_id(connection);
    uint32_t mask[] = {screen->white_pixel, XCB_EVENT_MASK_EXPOSURE | XCB_EVENT_MASK_BUTTON_PRESS | XCB_EVENT_MASK_BUTTON_RELEASE};
    xcb_create_window(connection, XCB_COPY_FROM_PARENT, window, screen->root, 0, 0, 600, 600, 5, XCB_WINDOW_CLASS_INPUT_OUTPUT, screen->root_visual, XCB_CW_BACK_PIXEL | XCB_CW_EVENT_MASK, mask);

    xcb_intern_atom_cookie_t cookie = xcb_intern_atom(connection, 0, strlen("_MOTIF_WM_HINTS"), "_MOTIF_WM_HINTS");
    xcb_intern_atom_reply_t *property = xcb_intern_atom_reply(connection, cookie, NULL);
    MotifHints *hints = (MotifHints*)malloc(20);
    hints->flags = 2;
    hints->decorations =
#ifdef X11_NO_WINDOW_DECORATIONS
#if X11_NO_WINDOW_DECORATIONS == true
        0;
#else
        1;
#endif
#else
        1;
#endif
    xcb_change_property(connection, XCB_PROP_MODE_REPLACE, window, property->atom, property->atom, 32, 5, hints);
    xcb_map_window(connection, window);
    xcb_flush(connection);
    free(property);
    free(hints);

    xcb_gcontext_t gc = xcb_generate_id(connection);
    uint32_t gcmask = XCB_GC_FOREGROUND;
    uint32_t value[] = {screen->white_pixel};
    xcb_create_gc(connection, gc, window, gcmask, value);

    xcb_generic_event_t *event;
    while (event = xcb_wait_for_event(connection)) {
        switch (event->response_type & -0x80) {
            case XCB_EXPOSE: {
                    xcb_expose_event_t *expose = (xcb_expose_event_t *)event;
                }
                break;

            case XCB_BUTTON_PRESS: {
                    xcb_button_press_event_t *press = (xcb_button_press_event_t *)event;
                }
                break;
        }
        free(event);
    }

    xcb_unmap_window(connection, window);
    xcb_flush(connection);
    
    xcb_disconnect(connection);
    return 0;
}
```  
## Object Based Programming in C  
### 1: Using Plain C  
```c
// Vec3.h

#ifndef __VEC3_H_INCLUDED__
#define __VEC3_H_INCLUDED__

#ifdef __cplusplus
extern "C" {
#endif

typedef struct Vec3_struct *Vec3; // opaque pointer is used for encapsulation (named differently to be compatible with C++)
Vec3 Vec3_new(double x, double y, double z);
void Vec3_delete(Vec3 _inst); // _inst is used as a convention, using any other name e.g. self is also fine
                              // just don't use this, so that it can be successfully compiled on a C++ compiler
Vec3 Vec3_fromVec3(Vec3 _inst);
double Vec3_get(Vec3 _inst, char param);
void Vec3_set(Vec3 _inst, char param, double value);

#ifdef __cplusplus
}
#endif

#endif

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
