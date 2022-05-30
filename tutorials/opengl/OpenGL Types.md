# OpenGL Types  
| OpenGL Type | C++ Type | Size(bytes) |  
|-------------|----------|-------------|  
|GLvoid|void|0|  
|GLboolean|bool<br>unsigned char<br>uint8_t|1|  
|GLchar|char|1|  
|GLbyte|signed char<br>int8_t|1|  
|GLubyte|unsigned char<br>uint8_t|1|  
|GLshort|short<br>int16_t|2|  
|GLushort|unsigned short<br>uint16_t|2|  
|GLint<br>GLsizei<br>Glfixed|int<br>int32_t|4|  
|GLuint<br>GLenum<br>GLbitfiled|unsigned int<br>uint32_t|4|  
|GLint64|\_\_int64 (MSVC <1400)<br>signed long long (Borland C++)<br>int64_t|4|  
|GLuint64|unsigned \_\_int64 (MSVC <1400)<br>unsigned long long (Borland C++)<br>uint64_t|4|  
|GLhalf|unsigned short|2|  
|GLfloat<br>GLclampf|float|4|  
|GLdouble<br>GLclampd|double|8|  
|GLintptr<br>GLsizeiptr|\_\_w64 int (MSVC 32-bit >= 1300)<br>int (MSVC 32-bit <1300)<br>\_\_int64 (MSVC 64-bit)<br>ptrdiff_t|size of a pointer type|  
|GLsync|struct \_\_GLsync*|size of a pointer type|  

### Reference  
GLEW
