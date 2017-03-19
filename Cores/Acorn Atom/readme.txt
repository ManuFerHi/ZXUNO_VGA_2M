TEST1 (17-Ago-2015)

El código original del usuario Hoglet, en el que se ha basado el port, está disponible aquí: https://github.com/hoglet67/AtomFpga.

Post escrito por Quest originalmente en Zona de Pruebas.
Enlace original:
http://www.zonadepruebas.com/viewtopic. ... 754#p59754

Otro sistema más funcional en el ZX-UNO (Y van 5) :D

En esta ocasión he portado el core del Acorn Atom
Más abajo pongo el link de descarga del bitfile / mcs para el que lo quiera probar :)

Tiene soporte para cargar el software con tarjeta SD.

Como en la ocasión anterior con el de SMS, ha habido que remapear todos los pines, crear nuevos relojes a aprtir de nuestro oscilador de 50Mhz, eliminar señales que daban problemas (como las de los joystick), cambiar ligeramente el código del teclado para que funcionara en el ZX-UNO, etc. El código original, en el que se ha basado el port está disponible aquí: https://github.com/hoglet67/AtomFpga , del usuario Hoglet.

Para hacerlo funcionar en el ZX-UNO:

- Meter el bitfile a la FPGA (o el mcs para la flash)
- Enchufar un teclado PS/2 al l ZX-UNO
- Enchufar la plaquita VGA al conector J8 y conectarlo a un monitor VGA normal. (no va por vídeo compuesto, sólo VGA de momento)
- Enchufar el jack de salida de audio a unos altavoces.
- Preparar una tarjeta SD formateada en FAT. Bajad de aquí: http://www.stardot.org.uk/forums/viewto ... =44&t=6544 el archivo "AtomSoftwareArchive_20150504_V8.zip" y descomprimidlo tal cual en la raíz de la SD (si no va la SD, probad con otra distinta). Y meterla en el ZX-UNO.

Y ahora, a funcionar:

- Al enchufar el ZX-UNO ya arranca en modo BASIC del Atom. El bitfile del core ya viene con la extensión AtoMMC2 incorporada, con lo cual, disponemos de carga mediante la SD:
- Para lanzar el menú de selección de software que hemos cargado en la SD previamente, pulsamos SHIFT+F10 (si no va a la primera intentarlo más veces, a veces no va 100% fino)
- A disfrutar.

- Para volver a sacar el menú: SHIFT+10
- Resetear el Atom: F10
- Modos turbo: F1 = 1Mhz, F2 = 2Mhz, F3 = 4Mhz, F4 = 8Mhz
- El mapeado del teclado es inglés. Tenedlo en cuenta, porque no coinciden algunas teclas con el español. Mirad una foto de uno inglés para comparar.