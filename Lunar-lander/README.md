#Lunar lander
Proyecto de juego en HTML5+CSS3+JavaScript. Actualmente solo está diseñado el esquema de un juego en HTML+CSS. Próximamente se añadirá el motor del juego en JavaScript.

#### Autor: _Marc Hernández Cabot_

#### Diseño original: Óscar, Jamal, Lamiae El Wahabi, Isabel

_**Nota**: Pueden verse estos diseños originales en la carpeta "mockups"._



##Notas sobre el diseño en HTML:
Se ha intentado respetar al máximo el original.

Los cambios realizados en el diseño han sido:

- El medidor de Velocidad ahora muestra la palabra “Vel.” y no “Speed”.
	Motivo: Por cuestiones de coherencia, se ha decidido que los tres indicadores estén en el mismo idioma y no en idiomas distintos (en el diseño propuesto las palabras que aparecían era “Fuel”, “Speed”, “Altitud”.

- El botón reiniciar ha desaparecido.
Motivo: Por cuestiones prácticas, el juego podrá reiniciarse si se ha pausado, pero no mientras se juega (ya que, entre otras cosas, y especialmente si se juega en el móvil, podría reiniciarse sin querer).

- El fondo se ha dividido en 4 partes: El fondo estrellado, el planeta azul, la estrella y el suelo lunar.
	Motivo: El suelo se ha separado por cuestiones de jugabilidad. El resto de elementos (planeta y estrella) se han separado para evitar que se deformen con una redimensión del fondo, y para permitir un tratamiento responsive.


##TRATAMIENTO DE IMÁGENES
El diseño de los elementos gráficos de este juego: los botones, la nave espacial, etc. fueron realizados íntegramente por el cliente con un programa de diseño vectorial; y él mismo me explicó su deseo de mantenerlos en la medida de lo posible. Por este motivo el tratamiento dado a las imágenes se ha hecho con la máxima precaución, respetando al máximo los diseños originales. La parte quizás más controvertida ha sido el tratamiento que se le ha dado al fondo, pero el resultado obtenido respeta al máximo el diseño original.

_**Notas**: Los archivos originales pueden verse en la carpeta "mockups". Todas las imágenes han sido tratadas en png._

###Botones "play" y "pause"
Se ha reducido el margen transparente, se ha reducido la paleta de colores (indexado) y se han optimizado con un software de optimización. El tamaño de los archivos resultantes es aprox. un 60% menos (sin pérdida de calidad aparente).

###Botón "propulsor"
Se ha eliminado el texto, se ha reducido el margen transparente, se ha reducido la paleta de colores (indexado) y se han optimizado con un software de optimización. El tamaño del archivo resultante es aprox. un 70% menos (sin pérdida de calidad aparente). 

Se ha añadido el texto como texto flotante (en el archivo html). Tras consultarlo con el cliente, se ha corregido el texto (en la imagen original contenía un error ortográfico, pues aparecía la palabra “Proulsor” en lugar de la correcta: “Propulsor”). El color utilizado para las letras fue exactamente el que había utilizado el cliente: #C7D541. La tipografía que se solicita al navegador es, por este orden: Helvetica, Arial, Sans-Serif.

###Fondo
El fondo aportado tiene implícitas varias limitaciones que impiden su uso en un diseño responsive.
* Los planetas están fijos, por lo que con un cambio de pantalla aparecerían deformados.
* La superficie lunar está incrustada en el fondo, lo que impide un tratamiento independiente.

Por esos motivos:
Se han separado la superficie lunar, el planeta y el sol en otras imágenes independientes. También se ha creado un patrón cuadrado estrellado basándose en el fondo, de forma que pueda repetirse en forma de mosaico mediante CSS. Ambas medidas permiten un tratamiento responsive del fondo.
