# OpenGL Types  
| OpenGL Type | C++ Type | Java Type | Size(bytes) |  
|-------------|----------|-----------|-------------|  
|GLvoid|void|void<br>(void* is Buffer)|0|  
|GLboolean|bool<br>unsigned char<br>uint8_t|boolean|1|  
|GLchar|char|(GLchar*/const GLchar* is String)|1|  
|GLbyte|signed char<br>int8_t|1|  
|GLubyte|unsigned char<br>uint8_t|1|  
|GLshort|short<br>int16_t|2|  
|GLushort|unsigned short<br>uint16_t|2|  
|GLint<br>GLsizei<br>Glfixed|int<br>int32_t|int<br>(GLint* is IntBuffer)|4|  
|GLuint<br>GLenum<br>GLbitfiled|unsigned int<br>uint32_t|4|  
|GLint64|\_\_int64<sub>MSVC <1400</sub><br>signed long long<sub>Borland C++</sub><br>int64_t|4|  
|GLuint64|unsigned \_\_int64<sub>MSVC <1400</sub><br>unsigned long long<sub>Borland C++</sub><br>uint64_t|4|  
|GLhalf|unsigned short|2|  
|GLfloat<br>GLclampf|float|float<br>(GLfloat* is FloatBuffer)|4|  
|GLdouble<br>GLclampd|double|8|  
|GLintptr<br>GLsizeiptr|\_\_w64 int<sub>MSVC 32-bit >= 1300</sub><br>int<sub>MSVC 32-bit <1300</sub><br>\_\_int64<sub>MSVC 64-bit</sub><br>ptrdiff_t|size of a pointer type|  
|GLsync|struct \_\_GLsync*|size of a pointer type|  

### Reference  
GLEW
