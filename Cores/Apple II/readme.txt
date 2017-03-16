TEST3 (06-Sep-2016)

Añadidas tarjetas de expansión de RAM. 128K Saturn RAM (slot 5) + 16K Language card (slot 0).
Reescrito y sustituido completamente el core de teclado ps/2. Ahora es mucho más estable.
Añadida combinación Master Reset (Ctrl + Alt + Backspace) para volver al core de Spectrum (como estamos haciendo de foma estándar para todos los cores, paulatinamente)
Eliminado Reset externo para mayor estabilidad. El reset en frío ahora es únicamente interno.
Reset en frío (tecla F12) mejorado, inicializando porción de SRAM (0x3F4), para que tras cada reset siempre arranque de la unidad de disco y no haya corrupciones.
Añadida función de scanlines VGA, activable mediante la tecla "-" del teclado numérico. (EXPERIMENTAL. Aún hay que ajustar timings)
Añadida función de cambio de tipo de monitor Color / Blanco y negro, activable mediante la tecla "*" del teclado numérico
Arreglado botón 2 del joystick, ahora funciona.
Aumentada la capacidad de arrancar desde imágenes de disco en SD (RAW), ahora se pueden insertar hasta 20 imágenes de disco distintas. Las primeras 10 pulsando de F1 a F10 y las siguientes 10, pulsando de SHIFT+F1 a SHIFT+F10.