TEST1 (8-Ene-2016)

Es un port del trabajo original de David Banks (hoglet), como todo lo que tenemos de Acorn hasta el momento (fuentes originales en https://github.com/hoglet67/ElectronFpga).

Salida vídeo compuesto/RGB y VGA 50Hz seleccionables vía teclado. Por defecto arranca en RGB/Vcomp. Tecla RePag = VGA, tecla AvPag = RGB/Vcomp. También hay otros modos (60Hz, etc) usando combinaciones de ctrl+CapsLock+1 al 4)
Soporte SD/MMC, vía archivos de imagen ".MMB" (BEEB.MMB, que son contenedores de imágenes de disquete). Explicado más abajo para que funcione correctamente (al igual que pasa con el core de BBC Micro)
Carga de software via cinta/audo por el puerto EAR del ZX-UNO.
Teclado PS/2 (mapeado a teclado inglés)
Sonido estándar.
Reset (tecla F10 y ctrl+F10)