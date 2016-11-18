#Lunar lander

Este es el esquema de un juego diseñado en HTML+CSS. Próximamente se añadirá el motor del juego en JavaScript.


###Diseño original: 
- Óscar Jamal, Lamiae El Wahabi, Isabel

###Diseño en HTML+CSS:
- Marc Hernández Cabot


###Notas sobre el diseño en HTML:
Se ha intentado respetar al máximo el original.

Los cambios realizados en el diseño han sido:

- El medidor de Velocidad ahora muestra la palabra “Velocidad” y no “Speed”.
	Motivo: Por cuestiones de coherencia, se ha decidido que los tres indicadores estén en el mismo idioma y no en idiomas distintos (en el diseño propuesto las palabras que aparecían era “Fuel”, “Speed”, “Altitud”.

- El botón reiniciar ha desaparecido.
Motivo: Por cuestiones prácticas, el juego podrá reiniciarse si se ha pausado, pero no mientras se juega (ya que, entre otras cosas, y especialmente si se juega en el móvil, podría reiniciarse sin querer).

- El fondo se ha dividido en 4 partes: El fondo estrellado, el planeta azul, la estrella y el suelo lunar.
	Motivo: El suelo se ha separado por cuestiones de jugabilidad. El resto de elementos (planeta y estrella) se han separado para evitar que se deformen con una redimensión del fondo, y para permitir un tratamiento responsive.
