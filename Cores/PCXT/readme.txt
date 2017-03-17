Autor Distwave.

- Eliminado el PSG para el sonido Tandy 3-voice. Se ha reducido notablemente el ruido de fondo.
- Solucionados los gitches en modo texto.
- BIOS Incorporada en el core, ya no es necesario grabarla en los últimos 8 KB de la SD. Ahora se aloja en la BRAM utilizada como memoria de vídeo y el bootloader la copia a la memoria RAM en el primer arranque (tal y como sugirió antoniovillena).
- Frecuencia de trabajo de la memoria SRAM aumentada de 50 MHz a 75 MHz. Este cambio aumenta el rendimiento del core notablemente, aunque el procesador siga funcionando a 25 MHz.
- Mapeo directo de los 2 MB de SRAM en los primeros 2 MB direccionables. La distribución de la memoria queda de la siguiente forma:
· 640 KB de memoria convencional
· 224 KB de memoria superior
· 32 KB para alojar la BIOS
· 64 KB de memoria alta
· 448 KB de memoria extendida (XMS)
