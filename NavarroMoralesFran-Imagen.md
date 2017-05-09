#### Trabajo realizado por Francisco Javier Navarro Morales
# Análisis Imagen (formatos y códecs)

En primer lugar vamos a visualizar el **material** con el que vamos a llevar a cabo el análisis, se tratan de **5 fotografías en formato .dng** (sin compresión de tipo raw), realizadas con un teléfono móvil y una última **imágen en la que se mezclan gráficas y texto**, realizadas con el programa paint y almacenadas en un formato **.bmp** sin compresión.

![alt text][originales]

Las fotos originales tienen un **tamaño de 23.8 MB** y unas **dimensiones de 504x376 píxeles**. La imagen creada desde paint tiene las mismas dimensiones, pero un **tamaño de 555 KB**.

Para el estudio vamos a utilizar los siguientes formatos:
+ JPG
+ JPG2000
+ PNG
+ BMP
+ GIF
+ TIF

También usaremos distintos valores/algoritmos de compresión disponibles para cada formato.


## Estudio Comparativo

### Primera imagen
|                | Tamaño  | Valoración                                                                                           | Ranking |
|----------------|---------|------------------------------------------------------------------------------------------------------|---------|
| JPG (Q100)     | 198 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG (Q75)      | 45 KB   | Aumentando la tasa de compresión  sigue sin apreciarse diferencias de calidad.                       | 1       |
| JPG (Q50)      | 29 KB   | Empiezan a notarse el efecto pixelado de la imagen.                                                  | 3       |
| JPG (Q10)      | 10 KB   | La imagen se pixela por bloques.                                                                     | 4       |
| JPG2000 (1:1)  | 371 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG2000 (1:25) | 22,1 KB | Se comienza a notar el efecto emborronamiento por algunas zonas.                                     | 4       |
| JPG2000 (1:50) | 11,1 KB | Todavía se acentua más el efecto emborronamiento.                                                    | 5       |
| JPG2000 (1:99) | 5,54 KB | La imagen está totalmente difuminada.                                                                | 6       |
| PNG (SIN)      | 556 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| PNG (C-2)      | 367 KB  | Misma calidad y menor espacio que sin aplicar compresión.                                            | 1       |
| PNG (C-5)      | 372 KB  | Ampliando la compresión no disminuye el tamaño.                                                      | 1       |
| PNG (C-9)      | 369 KB  | Cambiar el parámetro de compresión no tiene efecto como pasa con la anterior.                        | 1       |
| BMP (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| BMP (RLE)      | 555 KB  | De la misma forma aplicándole un algortimo sin pérdida obtenemos una imagen similar a la original.   | 1       |
| GIF            | 111 KB  | Se pierden algunos colores de la foto, como podemos ver en las persianas que aparecen en la derecha. | 3       |
| TIF (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| TIF (LZW)      | 485 KB  | La imagen se ve como la original.                                                                    | 1       |
| TIF (JPG-75)   | 61,9 KB | La imagen se enborrona y se pierden colores, apareciendo como un marco rojo en distintas zonas.      | 4       |

Esta primera imagen recoge una escena entre sol y sombra de un patio de vecinos, en este tipo de fotos de exterior los formatos sin compresión **PNG, BMP y TIF** almacenan la información completa de la imgen manteniendo una calidad como la original al igual que el tamaño que ocupa.

De entre los formatos que aun aplicándole un algoritmo de compresión, no se aprecia disminución de calidad a simple vista (marcados con un 1 en la casilla ranking) cabe destacar que **JPG(Q75)** es el que mayor tasa de compresión consigue, reduciendo el tamaño de la imagen a un 8% de la original sin verse afectada la calidad.

El formato **JPG2000** en cuanto comienza a aplicar compresión emborrona bastante la imagen.

Con **GIF** nos pasa que como tenemos gran variedad de colores perdemos homogeniedad en la imagen, notando el salto entre píxeles en algunas zonas.

### Segunda imagen
|                | Tamaño  | Valoración                                                                                           | Ranking |
|----------------|---------|------------------------------------------------------------------------------------------------------|---------|
| JPG (Q100)     | 150 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG (Q75)      | 28,6 KB | Se nota una pérdida de detalle en la mano.                                                           | 2       |
| JPG (Q50)      | 19,1 KB | Empiezan a notarse el efecto pixelado de la imagen.                                                  | 3       |
| JPG (Q10)      | 7,58 KB | La imagen se pixela por bloques.                                                                     | 4       |
| JPG2000 (1:1)  | 275 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG2000 (1:25) | 22,2 KB | Perdemos casi todas las arrugas de la palma de la mano.                                              | 4       |
| JPG2000 (1:50) | 11,1 KB | La imagen completa empieza a estar muy borrosa.                                                      | 5       |
| JPG2000 (1:99) | 5,59 KB | La imagen está totalmente difuminada.                                                                | 6       |
| PNG (SIN)      | 556 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| PNG (C-2)      | 300 KB  | Misma calidad y menor espacio que sin aplicar compresión.                                            | 1       |
| PNG (C-5)      | 282 KB  | Ampliando la compresión ganamos un poco de espacio sin notarse en la calidad.                        | 1       |
| PNG (C-9)      | 276 KB  | De nuevo ganamos algo de espacio sin verse reflejado en la calidad de la imagen.                     | 1       |
| BMP (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| BMP (RLE)      | 555 KB  | De la misma forma aplicándole un algortimo sin pérdida obtenemos una imagen similar a la original.   | 1       |
| GIF            | 98 KB   | Se pierden algunos colores de la foto, notando el cambio de color entre píxeles cercanos.            | 3       |
| TIF (SIN)      | 556 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| TIF (LZW)      | 471 KB  | La imagen se ve como la original.                                                                    | 1       |
| TIF (JPG-75)   | 42,4 KB | La imagen se enborrona y se pierden colores.                                                         | 4       |

Esta imagen recoge un plano cercano dónde podemos apreciar distintos rasgos de la palma de la mano, los formatos sin compresión **PNG, BMP y TIF** almacenan la información completa de la imgen manteniendo una calidad como la original al igual que el tamaño que ocupa.

De entre los formatos cuya compresión no afecta a la calidad (marcados con un 1 en la casilla ranking) cabe destacar que **JPG(Q100)** es el que mayor tasa de compresión consigue sin perder calidad, reduciendo el tamaño de la imagen a un 27%.

El formato **JPG2000** en cuanto comienza a aplicar compresión dejamos de ver las arrugas de la mano.

De nuevo **GIF** no consigue mapear todos los colores en su paleta de color perdiendo calidad.

### Tercera imagen
|                | Tamaño  | Valoración                                                                                           | Ranking |
|----------------|---------|------------------------------------------------------------------------------------------------------|---------|
| JPG (Q100)     | 134 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG (Q75)      | 23,3 KB | Se nota una pérdida de detalle en el pico y los ojos del pollo.                                      | 2       |
| JPG (Q50)      | 15,4 KB | Empiezan a notarse el efecto pixelado de la imagen.                                                  | 3       |
| JPG (Q10)      | 6,46 KB | La imagen se pixela por bloques.                                                                     | 4       |
| JPG2000 (1:1)  | 253 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG2000 (1:25) | 22 KB   | Empieza a difuminarse la imgen sobre todo por las zonas de sombra.                                   | 4       |
| JPG2000 (1:50) | 11,1 KB | La imagen completa empieza a estar muy borrosa.                                                      | 5       |
| JPG2000 (1:99) | 5,59 KB | La imagen está totalmente difuminada.                                                                | 6       |
| PNG (SIN)      | 556 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| PNG (C-2)      | 284 KB  | Misma calidad y menor espacio que sin aplicar compresión.                                            | 1       |
| PNG (C-5)      | 265 KB  | Ampliando la compresión ganamos un poco de espacio sin notarse en la calidad.                        | 1       |
| PNG (C-9)      | 259 KB  | De nuevo ganamos algo de espacio sin verse reflejado en la calidad de la imagen.                     | 1       |
| BMP (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| BMP (RLE)      | 555 KB  | De la misma forma aplicándole un algortimo sin pérdida obtenemos una imagen similar a la original.   | 1       |
| GIF            | 77,5 KB | Se pierden algunos colores de la foto, notando el cambio de color entre píxeles cercanos.            | 3       |
| TIF (SIN)      | 556 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| TIF (LZW)      | 440 KB  | La imagen se ve como la original.                                                                    | 1       |
| TIF (JPG-75)   | 34 KB   | La imagen se enborrona y se pierden colores.                                                         | 4       |

Esta tercera imagen el objeto a fotografía es un pollo de plástico con mucha rugosidad, de nuevo los formatos sin compresión **PNG, BMP y TIF** almacenan la información completa de la imgen, por lo cual la calidad es como la original.

De entre los formatos que aun aplicándole un algoritmo de compresión, no se aprecia disminución de calidad a simple vista (marcados con un 1 en la casilla ranking) cabe destacar que **JPG(Q100)** es el que mayor tasa de compresión consigue, reduciendo el tamaño de la imagen a un 24% de la original sin verse afectada la calidad.

El formato **JPG2000** en cuanto comienza a aplicar compresión emborrona bastante la imagen.

Con **GIF** lo de siempre en la imagen existen más colores de lo que puede amacenar afectando a la calidad.

### Cuarta imagen
|                | Tamaño  | Valoración                                                                                           | Ranking |
|----------------|---------|------------------------------------------------------------------------------------------------------|---------|
| JPG (Q100)     | 180 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG (Q75)      | 39 KB   | La calidad sigue siendo buena, sin notar cambios.                                                    | 1       |
| JPG (Q50)      | 25,1 KB | Empiezan a notarse el efecto pixelado de la imagen.                                                  | 2       |
| JPG (Q10)      | 9,02 KB | La imagen se pixela por bloques.                                                                     | 4       |
| JPG2000 (1:1)  | 331 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG2000 (1:25) | 22,1 KB | Se pierden las texturas de la tela y las zapas.                                                      | 4       |
| JPG2000 (1:50) | 11 KB   | La imagen completa empieza a estar muy borrosa.                                                      | 5       |
| JPG2000 (1:99) | 5,61 KB | La imagen está totalmente difuminada.                                                                | 6       |
| PNG (SIN)      | 556 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| PNG (C-2)      | 348 KB  | Misma calidad y menor espacio que sin aplicar compresión.                                            | 1       |
| PNG (C-5)      | 340 KB  | Ampliando la compresión ganamos un poco de espacio sin perder calidad.                               | 1       |
| PNG (C-9)      | 336 KB  | De nuevo ganamos algo de espacio sin verse reflejado en la calidad de la imagen.                     | 1       |
| BMP (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| BMP (RLE)      | 555 KB  | De la misma forma aplicándole un algortimo sin pérdida obtenemos una imagen similar a la original.   | 1       |
| GIF            | 102 KB  | No parece notarse la pérdida de calidad.                                                             | 2       |
| TIF (SIN)      | 556 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| TIF (LZW)      | 508 KB  | La imagen se ve como la original.                                                                    | 1       |
| TIF (JPG-75)   | 53,4 KB | La imagen parece desenfocada.                                                                        | 3       |


En esta imagen fotografiamos unas zapatillas y un pantalón para ver como se comportan los formatos con objetos textiles, los formatos sin compresión **PNG, BMP y TIF** como ya sabemos almacenan toda la información.

De entre los formatos que aun aplicándole un algoritmo de compresión, no se aprecia disminución de calidad a simple vista (marcados con un 1 en la casilla ranking) cabe destacar que **JPG(Q75)** es el que mayor tasa de compresión consigue, reduciendo el tamaño de la imagen a un 7% de la original sin verse afectada la calidad.

El formato **JPG2000** en cuanto comienza a aplicar compresión emborrona bastante la imagen.

En este caso **GIF** aunque en un principio me pareció que de nuevo se perdían colores en la tela del pantalón, comparándola con la original se observa que también existen esas zonas blancas provocadas por el brillo de la tela azul, de todas formas no es el formato que mayor compresión consigue.

### Quinta imagen
|                | Tamaño  | Valoración                                                                                           | Ranking |
|----------------|---------|------------------------------------------------------------------------------------------------------|---------|
| JPG (Q100)     | 172 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG (Q75)      | 34,3 KB | Se pierde definición tanto en el muñeco, como la pared y el líquido.                                 | 2       |
| JPG (Q50)      | 22 KB   | Empiezan a notarse el efecto pixelado de la imagen.                                                  | 3       |
| JPG (Q10)      | 7,44 KB | La imagen se pixela por bloques.                                                                     | 4       |
| JPG2000 (1:1)  | 325 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG2000 (1:25) | 22,2 KB | La imagen parece desenfocada.                                                                        | 4       |
| JPG2000 (1:50) | 11,1 KB | La imagen completa empieza a estar muy borrosa.                                                      | 5       |
| JPG2000 (1:99) | 5,61 KB | La imagen está totalmente difuminada.                                                                | 6       |
| PNG (SIN)      | 556 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| PNG (C-2)      | 331 KB  | Misma calidad y menor espacio que sin aplicar compresión.                                            | 1       |
| PNG (C-5)      | 324 KB  | Ampliando la compresión ganamos un poco de espacio sin perder calidad.                               | 1       |
| PNG (C-9)      | 319 KB  | De nuevo ganamos algo de espacio sin verse reflejado en la calidad de la imagen.                     | 1       |
| BMP (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| BMP (RLE)      | 555 KB  | De la misma forma aplicándole un algortimo sin pérdida obtenemos una imagen similar a la original.   | 1       |
| GIF            | 97,2 KB | En las zonas de colores se nota poca uniformidad.                                                    | 3       |
| TIF (SIN)      | 556 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| TIF (LZW)      | 501 KB  | La imagen se ve como la original.                                                                    | 1       |
| TIF (JPG-75)   | 47,4 KB | La imagen se desenfoca y las zonas de blanco se pierden adquiriendo el color de su alrededor.        | 5       |


En una escena un poco más general con distintos objetos en ella podemos concretrar extraer las siguientes conclusiones, los formatos sin compresión **PNG, BMP y TIF** se comportan igual que la original.

De entre los formatos que aun aplicándole un algoritmo de compresión, no se aprecia disminución de calidad a simple vista (marcados con un 1 en la casilla ranking) cabe destacar que **JPG(Q100)** es el que mayor tasa de compresión consigue, reduciendo el tamaño de la imagen a un 31% de la original sin verse afectada la calidad.

El formato **JPG2000** en cuanto comienza a aplicar compresión se produce un efecto de desenfoque.

Con **GIF** en este caso al ser un plano con mayor riqueza de colores, brillos y zonas de sombra le cuesta almacenar estos y se notan los píxeles.

### Sexta imagen
|                | Tamaño  | Valoración                                                                                           | Ranking |
|----------------|---------|------------------------------------------------------------------------------------------------------|---------|
| JPG (Q100)     | 76,7 KB | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG (Q75)      | 29,7 KB | Comienza a aparecer manchas alrededor de las letras y los colores de las barras.                     | 2       |
| JPG (Q50)      | 23,8 KB | Las zonas manchadas aumentan.                                                                        | 3       |
| JPG (Q10)      | 14,7 KB | Todos los bordes de las graficas y letras tienen los colores mezclados.                              | 4       |
| JPG2000 (1:1)  | 77,2 KB | No se aprecia disminución  de la calidad.                                                            | 1       |
| JPG2000 (1:25) | 22,2 KB | Se comienza a notar el efecto emborronamiento por el contorno de letras y barras.                    | 3       |
| JPG2000 (1:50) | 11,1 KB | Todavía se acentua más el efecto emborronamiento.                                                    | 4       |
| JPG2000 (1:99) | 5,60 KB | La imagen está totalmente difuminada.                                                                | 5       |
| PNG (SIN)      | 556 KB  | No se aprecia disminución  de la calidad.                                                            | 1       |
| PNG (C-2)      | 10,2 KB | Misma calidad ganando muchísimo espacio.                                                             | 1       |
| PNG (C-5)      | 6,57 KB | Ampliando la compresión ganamos un poco de espacio sin perder calidad.                               | 1       |
| PNG (C-9)      | 5,79 KB | De nuevo ganamos algo de espacio sin verse reflejado en la calidad de la imagen.                     | 1       |
| BMP (SIN)      | 555 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| BMP (RLE)      | 555 KB  | De la misma forma aplicándole un algortimo sin pérdida obtenemos una imagen similar a la original.   | 1       |
| GIF            | 8,12 KB | Como tenemos pocos colores en la imagen podemos comprimirla sin notar pérdidas.                      | 1       |
| TIF (SIN)      | 556 KB  | Al ser un formato sin compresión, no perdemos nada de información, por lo tanto se ve genial.        | 1       |
| TIF (LZW)      | 38,6 KB | La imagen se ve como la original.                                                                    | 1       |
| TIF (JPG-75)   | 27,8 KB | La imagen se desenfoca y las zonas de blanco se pierden adquiriendo el color de su alrededor.        | 5       |


Esta última foto ha sido creada desde paint para estudiar el efecto en texto y gráficas, los formatos sin compresión **PNG, BMP y TIF** ya sabemos que se comportan como la original.

De entre los formatos que aun aplicándole un algoritmo de compresión, no se aprecia disminución de calidad a simple vista (marcados con un 1 en la casilla ranking) cabe destacar que **PNG(C-9)** es el que mayor tasa de compresión consigue, reduciendo el tamaño de la imagen a un 1% de la original sin verse afectada la calidad.

El formato **JPG2000** en cuanto comienza a aplicar compresión emborrona bastante la imagen.

Con **GIF** en este caso obtenemos una imagen como la original, esto es debido a que en la imagen apenas hay 8 colores que podemos mapear sin problemas.


## Conclusiones
Para concluir el estudio voy a comentar mi opinión personal sobre las imágenes estudiadas aplicado los diferentes formatos/códecs.

En primer lugar comentar que, por alguna razón, al convertir la imagen original a un formato sin compresión, el tamaño varía desde los 23,5 MB hasta los 556 KB, esto pienso que se puede deber a que la imagen original guarda información de metadatos adicional que no son almacenados al convertirse, no obstante los resultados obtenidos son los esperados tal y como vimos en la teoría.

Los formatos sin compresión **PNG, BMP y TIF** en todos los casos optienen una **calidad óptima**, esto es debido a que no utilizan algoritmos de compresión, ó son algoritmos sin pérdidas en los que se puede recuperar la información tal y como se almacenó.

El formato **JPG** es el que **mayor tasa de compresión consigue en imágenes reales** (foto exterior, objetos, texturas..), en **imágenes de paisajes** ó dónde los objetos no se encuentren cerca del objetivo aplicando un **parámetro Q=75** (tal y como vimos en clase es un umbral de "calidad" que permite conseguir una buena compresión sin que el ojo humano periciba peor calidad) conseguimos una imagen de calidad. Por otro lado cuando fotografiamos **objetos cercanos** con mucho detalle necesitamos usar un parámetro de compresión **Q=100**.

El formato **PNG** por su forma de estructurar las imágenes es el que mejor tasa de compresión y calidad consigue en **imágenes que mezclan texto y gráficos**.

El formato **JPG2000** no lo conocía antes de cursar esta asignatura, es más he necesitado buscar un programa que pudiese visualizar dicho formato. El resltado de aplicar distintos parámetros de compresión ha sido totalmente el visto en clase, **a medida que aumentamos dicho parámetro vamos tornando la imagen más borrosa** hasta el punto de no apreciar nada de detalle. Aunque **no comete los fallos de su "padre"** de **pixelar por bloques**, la **imagen** aunque de menor tamaño **queda totalmente borrosa**.

Y por último **GIF** que **funciona bien en imágenes con pocos colores** pero para imágenes reales pierde información de colores notándose por zonas un cambio brusco entre píxeles.

## Comparativa entre JPEG y JPEG2000
Me parecía interesante añadir la siguiente foto para comparar los distintos formatos, en ella podemos ver lo visto en clase por un lado en la segunda fila observamos como la imagen se va pixelando por bloques, mientras que en la primera fila el efecto negativo de aplicar la compresión es un emborronado de la imagen.

**JPEG2000**


![alt text][buddy]


**JPEG**



## Referencias
+ Programa para convertir las imágenes -> http://www.xnview.com/en/xnconvert/#downloads
+ Programa para crear collages -> https://www.befunky.com/es/crear/collage/
+ Programa para visualizar JPEG2000 -> http://openseeit.sourceforge.net/
+ Enlace a mi github para visualizar trabajo con mejor estilo ->


[originales]: http://i64.tinypic.com/72rig1.jpg "Fotos originales"
[buddy]: http://i68.tinypic.com/hvxvma.png "Comparativa entre JPG y JPG2000"

