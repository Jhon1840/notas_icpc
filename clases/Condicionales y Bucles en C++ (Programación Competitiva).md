
## 🔹 Condicionales (`if`, `else if`, `else`)

  

Los condicionales se usan para controlar el flujo del programa según condiciones booleanas.

  

```cpp

int x = 10;

  

if (x > 0) {

    cout << "Positivo\n";

} else if (x < 0) {

    cout << "Negativo\n";

} else {

    cout << "Cero\n";

}

```

  

###  Tips:

- Siempre usa llaves `{}` incluso si es una sola línea; mejora la legibilidad.

- Puedes encadenar múltiples condiciones con `&&` (AND) y `||` (OR).

  

```cpp

if (a > 0 && b > 0) {

    // Ambos positivos

}

```

  

---

  

## Bucles (`for`, `while`, `do while`)

  

### 🔸 `for` clásico

  

Ideal para iteraciones con índices.

  

```cpp

for (int i = 0; i < n; i++) {

    cout << i << " ";

}

```

  

### 🔸 `while`

  

Útil cuando no sabes cuántas veces se repetirá.

  

```cpp

while (x > 0) {

    x /= 2;

}

```

  

### 🔸 `do while`

  

Se ejecuta **al menos una vez**.

  

```cpp

int x = 5;

do {

    cout << x << "\n";

    x--;

} while (x > 0);

```

  

---

  

##  Rango (`for-each`)

###### El `for-each` es una **forma más corta y clara** de recorrer los elementos de un contenedor (como `vector`, `array`, `set`, etc)
  
```cpp

int main() {
    int v[] = {10, 20, 30, 40, 50};

    for (int x : v) {
        cout << x << " ";
    }
    // Salida: 10 20 30 40 50
}

```

  

---

  

##  Casos frecuentes  

  

### 🔸 Iterar arrays o vectores:

  

```cpp

for (int i = 0; i < n; i++) {

        cin >> vector[i];


}

```

  

### 🔸 Loop infinito (con `break` interno):

  

```cpp

while (true) {

    int x;

    cin >> x;

    if (x == 0) break;

    // Procesar x

}

```

  

---

  

## ⚠️ Errores comunes

  

- ❌ Olvidar el `;` después del `for` en macros.

- ❌ Usar `=` en lugar de `==` en condiciones.

- ❌ Desbordes por índices fuera de rango (`i <= n` en lugar de `i < n`).

- ❌ No reiniciar variables dentro de bucles anidados.

  


  

---

  

## 🧵 Buenas prácticas

  

- Declara variables de bucle dentro del propio bucle (`for (int i = 0; ...)`) para limitar su ámbito.

- Evita operaciones costosas dentro de la condición (e.g., llamar a funciones complejas).

- Para bucles anidados, considera romper cuando encuentres la solución para ahorrar iteraciones.

  

---
