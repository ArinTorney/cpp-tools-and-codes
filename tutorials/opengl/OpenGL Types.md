# OpenGL Types  
| OpenGL Type | C++ Type | Java Type | Size(bytes) |  
|-------------|----------|-----------|-------------|  
|GLvoid|void|void<br>(void* is Buffer)|0|  
|GLboolean|bool<br>unsigned char<br>uint8_t|boolean|1|  
|GLchar|char|(GLchar*/const GLchar* is String)|1|  
|GLbyte|signed char<br>int8_t|byte<br>(GLbyte* is ByteBuffer or (byte\[\], int v_offset))|1|  
|GLubyte|unsigned char<br>uint8_t|byte<br>(GLubyte* is ByteBuffer or (byte\[\], int v_offset))|1|  
|GLshort|short<br>int16_t|short<br>(GLshort* is ShortBuffer or (short\[\], int v_offset))|2|  
|GLushort|unsigned short<br>uint16_t|short<br>(GLushort* is ShortBuffer or (short\[\], int v_offset))|2|  
|GLint<br>GLsizei<br>Glfixed|int<br>long<br>int32_t|int<br>(GLint* is IntBuffer or (int\[\], int v_offset))|4|  
|GLuint<br>GLenum<br>GLbitfiled|unsigned int<br>unsigned long<br>uint32_t|int<br>(GLuint* is IntBuffer or (int\[\], int v_offset))|4|  
|GLint64|\_\_int64<sub>MSVC < 1400</sub><br>signed long long<sub>Borland C++</sub><br>int64_t|long<br>(GLint64* is LongBuffer or (long\[\], int v_offset))|8|  
|GLuint64|unsigned \_\_int64<sub>MSVC < 1400</sub><br>unsigned long long<sub>Borland C++</sub><br>uint64_t|long<br>(GLuint64* is LongBuffer or (long\[\], int v_offset))|8|  
|GLhalf<sub>NVIDIA-specific</sub>|unsigned short||2|  
|GLfloat<br>GLclampf|float|float<br>(GLfloat* is FloatBuffer or (float, int v_offset))|4|  
|GLdouble<br>GLclampd|double|double<br>(GLdouble* is DoubleBuffer or (double, int v_offset))|8|  
|GLintptr<br>GLsizeiptr|\_\_w64 int<sub>MSVC 32-bit >= 1300</sub><br>int<sub>MSVC 32-bit < 1300</sub><br>\_\_int64<sub>MSVC 64-bit</sub><br>ptrdiff_t|long|size of a pointer type|  
|GLsync|struct \_\_GLsync*|long|size of a pointer type|  

### Reference  
1. GLEW  
2. JOGL Docs  
