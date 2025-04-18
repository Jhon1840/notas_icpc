# ABS()
abs()

La función `abs()` en C++ devuelve el **valor absoluto** de un número. En este caso, se usa para asegurarse de que la diferencia entre `a` y `b` siempre sea positiva, sin importar cuál sea mayor.

cout << abs(a - b) << endl;



# Lexitografia

la lexitografia es el la letra a nivel assci
"aloh" < "hola"
ya que 'a' tiene un codigo ascii inferior a 'h'
esto es muy importante ya que al ordenarlo asi
```
cad2="hola";
do{
	 cout<<cad2;
} while (next_permutation(cad2.begin(), cad2.end()));
```
si cad2="hola" solo va a genera permutaciones lexitograficamente superiores a "hola" omitiendo alguna menores como "ahlo" , la fomra correcta es o escribir la lexitografia menor u ordenarla de antemano
```
string cad2 = "hola"; sort(cad2.begin(), cad2.end());
```
(tienes que usar `"#include <algorithm>"` para poder usar next_permutation)


# LONG_MAX

es una funcion de la libreria `#include <climits>` se usa para declara una variable en el valor maximo que puede tomar.
```
long a=LONG_MA;
```
aquir a tenda el valor maximo que puede tener una variable long



# Triangulos Degenerados

Un **triángulo no degenerado** es un triángulo que cumple con la desigualdad triangular, es decir, sus tres lados forman una figura con área positiva. Matemáticamente, para que un triángulo con lados a,b,ca, b, ca,b,c sea **no degenerado**, debe cumplirse:

						a+b>c    b+c>b     b+c>a

Si alguna de estas desigualdades no se cumple, el "triángulo" en realidad colapsa en una línea recta y se dice que es un **triángulo degenerado** con área cero.

![[Pasted image 20250224154846.png]]



por ejemplo un triangulo de a=2 , b=4, c=6 seria degenerado ya que formaria una linea recta. con un area de 0  


# Reordenamiento (4 digitos)


```
	if(a1>a2) swap(a1, a2);
    if(a3>a4) swap(a3, a4);
    if(a1>a3) swap(a1, a3);
    if(a2>a4) swap(a2, a4);
    if(a2>a3) swap(a2, a3);
```




