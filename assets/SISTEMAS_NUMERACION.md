# Sistema Decimal

+++
@snap[span-100]
Para representar números, las personas utilizamos el sistema decimal.
<br>
Esto significa que la base que usamos es 10, es decir, cada posición puede indicar sólamente @css[imp123](10 valores distintos).
<br>
@box[text-white bg-orange span-30 fragment](Número menor# 0)
@box[text-white bg-green span-30 fragment](Número Mayor# 9)
@snapend

+++
Las personas usamos este sistema para representar dinero, matrículas, numeraciones, etc.

@fa[hand-spock fragment fa-5x imp123]
@fa[hand-paper fragment fa-5x imp123]

+++
@snap[span-100]
Para indicar que estamos utilizando base 10, agregamos el subíndice "10"
<br>
<br>

`\[
\text{Ejemplo:}
\]`

`\[
\text{Ejemplo:} = 7_{10} 
\]`

`\[
\text{Ejemplo:} = 257_{10} 
\]`

`\[
\text{Ejemplo:} = 1000_{10} 
\]`

@snapend

+++?code=assets/data/decimal.txt&lang = js

@snap[north-east span-100 text-06 text-gray]
Sistema Decimal
@snapend

@snap[south span-100]
@[1](Comenzamos con el número de menor valor)
@[2](En cada salto, incrementamos el valor en 1)
@[3](En cada salto, incrementamos el valor en 1)
@[4](En cada salto, incrementamos el valor en 1)
@[5]
@[6]
@[7]
@[8]
@[9]
@[10](Llegamos al último posible valor en la escala decimal.)
@[11](Agregamos un 1 al principio, y volvemos a comenzar desde 0)
@[12]
@[13]
@[14]
@[15]
@[16]
@[17](Y así continuamos sucesivamente!)
@snapend

---
# Sistema Binario

+++ 
### Binario
Las computadoras, representan la información utilizando el sistema binario. La base que utiliza es 2, es decir, cada posición puede indicar sólamente @css[imp123](2 valores distintos).

@box[text-white bg-orange span-30 fragment](Número menor# 0)
@box[text-white bg-green span-30 fragment](Número Mayor# 1)
@snapend

+++
Las personas utilizan este sistema para representar caracters, contar, sumar, etc.

@fa[hand-pointer fragment fa-5x imp123]
@fa[hand-rock fragment fa-5x imp123]

+++?code=assets/data/binary.txt&lang = js

@snap[north-east span-100 text-06 text-gray]
Sistema Binario
@snapend

@snap[south span-100]
@[1](Comenzamos con el número de menor valor)
@[2](Llegamos al último posible valor en la escala binaria)
@[3](Agregamos un 1 al principio, y volvemos a comenzar desde 0)
@[4](Sumamos 1, llegamos al máximo valor que se puede representar con dos dígitos)
@[5](Agregamos un 1 al principio, y volvemos a comenzar desde 100)
@[6]
@[7]
@[8]
@[9](Agregamos un 1 al principio, y volvemos a comenzar desde 1000)
@[10]
@[11]
@[12]
@[13]
@[14]
@[15]
@[16]
@[17](Y así continuamos sucesivamente!)
@snapend

+++ 
### Conversiones de Binario a Decimal
@snap[span-100 text-08]
1. Dado un número en binario:
`\[
110100_{2} 
\]`
<br>
@snapend

@snap[span-100 fragment text-08 text-left]
2. Comenzamos numerando las posiciones de derecha a izquierda, comenzando en cero.
`\[
110100_{2} =  1\cdot2^5 + 1\cdot2^4 + 0\cdot2^3 + 1\cdot2^2 + 0\cdot2^1  + 0\cdot2^0
\]`
<br>
`\[
110100_{2} =  32_{10} + 16_{10} + 0_{10} + 4_{10} + 0_{10}  + 0_{10}
\]`
<br>
@snapend

@snap[span-100 fragment text-08]
3. Completamos la suma:
`\[
110100_{2} =  52_{10}
\]`
@snapend
+++

### Otro ejemplo...
@snap[span-100 text-06]
Problema 1:
`\[
10101011_{2}
\]`
<br>
`\[
\require{cancel}
10101011_{2} =  1\cdot2^7 + \cancel{0\cdot2^6} + 1\cdot2^5 + \cancel{0\cdot2^4} + 1\cdot2^3 + \cancel{0\cdot2^2} + 1\cdot2^1 + 1\cdot2^0
\]`
<br>
`\[
\require{cancel}
10101011_{2} =  1\cdot2^7 + 1\cdot2^5 + 1\cdot2^3 + 1\cdot2^1+ 1\cdot2^0
\]`
<br>
`\[
10101011_{2} =  128_{10} + 32_{10} + 8_{10} + 2_{10} + 1_{10}
\]`
<br>
`\[
10101011_{2} =  171_{10}
\]`
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_12.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Dividimos el número a convertir entre 2, que es la base deseada)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_11.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Apuntamos el valor del residuo.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_10.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Se baja el valor del resultado de la división. Se repite la operación y apuntamos el residuo.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_9.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Se baja el valor del resultado de la división. Se repite la operación y apuntamos el residuo.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_8.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](El resultado de la división entera 125/2 = 62, con un residuo de 1. Apuntamos el residuo y el resultado de la división entera.)
@snapend


+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_7.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Repetimos la operación hasta que no podamos dividir el número.)
@snapend


+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_6.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Repetimos la operación hasta que no podamos dividir el número.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_5.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Repetimos la operación hasta que no podamos dividir el número.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_4.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Repetimos la operación hasta que no podamos dividir el número.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_3.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](Repetimos la operación hasta que no podamos dividir el número.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_2.png)
@snapend

