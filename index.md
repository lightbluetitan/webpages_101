---
title: "Sintaxis Básica Markdown"
author: "Renzo Cáceres Rossi"
date: "2022/10/06"
output:
  html_document:
    code_download: yes
  word_document: default
  pdf_document: default
subtitle: "Markdown - RMarkdown"
---

<!-- Añadir comentarios a nuestro documento Markdown - HTML tags -->


## Overview

**Markdown** es un lenguaje de marcado ligero (**Lighweight Markup Language**), siendo **RMarkdown**[^1] uno de sus dialectos, una de sus variantes, uno de sus sabores (**Markdown Flavours**.)




## Encabezados - Títulos

# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Título 1
=========

Título 2
---------

## Separaciones - Líneas Horizontales

---

***

---

***

## Citas - Añadir citas a nuestro documento Markdown


> “La tecnología no es nada. Lo importante es que tengas fe en la gente, que sean básicamente buenas e inteligentes, y si les das herramientas, harán cosas maravillosas con ellas”
>
> -- <cite>[Steve Jobs][^2]</cite>


[^1]: **RMarkdown** es un paquete del lenguaje de programación R, que nos permite crear documentos científicos y técnicos para convertirlos a formatos tales como HTML,PDF,Word entre otros.

[^2]: https://www.animsa.es/noticias/10-frases-sobre-tecnologia-para-reflexionar/



## Negrita - Cursiva - Tachado - Subrayado 

**Texto formateado como Negrita**

*Texto formateado como Cursiva*

***Texto formateado como Negrita y Cursiva***

~~Texto tachado~~

<u>Texto subrayado</u> <!-- HTML tags -->


## Superíndice - Subíndice

**Superíndice**^999^


**Subíndice**~999~


## Listas

### Lista Viñetas - Lista Anidada

- Lista 1
- Lista 2
- Lista 3
- Lista 4
- Lista 5
  - Lista 5.1
  - Lista 5.2
  - Lista 5.3
- Lista 6
- Lista 7
- Lista 8


### Lista Numerada

1. Lista 1
2. Lista 2
3. Lista 3
4. Lista 4
5. Lista 5
6. Lista 6
7. Lista 7

### Lista ordenada alfabéticamente

a. Lista A
b. Lista B
c. Lista C
d. Lista D
e. Lista E
f. Lista F

### Casos - Ejemplos


- Lista 1
- Lista 2
- Lista 3
* Lista 4
* Lista 5
* Lista 6
+ Lista 7
+ Lista 8
+ Lista 9

---

- [ ] Lista A
- [ ] Lista B
- [ ] Lista C
- [ ] Lista D
- [ ] Lista E
- [ ] Lista F
- [ ] Lista G

---

1. Lista A
3. Lista B
5. Lista C
7. Lista D
9. Lista E
11. Lista F


## Tablas - Añadir tablas a nuestro documento Markdown

|TABLA A|TABLA B|TABLA C|
|:-----:|:-----:|:-----:|
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |
|A      |B      |C      |


## Enlaces - Añadir links a nuestro documento Markdown


<https://latin-r.com/>{target=_blank}


[Latin R](https://latin-r.com/){target=_blank}

[Latin R 2022](https://latin-r.com/ "Ingresar a Latin R 2022"){target=_blank}


## Imágenes - Añadir imágenes a nuestro documento Markdown

<center>

![**Logo R**](logo_r.png)



![**RMarkdown**](https://d33wubrfki0l68.cloudfront.net/aee91187a9c6811a802ddc524c3271302893a149/a7003/images/bandthree2.png){width=400}



</center>


## Vídeos - Añadir vídeos a nuestro documento Markdown

<!-- HTML tags -->

<center>

<iframe width="560" height="315" src="https://www.youtube.com/embed/EkxRj02iaLk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen data-external=1></iframe>

</center>


## Mapas - Añadir mapas a nuestro documento Markdown

<!-- HTML tags -->

<center>

<iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3901.980822578654!2d-77.03197518561798!3d-12.044840345143056!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x9105c8b5d35662c7%3A0x15f0bda5ccbd31eb!2sPalacio%20de%20Gobierno%20del%20Per%C3%BA!5e0!3m2!1ses!2spe!4v1665071333171!5m2!1ses!2spe" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade" data-external=1></iframe>


</center>


## Código - Añadir código de distintos lenguajes de programación


    summary(mtcars)
    
La función `barplot()` nos permite crear diagramas de barras (**Bar Charts**) en el lenguaje de programación R.

```R

x <- table(mtcars$cyl)

colores <- c("orange","blue","purple")

barplot(x,xlab="Cilindros",ylab="Frecuencias",main="Número de Cilindros",col=colores)


```

```Python

import matplotlib.pyplot as plt
 

eje_x = ['Python', 'R', 'Node.js', 'PHP']
 

eje_y = [50,20,35,47]
 

plt.bar(eje_x, eje_y)
 

plt.ylabel('Cantidad de usuarios')
 

plt.xlabel('Lenguajes de programación')
 

plt.title('Usuarios de lenguajes de programación')
 

plt.show()


```

    SELECT id_usuario,usuario_nombre,usuario_apellido FROM usuarios,


```sql
USE Northwind;

SELECT * FROM Products;

```

## Anular sintaxis Markdown


\**Texto que debería ser formateado como Negrita**


\*Texto que debería ser formateado como Cursiva*


\~~Texto que debería ser formateado como tachado~~


