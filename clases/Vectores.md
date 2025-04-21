
---

# Vectores en C++ (uso de `v[]`)

## 1. ¿Qué es un vector (array) en C++?

Un **vector** o **array** es una estructura de datos estática que almacena un conjunto de elementos del mismo tipo en posiciones contiguas de memoria. Se accede a cada elemento mediante un índice entero, empezando en 0.

---

## 2. Declaración e inicialización

```cpp
// Declaración de un array de 5 enteros (no inicializado)
int v[5];

// Declaración e inicialización
int w[5] = {1, 2, 3, 4, 5};

// Inicialización parcial (el resto se pone a 0)
int x[5] = {10, 20};

// Inicialización automática del tamaño
int y[] = {7, 8, 9};  // tamaño 3
```

- **Sintaxis**:
    
    ```cpp
    T nombre[tamaño];
    ```
    
    donde `T` es el tipo ( `int`, `double`, `char`, …) y `tamaño` es una constante entera.
    

---

## 3. Acceso y recorrido

- **Acceso directo**: `v[i]` accede al elemento en la posición `i` (0 ≤ i < tamaño).
    
- **Recorrer**:
    
    ```cpp
    for (int i = 0; i < 5; ++i) {
        std::cout << v[i] << " ";
    }
    ```
    

---

## 4. Operaciones comunes

1. **Asignar valor**:
    
    ```cpp
    v[2] = 42;
    ```
    
2. **Leer valor**:
    
    ```cpp
    int x = v[2];
    ```
    
3. **Buscar un elemento**:
    
    ```cpp
    bool encontrado = false;
    int valor_buscado = 7;
    for (int i = 0; i < n; ++i) {
        if (v[i] == valor_buscado) {
            encontrado = true;
            break;
        }
    }
    ```
    
4. **Copiar un array**:
    
    ```cpp
    int u[5];
    for (int i = 0; i < 5; ++i)
        u[i] = v[i];
    ```
    

---

## 5. Ejemplo completo

```cpp
#include <iostream>
using namespace std;
int main() {
    const int N = 8;
    int v[N] = {5, 3, 8, 1, 9, 2, 4, 7};

    // Mostrar el array
    cout << "Vector v: ";
    for (int i = 0; i < N; ++i)
        cout << v[i] << " ";
    cout << "\n";

    // Suma de todos los elementos
    int suma = 0;
    for (int i = 0; i < N; ++i)
        suma += v[i];
    cout << "Suma: " << suma << "\n";

    // Encontrar el máximo
    int maximo = v[0];
    for (int i = 1; i < N; ++i)
        if (v[i] > maximo)
            maximo = v[i];
    cout << "Máximo: " << maximo << "\n";

    return 0;
}
```

---