@snap[east span-50 text-08 text-right]
@css[text-pink](La división entera 1/2 = 0, con un residuo de 1. Apuntamos el 1 y concluimos.)
@snapend

+++?color=white
@transition[none]
@snap[north-east span-40 h4-black] 
#### Conversiones de Decimal a Binario
@snapend
@snap[west span-80]
![](assets/img/dec_conv/step_1.png)
@snapend

@snap[south-east span-50 text-08 text-right]
@css[text-pink](Para finalizar, copiamos los números de abajo hacia arriba.)
@snapend

+++
### Trabajo individual
`\[
100001_{2} \to x_{10}
\]`

`\[
11111111_{2} \to x_{10}
\]`

`\[
254_{10} \to x_{2}
\]`

`\[
17_{10} \to x_{2}
\]`

---
@snap[text-09]
# Sistema Hexadecimal y Octal
@snapend

+++ 
### Hexadecimal y Octal
Para evitar largos conjuntos de caracteres cuando queramos representar números en binario, utilizamos las bases intermedias de @css[imp123](Octal) y @css[imp123](Hexadecimal).

+++
### Octal
@snap[span-100]

Cada dígito en esta representación puede representar hasta 8 valores.

@box[text-white bg-orange span-30 fragment](Número menor# 0)
@box[text-white bg-green span-30 fragment](Número Mayor# 7)
@snapend

+++?code=assets/data/octal.txt&lang = js
@[1](Comenzamos el conteo)
@[2](Sumamos 1)
@[3](Sumamos 1)
@[4](Sumamos 1)
@[5](Sumamos 1)
@[6](Sumamos 1)
@[7](Sumamos 1)
@[8](Alcanzamos el máximo valor por dígito)
@[9](Comenzamos de nuevo desde 10)
@[10-16](Sumamos 1 hasta llegar a 17)
@[17](Comenzamos desde 20)
@[18-21](Y así sucesivamente hasta que llegamos al 77, y de ahí pasamos al 100)

@snap[north-east span-100 text-06 text-gray]
Sistema Octal
@snapend

+++
### Hexadecimal
@snap[span-100]
Cada dígito en esta representación puede representar hasta 15 distintos valores. 
Para esto, se utilizan los números del 0-1, y las letras de la A-F.
@box[text-white bg-orange span-30 fragment](Número menor# 0)
@box[text-white bg-green span-30 fragment](Número Mayor# F)
@snapend

+++?code=assets/data/hexadecimal.txt&lang = js
@[1](Comenzamos el conteo)
@[2](Sumamos 1)
@[3](Sumamos 1)
@[4](Sumamos 1)
@[5](Sumamos 1)
@[6](Sumamos 1)
@[7](Sumamos 1)
@[8](Sumamos 1)
@[9](Sumamos 1)
@[10](Sumanos 1)
@[11](El 10 decimal lo representamos con una "A")
@[12](El 11 decimal lo representamos con una "B")
@[13](El 12 decimal lo representamos con una "C")
@[14](El 13 decimal lo representamos con una "D")
@[15](El 14 decimal lo representamos con una "E")
@[16](Máximo valor representable por una posición, "F")
@[17](Volvemos a comenzar desde el 10)
@[18-33](Y asi sucesivamente!)

@snap[north-east span-100 text-06 text-gray]
Sistema Hexadecimal
@snapend
