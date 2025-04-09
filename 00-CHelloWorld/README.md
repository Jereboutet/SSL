# Prueba de Compilador C23

Este proyecto tiene como objetivo verificar el soporte del compilador seleccionado para el estándar **C23** de C.

---

### A. Compilador seleccionado

###### **GCC (GNU Compiler Collection)**

---

### B. Versión del compilador

```bash
$ gcc --version
gcc.exe (Rev3, Built by MSYS2 project) 13.2.0
```

### C. Versión de C que el compilador compila
El compilador soporta el estándar **C23**, invocado mediante la opción `-std=c2x`.

Se verificó el soporte compilando correctamente el siguiente código que utiliza `auto`, una característica exclusiva de C23:

```c
#include <stdio.h>

int main(void) {
    auto x = 42;
    auto y = 3.14;

    printf("x: %d\n", x);
    printf("y: %.2f\n", y);

    return 0;
}


