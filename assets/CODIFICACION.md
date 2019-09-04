# Codificación de Información

+++
### Codificación

@snap[text-08 span-100]
La codificación de caracteres es el método que permite convertir un carácter de un alfabeto en un símbolo de otro sistema de representación, aplicando normas o reglas de codificación. @css[imp123](Para representar información en las computadoras, utilizamos las siguientes codificaciones):
@snapend

@snap[text-08 span-100]
@ul[fragment]
* ASCII
* UTF-8
* Unicode
@ulend
@snapend

@snap[south-east]
@fa[code fa-2x]
@snapend

+++
### Codificación
Podemos expresar la cantidad de caracteres representables "M" en función de la cantidad de bits "n" con la siguiente relación.
`\[ M(n) = 2^n   \]`

Por lo que con un byte, se puede representar:

`\[ M(8) = 2^8 = 256 \]`

+++
### Codificación
@snap[fragment span-100 text-07]
Podemos despejar la ecuación para obtener la cantidad de bits mínimos para representar un alfabeto, por ejemplo:
`\[ n \ge log_{2}(M) \]`
`\[ n \ge 3.32 log(M) \]`
<br>
@snapend 

@snap[fragment span-100 text-07]
Por ejemplo, para codificar el siguiente alfabeto:
`\[ \lbrace0,1,2,3,4,5,6,7,8,9\rbrace \]`
<br>
@snapend 

@snap[fragment span-100 text-07]
Necesaríamos:
`\[ n \ge 3.32 log(10) \]`
`\[ n \ge 3.32 \]`
<br>
@snapend

@snap[fragment span-100 text-07]
Redondeado sería
`\[ n \ge 4 \]`
@snapend

+++
### ASCII encoding 
@snap[span-35 text-07]
ASCII es una codificación que requiere @css[imp123](1 byte por caraceter). La codificación ASCII incluye:
@ul[]
* 128 caracetes de ASCII estándar 
* 128 caracters de ASCII extendido
@ulend
@snapend
@snap[south-east span-70]
![ASCII](assets/img/ascii_table.gif)
@snapend

+++
### Unicode
Es mantenido por **The Unicode Consortium**.
Hasta su versión 12.1, contiene un total de @css[imp123](137,929) caracteres.

Incluye:
- Caracteres A @css[text-black](U+0041)
- Íconos ☃ @css[text-black](U+2602)
- Modificadores 👶👶🏻👶🏼👶🏽 @css[text-black](U+1F476) @css[text-black](+) @css[text-black](U+1F3FB)
- Kanji ぁ @css[text-black](U + 3041)
- Emojis @emoji[smile] @css[text-black](U + 1F60A)

+++
### Unicode
@snap[span-100]
![Unicode](assets/img/unicode.png)
@snapend