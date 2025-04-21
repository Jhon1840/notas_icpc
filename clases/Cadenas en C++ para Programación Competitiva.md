
## Introducción

Las cadenas (strings) son estructuras fundamentales en programación competitiva. En C++, tenemos principalmente dos formas de manejar cadenas:

- La clase `std::string` de la biblioteca estándar

 generalmente es preferible usar `std::string` por su facilidad de uso y funcionalidades incorporadas.

## Declaración y Operaciones Básicas

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    // Declaración e inicialización
    string s1 = "Hola";
    string s2("Mundo");
    string s3(5, 'a');  // "aaaaa"
    
    // Concatenación
    string resultado = s1 + " " + s2;  // "Hola Mundo"
    
    // Acceso a caracteres
    char primerCaracter = s1[0];  // 'H'
    char ultimoCaracter = s1[s1.size() - 1];  // 'a'
    
    // Longitud de la cadena
    int longitud = s1.length();  // 4
    int tamanio = s1.size();     // 4 (equivalente a length)
    
    // Comparación
    if (s1 == "Hola") cout << "Son iguales" << endl;
    if (s1 < s2) cout << "s1 es lexicográficamente menor que s2" << endl;
    
    return 0;
}
```

## Entrada y Salida

```cpp
#include <iostream>
#include <string>
using namespace std;

int main() {
    string s;
    
    // Lectura de una palabra (hasta espacio o salto de línea)
    cin >> s;
    
    // Lectura de una línea completa (incluye espacios)
    string linea;
    getline(cin, linea);
    
    
    // Salida
    cout << s << endl;
    
    return 0;
}
```

